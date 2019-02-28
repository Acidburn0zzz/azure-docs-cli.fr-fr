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
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158356"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="8ef6d-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="8ef6d-104">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="8ef6d-104">February 12, 2019</span></span>

<span data-ttu-id="8ef6d-105">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="8ef6d-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-106">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-106">Core</span></span>

* <span data-ttu-id="8ef6d-107">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="8ef6d-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="8ef6d-108">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="8ef6d-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-109">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-109">ACR</span></span>
* <span data-ttu-id="8ef6d-110">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="8ef6d-111">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-112">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-112">ACS</span></span>
* <span data-ttu-id="8ef6d-113">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="8ef6d-114">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="8ef6d-115">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="8ef6d-116">AMS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-116">AMS</span></span>
* <span data-ttu-id="8ef6d-117">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="8ef6d-118">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-119">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-119">Appservice</span></span>
* <span data-ttu-id="8ef6d-120">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="8ef6d-121">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="8ef6d-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="8ef6d-122">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="8ef6d-123">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="8ef6d-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="8ef6d-124">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="8ef6d-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="8ef6d-125">Botservice</span><span class="sxs-lookup"><span data-stu-id="8ef6d-125">Botservice</span></span>
* <span data-ttu-id="8ef6d-126">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="8ef6d-127">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="8ef6d-128">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="8ef6d-129">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="8ef6d-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="8ef6d-130">[DÉPRÉCIÉ] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="8ef6d-131">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="8ef6d-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="8ef6d-132">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="8ef6d-133">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="8ef6d-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="8ef6d-134">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="8ef6d-135">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="8ef6d-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="8ef6d-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-136">Key Vault</span></span>
* <span data-ttu-id="8ef6d-137">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-138">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-138">Monitor</span></span>
* <span data-ttu-id="8ef6d-139">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-140">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-140">Network</span></span>
* <span data-ttu-id="8ef6d-141">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="8ef6d-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="8ef6d-142">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="8ef6d-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="8ef6d-143">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="8ef6d-144">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="8ef6d-145">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="8ef6d-145">Policy Insights</span></span>
* <span data-ttu-id="8ef6d-146">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="8ef6d-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-147">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-147">RDBMS</span></span>
* <span data-ttu-id="8ef6d-148">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="8ef6d-149">Redis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-149">Redis</span></span>
* <span data-ttu-id="8ef6d-150">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="8ef6d-151">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="8ef6d-152">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="8ef6d-153">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="8ef6d-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="8ef6d-154">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="8ef6d-155">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="8ef6d-156">[DÉPRÉCIÉ] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-157">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-157">Role</span></span>
* <span data-ttu-id="8ef6d-158">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="8ef6d-159">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-159">SQL VM</span></span>
* <span data-ttu-id="8ef6d-160">[DÉPRÉCIÉ] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-161">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-161">VM</span></span>
* <span data-ttu-id="8ef6d-162">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="8ef6d-163">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="8ef6d-164">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="8ef6d-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="8ef6d-165">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="8ef6d-166">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="8ef6d-166">January 31, 2019</span></span>

<span data-ttu-id="8ef6d-167">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="8ef6d-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-168">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-168">Core</span></span>

* <span data-ttu-id="8ef6d-169">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="8ef6d-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="8ef6d-170">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="8ef6d-170">January 28, 2019</span></span>

<span data-ttu-id="8ef6d-171">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="8ef6d-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-172">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-172">ACR</span></span>
* <span data-ttu-id="8ef6d-173">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="8ef6d-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-174">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-174">ACS</span></span>
* <span data-ttu-id="8ef6d-175">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="8ef6d-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="8ef6d-176">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="8ef6d-177">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="8ef6d-178">AMS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-178">AMS</span></span>
* <span data-ttu-id="8ef6d-179">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="8ef6d-180">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-181">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-181">Appservice</span></span>
* <span data-ttu-id="8ef6d-182">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="8ef6d-183">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="8ef6d-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="8ef6d-184">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="8ef6d-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-185">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-185">Container</span></span>
* <span data-ttu-id="8ef6d-186">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-186">Added `container start` command</span></span>
* <span data-ttu-id="8ef6d-187">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8ef6d-188">EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ef6d-188">EventGrid</span></span>
* <span data-ttu-id="8ef6d-189">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="8ef6d-190">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="8ef6d-191">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="8ef6d-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="8ef6d-192">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="8ef6d-193">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8ef6d-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ef6d-194">HDInsight</span></span>
* <span data-ttu-id="8ef6d-195">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="8ef6d-196">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="8ef6d-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="8ef6d-197">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="8ef6d-198">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="8ef6d-199">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="8ef6d-200">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-201">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-201">IoT</span></span>
* <span data-ttu-id="8ef6d-202">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="8ef6d-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="8ef6d-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="8ef6d-203">Kusto</span></span>
* <span data-ttu-id="8ef6d-204">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-205">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-205">Monitor</span></span>
* <span data-ttu-id="8ef6d-206">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-207">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-207">Profile</span></span>
* <span data-ttu-id="8ef6d-208">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-209">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-209">Network</span></span>
* <span data-ttu-id="8ef6d-210">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="8ef6d-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="8ef6d-211">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="8ef6d-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-212">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-212">Resource</span></span>
* <span data-ttu-id="8ef6d-213">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="8ef6d-214">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="8ef6d-215">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="8ef6d-216">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-217">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-217">Storage</span></span>
* <span data-ttu-id="8ef6d-218">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="8ef6d-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="8ef6d-219">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-220">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-220">VM</span></span>
* <span data-ttu-id="8ef6d-221">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="8ef6d-222">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="8ef6d-223">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="8ef6d-223">January 15, 2019</span></span>

<span data-ttu-id="8ef6d-224">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="8ef6d-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-225">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-225">ACR</span></span>
* <span data-ttu-id="8ef6d-226">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="8ef6d-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="8ef6d-227">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="8ef6d-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="8ef6d-228">[DÉPRÉCIÉ] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="8ef6d-229">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-229">ACS</span></span>
* <span data-ttu-id="8ef6d-230">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-231">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-231">Appservice</span></span>
* <span data-ttu-id="8ef6d-232">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="8ef6d-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="8ef6d-233">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="8ef6d-234">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="8ef6d-235">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="8ef6d-236">Botservice</span><span class="sxs-lookup"><span data-stu-id="8ef6d-236">Botservice</span></span>
* <span data-ttu-id="8ef6d-237">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="8ef6d-238">Configuration</span><span class="sxs-lookup"><span data-stu-id="8ef6d-238">Configure</span></span>
* <span data-ttu-id="8ef6d-239">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="8ef6d-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-240">CosmosDB</span></span>
* <span data-ttu-id="8ef6d-241">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8ef6d-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ef6d-242">HDInsight</span></span>
* <span data-ttu-id="8ef6d-243">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="8ef6d-243">Added commands for managing applications</span></span>
* <span data-ttu-id="8ef6d-244">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="8ef6d-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="8ef6d-245">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="8ef6d-246">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="8ef6d-247">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-248">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-248">Network</span></span>
* <span data-ttu-id="8ef6d-249">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="8ef6d-250">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="8ef6d-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="8ef6d-251">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="8ef6d-252">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-253">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-253">Role</span></span>
* <span data-ttu-id="8ef6d-254">[DÉPRÉCIÉ] Dépréciation de l’argument `--password` au profit de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="8ef6d-255">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="8ef6d-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="8ef6d-256">Sécurité</span><span class="sxs-lookup"><span data-stu-id="8ef6d-256">Security</span></span>
* <span data-ttu-id="8ef6d-257">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-258">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-258">Storage</span></span>
* <span data-ttu-id="8ef6d-259">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="8ef6d-260">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="8ef6d-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="8ef6d-261">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="8ef6d-262">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="8ef6d-263">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-264">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-264">VM</span></span>
* <span data-ttu-id="8ef6d-265">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="8ef6d-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="8ef6d-266">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8ef6d-267">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="8ef6d-268">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="8ef6d-269">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="8ef6d-270">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="8ef6d-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="8ef6d-271">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-271">December 20, 2018</span></span>

<span data-ttu-id="8ef6d-272">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="8ef6d-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="8ef6d-273">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-273">Appservice</span></span>
* <span data-ttu-id="8ef6d-274">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="8ef6d-275">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="8ef6d-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="8ef6d-276">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="8ef6d-277">IotCentral</span><span class="sxs-lookup"><span data-stu-id="8ef6d-277">IoTCentral</span></span>
* <span data-ttu-id="8ef6d-278">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="8ef6d-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-279">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-279">Role</span></span>
* <span data-ttu-id="8ef6d-280">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-281">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-281">SQL</span></span>
* <span data-ttu-id="8ef6d-282">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-283">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-283">VM</span></span>
* <span data-ttu-id="8ef6d-284">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="8ef6d-285">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-285">December 18, 2018</span></span>

<span data-ttu-id="8ef6d-286">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="8ef6d-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="8ef6d-287">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-287">ACR</span></span>
* <span data-ttu-id="8ef6d-288">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="8ef6d-289">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="8ef6d-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="8ef6d-290">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="8ef6d-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-291">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-291">ACS</span></span>
* <span data-ttu-id="8ef6d-292">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="8ef6d-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="8ef6d-293">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="8ef6d-294">[DÉCONSEILLÉ] Commandes `az acs` déconseillées.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="8ef6d-295">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="8ef6d-296">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="8ef6d-297">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="8ef6d-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-298">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-298">Appservice</span></span>
* <span data-ttu-id="8ef6d-299">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="8ef6d-300">Botservice</span><span class="sxs-lookup"><span data-stu-id="8ef6d-300">Botservice</span></span>
* <span data-ttu-id="8ef6d-301">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="8ef6d-302">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="8ef6d-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="8ef6d-303">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="8ef6d-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="8ef6d-304">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="8ef6d-305">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="8ef6d-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-306">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-306">Consumption</span></span>
* <span data-ttu-id="8ef6d-307">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="8ef6d-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-308">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-308">CosmosDB</span></span>
* <span data-ttu-id="8ef6d-309">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="8ef6d-310">Cartes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-310">Maps</span></span>
* <span data-ttu-id="8ef6d-311">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-312">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-312">Network</span></span>
* <span data-ttu-id="8ef6d-313">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="8ef6d-314">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="8ef6d-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-315">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-315">Resource</span></span>
* <span data-ttu-id="8ef6d-316">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="8ef6d-317">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-318">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-318">Storage</span></span>
*  <span data-ttu-id="8ef6d-319">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-320">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-320">VM</span></span>
* <span data-ttu-id="8ef6d-321">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="8ef6d-322">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-322">December 4, 2018</span></span>

<span data-ttu-id="8ef6d-323">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="8ef6d-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="8ef6d-324">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-324">Core</span></span>
* <span data-ttu-id="8ef6d-325">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="8ef6d-326">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-327">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-327">Appservice</span></span>
* <span data-ttu-id="8ef6d-328">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="8ef6d-329">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-330">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-330">Network</span></span>
* <span data-ttu-id="8ef6d-331">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="8ef6d-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-332">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-332">Role</span></span>
* <span data-ttu-id="8ef6d-333">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="8ef6d-334">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-334">VM</span></span>
* <span data-ttu-id="8ef6d-335">[DÉCONSEILLÉ] Le paramètre `vm extension [show|wait] --expand` est déconseillé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="8ef6d-336">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="8ef6d-337">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="8ef6d-338">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="8ef6d-339">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-339">November 20, 2018</span></span>

<span data-ttu-id="8ef6d-340">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="8ef6d-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="8ef6d-341">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-341">Core</span></span>
* <span data-ttu-id="8ef6d-342">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="8ef6d-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-343">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-343">ACR</span></span>
* <span data-ttu-id="8ef6d-344">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="8ef6d-344">Added context token to task step</span></span>
* <span data-ttu-id="8ef6d-345">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="8ef6d-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="8ef6d-346">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-347">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-347">Appservice</span></span>
* <span data-ttu-id="8ef6d-348">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="8ef6d-349">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-349">Updated the default `node_version`.</span></span> <span data-ttu-id="8ef6d-350">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="8ef6d-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="8ef6d-351">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="8ef6d-352">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="8ef6d-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="8ef6d-353">IotCentral</span><span class="sxs-lookup"><span data-stu-id="8ef6d-353">IotCentral</span></span>
* <span data-ttu-id="8ef6d-354">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="8ef6d-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-355">KeyVault</span></span>
* <span data-ttu-id="8ef6d-356">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-357">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-357">Network</span></span>
* <span data-ttu-id="8ef6d-358">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="8ef6d-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="8ef6d-359">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="8ef6d-360">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="8ef6d-361">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8ef6d-362">Rdbms</span></span>
* <span data-ttu-id="8ef6d-363">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="8ef6d-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="8ef6d-364">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-364">Rbac</span></span>
* <span data-ttu-id="8ef6d-365">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="8ef6d-366">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="8ef6d-367">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-367">Storage</span></span>
* <span data-ttu-id="8ef6d-368">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="8ef6d-369">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="8ef6d-370">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="8ef6d-371">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-372">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-372">VM</span></span>
* <span data-ttu-id="8ef6d-373">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="8ef6d-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="8ef6d-374">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="8ef6d-375">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="8ef6d-376">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="8ef6d-377">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="8ef6d-378">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="8ef6d-379">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="8ef6d-380">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-380">November 6, 2018</span></span>

<span data-ttu-id="8ef6d-381">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="8ef6d-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-382">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-382">Core</span></span>
* <span data-ttu-id="8ef6d-383">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="8ef6d-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-384">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-384">ACR</span></span>
* <span data-ttu-id="8ef6d-385">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="8ef6d-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="8ef6d-386">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="8ef6d-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-387">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-387">ACS</span></span>
* <span data-ttu-id="8ef6d-388">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="8ef6d-389">Advisor</span><span class="sxs-lookup"><span data-stu-id="8ef6d-389">Advisor</span></span>
* <span data-ttu-id="8ef6d-390">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="8ef6d-391">AMS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-391">AMS</span></span>
* <span data-ttu-id="8ef6d-392">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="8ef6d-393">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="8ef6d-394">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="8ef6d-395">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="8ef6d-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="8ef6d-396">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="8ef6d-397">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="8ef6d-398">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="8ef6d-399">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="8ef6d-400">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="8ef6d-401">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="8ef6d-402">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="8ef6d-403">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="8ef6d-404">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="8ef6d-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="8ef6d-405">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="8ef6d-406">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="8ef6d-407">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="8ef6d-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="8ef6d-408">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-409">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-409">AppService</span></span>
* <span data-ttu-id="8ef6d-410">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="8ef6d-411">Configuration</span><span class="sxs-lookup"><span data-stu-id="8ef6d-411">Configure</span></span>
* <span data-ttu-id="8ef6d-412">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-413">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-413">Container</span></span>
* <span data-ttu-id="8ef6d-414">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="8ef6d-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="8ef6d-415">Event Hub</span><span class="sxs-lookup"><span data-stu-id="8ef6d-415">EventHub</span></span>
* <span data-ttu-id="8ef6d-416">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-417">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-417">Interactive</span></span>
* <span data-ttu-id="8ef6d-418">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="8ef6d-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-419">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-419">Monitor</span></span>
* <span data-ttu-id="8ef6d-420">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-421">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-421">Network</span></span>
* <span data-ttu-id="8ef6d-422">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="8ef6d-423">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="8ef6d-424">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="8ef6d-425">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-425">Profile</span></span>
* <span data-ttu-id="8ef6d-426">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-427">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-427">RDBMS</span></span>
* <span data-ttu-id="8ef6d-428">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="8ef6d-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-429">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-429">Resource</span></span>
* <span data-ttu-id="8ef6d-430">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-431">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-431">Role</span></span>
* <span data-ttu-id="8ef6d-432">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="8ef6d-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="8ef6d-433">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="8ef6d-434">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="8ef6d-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-435">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-435">Storage</span></span>
* <span data-ttu-id="8ef6d-436">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-437">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-437">VM</span></span>
* <span data-ttu-id="8ef6d-438">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="8ef6d-439">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="8ef6d-440">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="8ef6d-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="8ef6d-441">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="8ef6d-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="8ef6d-442">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="8ef6d-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="8ef6d-443">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="8ef6d-444">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-444">October 23, 2018</span></span>

<span data-ttu-id="8ef6d-445">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="8ef6d-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-446">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-446">Core</span></span>
* <span data-ttu-id="8ef6d-447">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="8ef6d-448">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-449">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-449">ACR</span></span>
* <span data-ttu-id="8ef6d-450">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="8ef6d-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="8ef6d-451">CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-451">CDN</span></span>
* <span data-ttu-id="8ef6d-452">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="8ef6d-453">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-454">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-454">Container</span></span>
* <span data-ttu-id="8ef6d-455">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="8ef6d-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="8ef6d-456">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="8ef6d-457">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="8ef6d-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="8ef6d-458">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="8ef6d-459">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="8ef6d-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="8ef6d-460">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="8ef6d-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="8ef6d-461">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-462">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-462">CosmosDB</span></span>
* <span data-ttu-id="8ef6d-463">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-464">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-464">Interactive</span></span>
* <span data-ttu-id="8ef6d-465">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="8ef6d-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="8ef6d-466">IoT Central</span><span class="sxs-lookup"><span data-stu-id="8ef6d-466">IoT Central</span></span>
* <span data-ttu-id="8ef6d-467">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="8ef6d-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="8ef6d-468">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="8ef6d-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-469">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-469">Monitor</span></span>
* <span data-ttu-id="8ef6d-470">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="8ef6d-471">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="8ef6d-472">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="8ef6d-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="8ef6d-473">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="8ef6d-474">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="8ef6d-475">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="8ef6d-476">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="8ef6d-477">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="8ef6d-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="8ef6d-478">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="8ef6d-479">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-480">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-480">Network</span></span>
* <span data-ttu-id="8ef6d-481">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="8ef6d-482">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="8ef6d-483">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-483">ServiceBus</span></span>
* <span data-ttu-id="8ef6d-484">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-485">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-485">SQL</span></span>
* <span data-ttu-id="8ef6d-486">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-487">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-487">Storage</span></span>
* <span data-ttu-id="8ef6d-488">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="8ef6d-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="8ef6d-489">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-490">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-490">VM</span></span>
* <span data-ttu-id="8ef6d-491">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="8ef6d-492">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="8ef6d-493">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="8ef6d-494">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-494">October 16, 2018</span></span>

<span data-ttu-id="8ef6d-495">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="8ef6d-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-496">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-496">VM</span></span>
* <span data-ttu-id="8ef6d-497">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="8ef6d-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="8ef6d-498">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-498">October 9, 2018</span></span>

<span data-ttu-id="8ef6d-499">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="8ef6d-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-500">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-500">Core</span></span>
* <span data-ttu-id="8ef6d-501">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-502">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-502">ACR</span></span>
* <span data-ttu-id="8ef6d-503">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="8ef6d-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-504">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-504">ACS</span></span>
* <span data-ttu-id="8ef6d-505">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="8ef6d-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="8ef6d-506">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="8ef6d-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="8ef6d-507">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="8ef6d-508">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-509">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-509">Container</span></span>
* <span data-ttu-id="8ef6d-510">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="8ef6d-511">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="8ef6d-512">Event Hub</span><span class="sxs-lookup"><span data-stu-id="8ef6d-512">Event Hub</span></span>
* <span data-ttu-id="8ef6d-513">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="8ef6d-514">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="8ef6d-515">Extensions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-515">Extensions</span></span>
* <span data-ttu-id="8ef6d-516">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8ef6d-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ef6d-517">HDInsight</span></span>
* <span data-ttu-id="8ef6d-518">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-519">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-519">IoT</span></span>
* <span data-ttu-id="8ef6d-520">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="8ef6d-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-521">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-521">KeyVault</span></span>
* <span data-ttu-id="8ef6d-522">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="8ef6d-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-523">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-523">Network</span></span>
* <span data-ttu-id="8ef6d-524">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="8ef6d-525">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="8ef6d-525">See #6052</span></span>
* <span data-ttu-id="8ef6d-526">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="8ef6d-527">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="8ef6d-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="8ef6d-528">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="8ef6d-529">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="8ef6d-530">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="8ef6d-531">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-532">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-532">Role</span></span>
* <span data-ttu-id="8ef6d-533">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="8ef6d-534">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="8ef6d-535">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="8ef6d-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="8ef6d-536">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="8ef6d-537">Service Bus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-537">Service Bus</span></span>
* <span data-ttu-id="8ef6d-538">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-539">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-539">VM</span></span>
* <span data-ttu-id="8ef6d-540">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="8ef6d-541">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="8ef6d-542">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="8ef6d-543">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="8ef6d-544">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="8ef6d-545">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="8ef6d-546">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-546">September 21, 2018</span></span>

<span data-ttu-id="8ef6d-547">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="8ef6d-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-548">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-548">ACR</span></span>
* <span data-ttu-id="8ef6d-549">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-549">Added ACR Task commands</span></span>
* <span data-ttu-id="8ef6d-550">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-550">Added quick run command</span></span>
* <span data-ttu-id="8ef6d-551">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="8ef6d-552">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="8ef6d-553">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="8ef6d-554">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="8ef6d-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-555">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-555">ACS</span></span>
* <span data-ttu-id="8ef6d-556">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="8ef6d-557">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="8ef6d-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-558">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-558">AppService</span></span>

* <span data-ttu-id="8ef6d-559">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="8ef6d-560">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="8ef6d-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="8ef6d-561">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="8ef6d-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="8ef6d-562">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-563">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-563">Batch</span></span>
* <span data-ttu-id="8ef6d-564">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="8ef6d-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="8ef6d-565">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="8ef6d-566">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="8ef6d-567">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8ef6d-568">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-568">Batch AI</span></span> 
* <span data-ttu-id="8ef6d-569">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8ef6d-570">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-570">Cognitive Services</span></span>
* <span data-ttu-id="8ef6d-571">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="8ef6d-572">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="8ef6d-573">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="8ef6d-574">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="8ef6d-575">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="8ef6d-576">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-577">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-577">Container</span></span>
* <span data-ttu-id="8ef6d-578">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="8ef6d-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="8ef6d-579">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="8ef6d-580">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="8ef6d-581">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="8ef6d-582">DataLake</span><span class="sxs-lookup"><span data-stu-id="8ef6d-582">Datalake</span></span>
* <span data-ttu-id="8ef6d-583">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="8ef6d-584">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-584">Interactive Shell</span></span>
* <span data-ttu-id="8ef6d-585">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="8ef6d-586">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-587">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-587">IoT</span></span>
* <span data-ttu-id="8ef6d-588">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="8ef6d-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-589">Key Vault</span></span>
* <span data-ttu-id="8ef6d-590">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="8ef6d-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-591">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-591">Network</span></span>
* <span data-ttu-id="8ef6d-592">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="8ef6d-593">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="8ef6d-594">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="8ef6d-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="8ef6d-595">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="8ef6d-596">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="8ef6d-597">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="8ef6d-598">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="8ef6d-599">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="8ef6d-600">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="8ef6d-601">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="8ef6d-602">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="8ef6d-603">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="8ef6d-604">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="8ef6d-605">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="8ef6d-606">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="8ef6d-607">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="8ef6d-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="8ef6d-608">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="8ef6d-609">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-610">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-610">RDBMS</span></span>
* <span data-ttu-id="8ef6d-611">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="8ef6d-612">Réservation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-612">Reservation</span></span>
* <span data-ttu-id="8ef6d-613">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="8ef6d-614">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="8ef6d-615">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="8ef6d-615">Manage App</span></span>
* <span data-ttu-id="8ef6d-616">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="8ef6d-617">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="8ef6d-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-618">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-618">Role</span></span>
* <span data-ttu-id="8ef6d-619">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="8ef6d-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-620">SignalR</span></span>
* <span data-ttu-id="8ef6d-621">Première version</span><span class="sxs-lookup"><span data-stu-id="8ef6d-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-622">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-622">Storage</span></span>
* <span data-ttu-id="8ef6d-623">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="8ef6d-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="8ef6d-624">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="8ef6d-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-625">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-625">VM</span></span>
* <span data-ttu-id="8ef6d-626">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="8ef6d-627">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="8ef6d-628">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-628">August 28, 2018</span></span>

<span data-ttu-id="8ef6d-629">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="8ef6d-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-630">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-630">Core</span></span>

* <span data-ttu-id="8ef6d-631">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="8ef6d-632">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8ef6d-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-633">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-633">ACR</span></span>

* <span data-ttu-id="8ef6d-634">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="8ef6d-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="8ef6d-635">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-636">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-636">ACS</span></span>

* <span data-ttu-id="8ef6d-637">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="8ef6d-638">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="8ef6d-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-639">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-639">AppService</span></span>

* <span data-ttu-id="8ef6d-640">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="8ef6d-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="8ef6d-641">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="8ef6d-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="8ef6d-642">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="8ef6d-643">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="8ef6d-643">Backup</span></span>

* <span data-ttu-id="8ef6d-644">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="8ef6d-645">Service de robot</span><span class="sxs-lookup"><span data-stu-id="8ef6d-645">Bot Service</span></span>

* <span data-ttu-id="8ef6d-646">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8ef6d-647">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-647">Cognitive Services</span></span>

* <span data-ttu-id="8ef6d-648">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-649">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-649">IoT</span></span>

* <span data-ttu-id="8ef6d-650">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-651">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-651">Monitor</span></span>

* <span data-ttu-id="8ef6d-652">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="8ef6d-653">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-654">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-654">Network</span></span>

* <span data-ttu-id="8ef6d-655">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-656">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-656">Resource</span></span>

* <span data-ttu-id="8ef6d-657">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-658">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-658">Storage</span></span>

* <span data-ttu-id="8ef6d-659">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-660">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-660">VM</span></span>

* <span data-ttu-id="8ef6d-661">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="8ef6d-662">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="8ef6d-663">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-663">Auguest 14, 2018</span></span>

<span data-ttu-id="8ef6d-664">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="8ef6d-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-665">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-665">Core</span></span>

* <span data-ttu-id="8ef6d-666">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="8ef6d-667">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="8ef6d-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="8ef6d-668">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-668">Telemetry</span></span>

* <span data-ttu-id="8ef6d-669">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-670">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-670">ACR</span></span>

* <span data-ttu-id="8ef6d-671">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="8ef6d-672">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-673">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-673">ACS</span></span>

* <span data-ttu-id="8ef6d-674">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="8ef6d-675">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="8ef6d-676">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="8ef6d-677">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="8ef6d-678">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="8ef6d-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="8ef6d-679">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-679">AppService</span></span>

* <span data-ttu-id="8ef6d-680">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="8ef6d-681">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="8ef6d-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="8ef6d-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-682">BatchAI</span></span>

* <span data-ttu-id="8ef6d-683">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="8ef6d-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="8ef6d-684">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-684">Container</span></span>

* <span data-ttu-id="8ef6d-685">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="8ef6d-686">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-686">IoT</span></span>

* <span data-ttu-id="8ef6d-687">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="8ef6d-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="8ef6d-688">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="8ef6d-689">Iot Central</span><span class="sxs-lookup"><span data-stu-id="8ef6d-689">Iot Central</span></span>

* <span data-ttu-id="8ef6d-690">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="8ef6d-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-691">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-691">KeyVault</span></span>


* <span data-ttu-id="8ef6d-692">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="8ef6d-693">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="8ef6d-694">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="8ef6d-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="8ef6d-695">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="8ef6d-696">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="8ef6d-697">Relais</span><span class="sxs-lookup"><span data-stu-id="8ef6d-697">Relay</span></span>

* <span data-ttu-id="8ef6d-698">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-699">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-699">Sql</span></span>

* <span data-ttu-id="8ef6d-700">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-701">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-701">Storage</span></span>

* <span data-ttu-id="8ef6d-702">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="8ef6d-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="8ef6d-703">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="8ef6d-704">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="8ef6d-705">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="8ef6d-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="8ef6d-706">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-707">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-707">VM</span></span>

* <span data-ttu-id="8ef6d-708">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="8ef6d-709">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-709">July 31, 2018</span></span>

<span data-ttu-id="8ef6d-710">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="8ef6d-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-711">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-711">ACR</span></span>

* <span data-ttu-id="8ef6d-712">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="8ef6d-713">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-714">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-714">ACS</span></span>

* <span data-ttu-id="8ef6d-715">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-716">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-716">Batch</span></span>

* <span data-ttu-id="8ef6d-717">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8ef6d-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-718">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-718">Container</span></span>

* <span data-ttu-id="8ef6d-719">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="8ef6d-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-720">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-720">Network</span></span>

* <span data-ttu-id="8ef6d-721">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8ef6d-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="8ef6d-722">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-722">Resource</span></span>

* <span data-ttu-id="8ef6d-723">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="8ef6d-724">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-725">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-725">Role</span></span>

* <span data-ttu-id="8ef6d-726">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="8ef6d-727">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="8ef6d-728">Recherche</span><span class="sxs-lookup"><span data-stu-id="8ef6d-728">Search</span></span>

* <span data-ttu-id="8ef6d-729">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="8ef6d-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="8ef6d-730">Service Bus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-730">Service Bus</span></span>

* <span data-ttu-id="8ef6d-731">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="8ef6d-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="8ef6d-732">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="8ef6d-733">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="8ef6d-734">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-735">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-735">Storage</span></span>

* <span data-ttu-id="8ef6d-736">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="8ef6d-737">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-738">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-738">VM</span></span>

* <span data-ttu-id="8ef6d-739">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="8ef6d-740">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="8ef6d-741">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="8ef6d-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="8ef6d-742">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="8ef6d-743">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-743">July 18, 2018</span></span>

<span data-ttu-id="8ef6d-744">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="8ef6d-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-745">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-745">Core</span></span>

* <span data-ttu-id="8ef6d-746">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="8ef6d-747">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="8ef6d-748">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-749">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-749">ACR</span></span>

* <span data-ttu-id="8ef6d-750">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="8ef6d-751">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="8ef6d-752">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="8ef6d-753">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-754">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-754">ACS</span></span>

* <span data-ttu-id="8ef6d-755">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="8ef6d-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-756">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-756">AppService</span></span>

* <span data-ttu-id="8ef6d-757">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="8ef6d-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-758">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-758">Batch</span></span>

* <span data-ttu-id="8ef6d-759">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8ef6d-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="8ef6d-760">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8ef6d-761">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-761">Batch AI</span></span>

* <span data-ttu-id="8ef6d-762">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-763">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-763">Container</span></span>

* <span data-ttu-id="8ef6d-764">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="8ef6d-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="8ef6d-765">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="8ef6d-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-766">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-766">Network</span></span>

* <span data-ttu-id="8ef6d-767">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="8ef6d-768">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-768">Added `network nic wait`</span></span>
* <span data-ttu-id="8ef6d-769">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="8ef6d-770">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="8ef6d-771">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-771">Resource</span></span>

* <span data-ttu-id="8ef6d-772">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="8ef6d-773">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="8ef6d-774">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="8ef6d-775">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="8ef6d-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-776">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-776">SQL</span></span>

* <span data-ttu-id="8ef6d-777">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="8ef6d-778">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="8ef6d-779">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-780">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-780">Storage</span></span>

* <span data-ttu-id="8ef6d-781">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="8ef6d-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-782">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-782">VM</span></span>

* <span data-ttu-id="8ef6d-783">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="8ef6d-784">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="8ef6d-785">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8ef6d-786">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-786">July 3, 2018</span></span>

<span data-ttu-id="8ef6d-787">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="8ef6d-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="8ef6d-788">AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-788">AKS</span></span>

* <span data-ttu-id="8ef6d-789">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8ef6d-790">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-790">July 3, 2018</span></span>

<span data-ttu-id="8ef6d-791">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="8ef6d-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-792">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-792">Core</span></span>

* <span data-ttu-id="8ef6d-793">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-794">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-794">ACR</span></span>

* <span data-ttu-id="8ef6d-795">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="8ef6d-795">Added polling build status</span></span>
* <span data-ttu-id="8ef6d-796">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="8ef6d-797">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-798">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-798">ACS</span></span>

* <span data-ttu-id="8ef6d-799">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="8ef6d-800">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="8ef6d-801">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="8ef6d-802">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="8ef6d-803">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="8ef6d-804">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="8ef6d-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="8ef6d-805">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-806">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-806">AppService</span></span>

* <span data-ttu-id="8ef6d-807">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="8ef6d-808">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="8ef6d-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="8ef6d-809">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="8ef6d-809">Backup</span></span>

* <span data-ttu-id="8ef6d-810">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="8ef6d-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="8ef6d-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-811">BatchAI</span></span>

* <span data-ttu-id="8ef6d-812">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="8ef6d-813">Cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-813">Cloud</span></span>

* <span data-ttu-id="8ef6d-814">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-815">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-815">Container</span></span>

* <span data-ttu-id="8ef6d-816">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="8ef6d-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="8ef6d-817">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="8ef6d-818">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="8ef6d-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-819">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-819">Extension</span></span>

* <span data-ttu-id="8ef6d-820">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-821">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-821">Network</span></span>

* <span data-ttu-id="8ef6d-822">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8ef6d-823">Rdbms</span></span>

* <span data-ttu-id="8ef6d-824">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-825">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-825">Resource</span></span>

* <span data-ttu-id="8ef6d-826">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-827">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-827">VM</span></span>

* <span data-ttu-id="8ef6d-828">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="8ef6d-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="8ef6d-829">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-829">June 25, 2018</span></span>

<span data-ttu-id="8ef6d-830">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="8ef6d-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="8ef6d-831">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-831">CLI</span></span>

* <span data-ttu-id="8ef6d-832">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="8ef6d-833">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-833">June 19, 2018</span></span>

<span data-ttu-id="8ef6d-834">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="8ef6d-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-835">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-835">Core</span></span>

* <span data-ttu-id="8ef6d-836">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-837">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-837">ACR</span></span>

* <span data-ttu-id="8ef6d-838">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="8ef6d-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="8ef6d-839">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-840">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-840">ACS</span></span>

* <span data-ttu-id="8ef6d-841">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="8ef6d-842">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-842">Added `--update` support</span></span>
* <span data-ttu-id="8ef6d-843">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="8ef6d-844">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="8ef6d-845">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="8ef6d-846">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="8ef6d-847">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="8ef6d-848">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-849">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-849">AppService</span></span>

* <span data-ttu-id="8ef6d-850">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="8ef6d-851">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-852">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-852">Batch</span></span>

* <span data-ttu-id="8ef6d-853">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8ef6d-854">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-854">Batch AI</span></span>

* <span data-ttu-id="8ef6d-855">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-855">Added support for workspaces.</span></span> <span data-ttu-id="8ef6d-856">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="8ef6d-857">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-857">Added support for experiments.</span></span> <span data-ttu-id="8ef6d-858">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="8ef6d-859">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="8ef6d-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="8ef6d-860">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="8ef6d-861">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="8ef6d-862">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="8ef6d-863">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="8ef6d-864">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="8ef6d-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="8ef6d-865">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="8ef6d-866">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="8ef6d-867">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="8ef6d-868">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="8ef6d-869">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="8ef6d-870">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="8ef6d-871">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="8ef6d-872">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="8ef6d-873">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="8ef6d-874">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="8ef6d-875">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="8ef6d-876">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="8ef6d-877">Cartes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-877">Maps</span></span>

* <span data-ttu-id="8ef6d-878">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-879">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-879">Network</span></span>

* <span data-ttu-id="8ef6d-880">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="8ef6d-881">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="8ef6d-882">#6502</span><span class="sxs-lookup"><span data-stu-id="8ef6d-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="8ef6d-883">Réservations</span><span class="sxs-lookup"><span data-stu-id="8ef6d-883">Reservations</span></span>

* <span data-ttu-id="8ef6d-884">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="8ef6d-885">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="8ef6d-886">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="8ef6d-887">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="8ef6d-888">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="8ef6d-889">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-890">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-890">Role</span></span>

* <span data-ttu-id="8ef6d-891">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-892">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-892">SQL</span></span>

* <span data-ttu-id="8ef6d-893">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-894">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-894">Storage</span></span>

* <span data-ttu-id="8ef6d-895">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-896">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-896">VM</span></span>

* <span data-ttu-id="8ef6d-897">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="8ef6d-898">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="8ef6d-899">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8ef6d-900">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-900">June 13, 2018</span></span>

<span data-ttu-id="8ef6d-901">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="8ef6d-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-902">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-902">Core</span></span>

* <span data-ttu-id="8ef6d-903">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8ef6d-904">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-904">June 13, 2018</span></span>

<span data-ttu-id="8ef6d-905">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="8ef6d-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="8ef6d-906">AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-906">AKS</span></span>

* <span data-ttu-id="8ef6d-907">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="8ef6d-908">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="8ef6d-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="8ef6d-909">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="8ef6d-910">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="8ef6d-911">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-912">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-912">AppService</span></span>

* <span data-ttu-id="8ef6d-913">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="8ef6d-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8ef6d-914">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-914">June 5, 2018</span></span>

<span data-ttu-id="8ef6d-915">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="8ef6d-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-916">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-916">Interactive</span></span>

* <span data-ttu-id="8ef6d-917">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8ef6d-918">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-918">June 5, 2018</span></span>

<span data-ttu-id="8ef6d-919">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="8ef6d-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-920">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-920">Core</span></span>

* <span data-ttu-id="8ef6d-921">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="8ef6d-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="8ef6d-922">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-923">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-923">ACR</span></span>

* <span data-ttu-id="8ef6d-924">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="8ef6d-925">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="8ef6d-926">AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-926">AKS</span></span>

* <span data-ttu-id="8ef6d-927">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-928">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-928">Batch</span></span>

* <span data-ttu-id="8ef6d-929">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-930">IOT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-930">IOT</span></span>

* <span data-ttu-id="8ef6d-931">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="8ef6d-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-932">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-932">Network</span></span>

* <span data-ttu-id="8ef6d-933">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="8ef6d-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="8ef6d-934">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="8ef6d-934">Policy Insights</span></span>

* <span data-ttu-id="8ef6d-935">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="8ef6d-936">ARM</span><span class="sxs-lookup"><span data-stu-id="8ef6d-936">ARM</span></span>

* <span data-ttu-id="8ef6d-937">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-938">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-938">SQL</span></span>

* <span data-ttu-id="8ef6d-939">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="8ef6d-940">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="8ef6d-941">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-941">Storage</span></span>

* <span data-ttu-id="8ef6d-942">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="8ef6d-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-943">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-943">VM</span></span>

* <span data-ttu-id="8ef6d-944">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="8ef6d-945">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="8ef6d-946">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="8ef6d-947">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-947">May 22, 2018</span></span>

<span data-ttu-id="8ef6d-948">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="8ef6d-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-949">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-949">Core</span></span>

* <span data-ttu-id="8ef6d-950">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="8ef6d-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-951">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-951">ACS</span></span>

* <span data-ttu-id="8ef6d-952">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="8ef6d-953">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-954">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-954">AppService</span></span>

* <span data-ttu-id="8ef6d-955">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-955">Improved generic update commands</span></span>
* <span data-ttu-id="8ef6d-956">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-957">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-957">Container</span></span>

* <span data-ttu-id="8ef6d-958">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="8ef6d-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="8ef6d-959">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-960">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-960">Extension</span></span>

* <span data-ttu-id="8ef6d-961">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-962">Interactive</span></span>

* <span data-ttu-id="8ef6d-963">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="8ef6d-964">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="8ef6d-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-965">KeyVault</span></span>

* <span data-ttu-id="8ef6d-966">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="8ef6d-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-967">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-967">Network</span></span>

* <span data-ttu-id="8ef6d-968">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="8ef6d-969">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-970">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-970">SQL</span></span>

* <span data-ttu-id="8ef6d-971">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="8ef6d-972">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="8ef6d-973">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="8ef6d-974">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="8ef6d-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="8ef6d-975">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="8ef6d-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="8ef6d-977">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="8ef6d-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-978">`edition`.</span></span> <span data-ttu-id="8ef6d-979">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="8ef6d-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-980">`elasticPoolName`.</span></span> <span data-ttu-id="8ef6d-981">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="8ef6d-982">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="8ef6d-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-983">`edition`.</span></span> <span data-ttu-id="8ef6d-984">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="8ef6d-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-985">`dtu`.</span></span> <span data-ttu-id="8ef6d-986">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="8ef6d-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-987">`databaseDtuMin`.</span></span> <span data-ttu-id="8ef6d-988">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="8ef6d-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-989">`databaseDtuMax`.</span></span> <span data-ttu-id="8ef6d-990">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="8ef6d-991">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="8ef6d-992">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-993">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-993">Storage</span></span>

* <span data-ttu-id="8ef6d-994">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="8ef6d-995">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-996">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-996">VM</span></span>

* <span data-ttu-id="8ef6d-997">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="8ef6d-998">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="8ef6d-999">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="8ef6d-1000">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="8ef6d-1001">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="8ef6d-1002">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1002">May 7, 2018</span></span>

<span data-ttu-id="8ef6d-1003">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1004">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1004">Core</span></span>

* <span data-ttu-id="8ef6d-1005">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="8ef6d-1006">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="8ef6d-1007">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="8ef6d-1008">#5591</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="8ef6d-1009">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="8ef6d-1010">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="8ef6d-1011">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="8ef6d-1012">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="8ef6d-1013">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1014">ACR</span></span>

* <span data-ttu-id="8ef6d-1015">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="8ef6d-1016">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="8ef6d-1017">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="8ef6d-1018">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="8ef6d-1019">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="8ef6d-1020">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1021">ACS</span></span>

* <span data-ttu-id="8ef6d-1022">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="8ef6d-1023">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="8ef6d-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1024">AMS</span></span>

* <span data-ttu-id="8ef6d-1025">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1026">Appservice</span></span>

* <span data-ttu-id="8ef6d-1027">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="8ef6d-1028">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="8ef6d-1029">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="8ef6d-1030">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8ef6d-1031">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1031">Batch AI</span></span>

* <span data-ttu-id="8ef6d-1032">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8ef6d-1033">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1033">Cognitive Services</span></span>

* <span data-ttu-id="8ef6d-1034">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-1035">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1035">Consumption</span></span>

* <span data-ttu-id="8ef6d-1036">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1037">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1037">Container</span></span>

* <span data-ttu-id="8ef6d-1038">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8ef6d-1039">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1039">Cosmos DB</span></span>

* <span data-ttu-id="8ef6d-1040">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="8ef6d-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1041">DMS</span></span>

* <span data-ttu-id="8ef6d-1042">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1043">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1043">Extension</span></span>

* <span data-ttu-id="8ef6d-1044">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1045">Interactive</span></span>

* <span data-ttu-id="8ef6d-1046">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="8ef6d-1047">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="8ef6d-1048">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="8ef6d-1049">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="8ef6d-1050">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1050">Lab</span></span>

* <span data-ttu-id="8ef6d-1051">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1052">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1052">Network</span></span>

* <span data-ttu-id="8ef6d-1053">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="8ef6d-1054">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1054">Profile</span></span>

* <span data-ttu-id="8ef6d-1055">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="8ef6d-1056">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="8ef6d-1057">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="8ef6d-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1058">Redis</span></span>

* <span data-ttu-id="8ef6d-1059">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="8ef6d-1060">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="8ef6d-1061">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="8ef6d-1062">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="8ef6d-1063">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1064">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1064">Role</span></span>

* <span data-ttu-id="8ef6d-1065">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1066">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1066">Storage</span></span>

* <span data-ttu-id="8ef6d-1067">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="8ef6d-1068">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="8ef6d-1069">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="8ef6d-1070">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="8ef6d-1071">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1072">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1072">VM</span></span>

* <span data-ttu-id="8ef6d-1073">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="8ef6d-1074">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="8ef6d-1075">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="8ef6d-1076">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="8ef6d-1077">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="8ef6d-1078">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1078">Added write accelerator support</span></span>
* <span data-ttu-id="8ef6d-1079">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="8ef6d-1080">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="8ef6d-1081">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="8ef6d-1082">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1082">April 10, 2018</span></span>

<span data-ttu-id="8ef6d-1083">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1084">ACR</span></span>

* <span data-ttu-id="8ef6d-1085">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1086">ACS</span></span>

* <span data-ttu-id="8ef6d-1087">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1088">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1088">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="8ef6d-1090">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="8ef6d-1091">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1091">BatchAI</span></span>

* <span data-ttu-id="8ef6d-1092">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="8ef6d-1093">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1093">Job level mounting</span></span>
  - <span data-ttu-id="8ef6d-1094">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="8ef6d-1095">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1095">Performance counters settings</span></span>
  - <span data-ttu-id="8ef6d-1096">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="8ef6d-1097">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="8ef6d-1098">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="8ef6d-1099">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="8ef6d-1100">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1100">Support for custom images</span></span>
  - <span data-ttu-id="8ef6d-1101">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="8ef6d-1102">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="8ef6d-1103">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="8ef6d-1104">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1104">National clouds are supported</span></span>
* <span data-ttu-id="8ef6d-1105">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="8ef6d-1106">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="8ef6d-1107">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="8ef6d-1108">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="8ef6d-1109">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="8ef6d-1110">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="8ef6d-1111">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="8ef6d-1112">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="8ef6d-1113">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="8ef6d-1114">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="8ef6d-1115">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="8ef6d-1116">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="8ef6d-1117">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="8ef6d-1118">Facturation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1118">Billing</span></span>

* <span data-ttu-id="8ef6d-1119">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-1120">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1120">Consumption</span></span>

* <span data-ttu-id="8ef6d-1121">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="8ef6d-1122">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="8ef6d-1123">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="8ef6d-1124">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="8ef6d-1125">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="8ef6d-1126">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1127">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1127">Container</span></span>

* <span data-ttu-id="8ef6d-1128">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="8ef6d-1129">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1130">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1130">Extension</span></span>

* <span data-ttu-id="8ef6d-1131">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1132">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1132">Interactive</span></span>

* <span data-ttu-id="8ef6d-1133">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="8ef6d-1134">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="8ef6d-1135">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1136">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1136">Network</span></span>

* <span data-ttu-id="8ef6d-1137">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="8ef6d-1138">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="8ef6d-1139">#4910</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1139">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="8ef6d-1140">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="8ef6d-1141">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="8ef6d-1142">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1143">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1144">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1145">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1145">Profile</span></span>

* <span data-ttu-id="8ef6d-1146">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="8ef6d-1147">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-1148">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1148">RDBMS</span></span>

* <span data-ttu-id="8ef6d-1149">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1149">Added `georestore` command</span></span>
* <span data-ttu-id="8ef6d-1150">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1151">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1151">Resource</span></span>

* <span data-ttu-id="8ef6d-1152">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="8ef6d-1153">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1154">SQL</span></span>

* <span data-ttu-id="8ef6d-1155">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1156">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1156">Storage</span></span>

* <span data-ttu-id="8ef6d-1157">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1158">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1158">VM</span></span>

* <span data-ttu-id="8ef6d-1159">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="8ef6d-1160">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="8ef6d-1162">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="8ef6d-1163">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="8ef6d-1164">#5718</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1164">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="8ef6d-1165">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="8ef6d-1166">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1166">March 27, 2018</span></span>

<span data-ttu-id="8ef6d-1167">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1168">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1168">Core</span></span>

* <span data-ttu-id="8ef6d-1169">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1170">ACS</span></span>

* <span data-ttu-id="8ef6d-1171">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1172">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1172">Appservice</span></span>

* <span data-ttu-id="8ef6d-1173">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="8ef6d-1174">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8ef6d-1175">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1175">Backup</span></span>

* <span data-ttu-id="8ef6d-1176">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="8ef6d-1177">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="8ef6d-1178">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="8ef6d-1179">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1180">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1180">Container</span></span>

* <span data-ttu-id="8ef6d-1181">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1181">Added `container exec` command.</span></span> <span data-ttu-id="8ef6d-1182">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="8ef6d-1183">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1184">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1184">Extension</span></span>

* <span data-ttu-id="8ef6d-1185">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="8ef6d-1186">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="8ef6d-1187">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1188">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1188">Interactive</span></span>

* <span data-ttu-id="8ef6d-1189">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="8ef6d-1190">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="8ef6d-1191">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="8ef6d-1192">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="8ef6d-1193">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1193">Lab</span></span>

* <span data-ttu-id="8ef6d-1194">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1195">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1195">Monitor</span></span>

* <span data-ttu-id="8ef6d-1196">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="8ef6d-1197">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="8ef6d-1198">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1199">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1199">Network</span></span>

* <span data-ttu-id="8ef6d-1200">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1201">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1201">Profile</span></span>

* <span data-ttu-id="8ef6d-1202">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-1203">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1203">RDBMS</span></span>

* <span data-ttu-id="8ef6d-1204">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1205">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1205">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="8ef6d-1207">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1207">Role</span></span>

* <span data-ttu-id="8ef6d-1208">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="8ef6d-1209">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="8ef6d-1210">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="8ef6d-1211">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="8ef6d-1212">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1213">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1213">Storage</span></span>

* <span data-ttu-id="8ef6d-1214">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="8ef6d-1215">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1216">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1216">VM</span></span>

* <span data-ttu-id="8ef6d-1217">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="8ef6d-1218">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="8ef6d-1219">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="8ef6d-1220">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="8ef6d-1221">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1221">March 13, 2018</span></span>

<span data-ttu-id="8ef6d-1222">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1223">ACR</span></span>

* <span data-ttu-id="8ef6d-1224">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="8ef6d-1225">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="8ef6d-1226">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1227">ACS</span></span>

* <span data-ttu-id="8ef6d-1228">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="8ef6d-1229">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="8ef6d-1230">Advisor</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1230">Advisor</span></span>

* <span data-ttu-id="8ef6d-1231">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="8ef6d-1232">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="8ef6d-1233">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="8ef6d-1234">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="8ef6d-1235">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1236">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1236">Appservice</span></span>

* <span data-ttu-id="8ef6d-1237">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="8ef6d-1238">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="8ef6d-1239">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1239">Eventhubs</span></span>

* <span data-ttu-id="8ef6d-1240">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1241">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1241">Extension</span></span>

* <span data-ttu-id="8ef6d-1242">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1243">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1243">Interactive</span></span>

* <span data-ttu-id="8ef6d-1244">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="8ef6d-1245">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="8ef6d-1246">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="8ef6d-1247">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1248">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1248">Monitor</span></span>

* <span data-ttu-id="8ef6d-1249">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="8ef6d-1250">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="8ef6d-1251">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="8ef6d-1252">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1253">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1253">Network</span></span>

* <span data-ttu-id="8ef6d-1254">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="8ef6d-1255">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="8ef6d-1256">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="8ef6d-1257">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1258">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1258">Profile</span></span>

* <span data-ttu-id="8ef6d-1259">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="8ef6d-1260">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-1261">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1261">RDBMS</span></span>

* <span data-ttu-id="8ef6d-1262">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="8ef6d-1263">Service Bus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1263">Service Bus</span></span>

* <span data-ttu-id="8ef6d-1264">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1265">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1265">Storage</span></span>

* <span data-ttu-id="8ef6d-1266">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="8ef6d-1267">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1268">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1268">VM</span></span>

* <span data-ttu-id="8ef6d-1269">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="8ef6d-1270">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="8ef6d-1271">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="8ef6d-1272">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="8ef6d-1273">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1273">February 27, 2018</span></span>

<span data-ttu-id="8ef6d-1274">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1275">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1275">Core</span></span>

* <span data-ttu-id="8ef6d-1276">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="8ef6d-1277">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="8ef6d-1278">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1279">ACS</span></span>

* <span data-ttu-id="8ef6d-1280">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="8ef6d-1281">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="8ef6d-1282">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="8ef6d-1283">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1284">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1284">Appservice</span></span>

* <span data-ttu-id="8ef6d-1285">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="8ef6d-1286">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8ef6d-1287">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1287">Cognitive Services</span></span>

* <span data-ttu-id="8ef6d-1288">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-1289">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1289">Consumption</span></span>

* <span data-ttu-id="8ef6d-1290">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="8ef6d-1291">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1292">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1292">Container</span></span>

* <span data-ttu-id="8ef6d-1293">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1294">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1294">Network</span></span>

* <span data-ttu-id="8ef6d-1295">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1296">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1296">Resource</span></span>

* <span data-ttu-id="8ef6d-1297">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1298">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1298">Role</span></span>

* <span data-ttu-id="8ef6d-1299">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1300">SQL</span></span>

* <span data-ttu-id="8ef6d-1301">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1302">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1302">Storage</span></span>

* <span data-ttu-id="8ef6d-1303">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1304">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1304">VM</span></span>

* <span data-ttu-id="8ef6d-1305">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="8ef6d-1306">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1306">February 13, 2018</span></span>

<span data-ttu-id="8ef6d-1307">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1308">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1308">Core</span></span>

* <span data-ttu-id="8ef6d-1309">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1310">ACS</span></span>

* <span data-ttu-id="8ef6d-1311">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="8ef6d-1312">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="8ef6d-1313">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="8ef6d-1314">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="8ef6d-1315">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="8ef6d-1316">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="8ef6d-1317">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="8ef6d-1318">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1319">Appservice</span></span>

* <span data-ttu-id="8ef6d-1320">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="8ef6d-1321">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="8ef6d-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1322">CDN</span></span>

* <span data-ttu-id="8ef6d-1323">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1324">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1324">Container</span></span>

* <span data-ttu-id="8ef6d-1325">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="8ef6d-1326">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-1327">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1327">CosmosDB</span></span>

* <span data-ttu-id="8ef6d-1328">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1329">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1329">Extension</span></span>

* <span data-ttu-id="8ef6d-1330">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="8ef6d-1331">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="8ef6d-1332">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1332">Feedback</span></span>

* <span data-ttu-id="8ef6d-1333">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1334">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1334">Interactive</span></span>

* <span data-ttu-id="8ef6d-1335">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="8ef6d-1336">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-1337">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1337">IoT</span></span>

* <span data-ttu-id="8ef6d-1338">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8ef6d-1339">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8ef6d-1340">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1341">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1342">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1342">Monitor</span></span>

* <span data-ttu-id="8ef6d-1343">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1344">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1344">Network</span></span>

* <span data-ttu-id="8ef6d-1345">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="8ef6d-1346">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1346">Profile</span></span>

* <span data-ttu-id="8ef6d-1347">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1348">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1348">Resource</span></span>

* <span data-ttu-id="8ef6d-1349">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1350">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1350">Role</span></span>

* <span data-ttu-id="8ef6d-1351">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1352">SQL</span></span>

* <span data-ttu-id="8ef6d-1353">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="8ef6d-1354">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="8ef6d-1355">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1356">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1356">Storage</span></span>

* <span data-ttu-id="8ef6d-1357">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1358">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1358">VM</span></span>

* <span data-ttu-id="8ef6d-1359">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="8ef6d-1360">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="8ef6d-1361">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="8ef6d-1362">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1362">January 31, 2018</span></span>

<span data-ttu-id="8ef6d-1363">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1364">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1364">Core</span></span>

* <span data-ttu-id="8ef6d-1365">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="8ef6d-1366">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="8ef6d-1367">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="8ef6d-1368">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="8ef6d-1369">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1370">ACS</span></span>

* <span data-ttu-id="8ef6d-1371">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="8ef6d-1372">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1373">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1373">Appservice</span></span>

* <span data-ttu-id="8ef6d-1374">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="8ef6d-1375">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="8ef6d-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1376">CDN</span></span>

* <span data-ttu-id="8ef6d-1377">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-1378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1378">CosmosDB</span></span>

* <span data-ttu-id="8ef6d-1379">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1380">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1380">Interactive</span></span>

* <span data-ttu-id="8ef6d-1381">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1382">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1382">Network</span></span>

* <span data-ttu-id="8ef6d-1383">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="8ef6d-1384">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="8ef6d-1385">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="8ef6d-1386">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="8ef6d-1387">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="8ef6d-1388">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="8ef6d-1389">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="8ef6d-1390">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="8ef6d-1391">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="8ef6d-1392">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1393">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1393">Profile</span></span>

* <span data-ttu-id="8ef6d-1394">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1395">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1395">Resource</span></span>

* <span data-ttu-id="8ef6d-1396">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1397">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1397">Storage</span></span>

* <span data-ttu-id="8ef6d-1398">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="8ef6d-1399">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="8ef6d-1400">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="8ef6d-1401">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="8ef6d-1402">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1403">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1403">VM</span></span>

* <span data-ttu-id="8ef6d-1404">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="8ef6d-1405">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="8ef6d-1406">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="8ef6d-1407">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="8ef6d-1408">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1408">January 17, 2018</span></span>

<span data-ttu-id="8ef6d-1409">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1410">ACR</span></span>

* <span data-ttu-id="8ef6d-1411">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="8ef6d-1412">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1413">ACS</span></span>

* <span data-ttu-id="8ef6d-1414">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="8ef6d-1415">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1416">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1416">Appservice</span></span>

* <span data-ttu-id="8ef6d-1417">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="8ef6d-1418">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="8ef6d-1419">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="8ef6d-1420">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1420">Backup</span></span>

* <span data-ttu-id="8ef6d-1421">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="8ef6d-1422">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="8ef6d-1423">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="8ef6d-1424">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="8ef6d-1425">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-1426">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1426">Batch</span></span>

* <span data-ttu-id="8ef6d-1427">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="8ef6d-1428">Cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1428">Cloud</span></span>

* <span data-ttu-id="8ef6d-1429">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-1430">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1430">Consumption</span></span>

* <span data-ttu-id="8ef6d-1431">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="8ef6d-1432">Event Grid</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1432">Event Grid</span></span>

* <span data-ttu-id="8ef6d-1433">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8ef6d-1434">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8ef6d-1435">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="8ef6d-1436">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="8ef6d-1437">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="8ef6d-1438">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="8ef6d-1439">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="8ef6d-1440">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1441">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1441">Interactive</span></span>

* <span data-ttu-id="8ef6d-1442">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="8ef6d-1443">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="8ef6d-1444">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-1445">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1445">IoT</span></span>

* <span data-ttu-id="8ef6d-1446">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="8ef6d-1447">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="8ef6d-1448">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1449">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1449">Monitor</span></span>

* <span data-ttu-id="8ef6d-1450">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="8ef6d-1451">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="8ef6d-1452">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1453">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1453">Network</span></span>

* <span data-ttu-id="8ef6d-1454">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="8ef6d-1455">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1456">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1456">Profile</span></span>

* <span data-ttu-id="8ef6d-1457">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1458">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1458">Role</span></span>

* <span data-ttu-id="8ef6d-1459">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8ef6d-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1460">Service Fabric</span></span>

* <span data-ttu-id="8ef6d-1461">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="8ef6d-1462">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1463">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1463">VM</span></span>

* <span data-ttu-id="8ef6d-1464">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="8ef6d-1465">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="8ef6d-1466">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="8ef6d-1467">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="8ef6d-1468">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="8ef6d-1469">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8ef6d-1470">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="8ef6d-1471">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="8ef6d-1472">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1472">December 19, 2017</span></span>

<span data-ttu-id="8ef6d-1473">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1473">Version 2.0.23</span></span>

* <span data-ttu-id="8ef6d-1474">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1475">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1475">Container</span></span>

* <span data-ttu-id="8ef6d-1476">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1477">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1477">Network</span></span>

* <span data-ttu-id="8ef6d-1478">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1479">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1480">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1480">Storage</span></span>

* <span data-ttu-id="8ef6d-1481">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1482">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1482">VM</span></span>

* <span data-ttu-id="8ef6d-1483">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="8ef6d-1484">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1484">December 5, 2017</span></span>

<span data-ttu-id="8ef6d-1485">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1485">Version 2.0.22</span></span>

* <span data-ttu-id="8ef6d-1486">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1486">Removed `az component` commands.</span></span> <span data-ttu-id="8ef6d-1487">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1488">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1488">Core</span></span>
* <span data-ttu-id="8ef6d-1489">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="8ef6d-1490">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1491">ACS</span></span>

* <span data-ttu-id="8ef6d-1492">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="8ef6d-1493">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="8ef6d-1494">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="8ef6d-1495">Advisor</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1495">Advisor</span></span>

* <span data-ttu-id="8ef6d-1496">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1497">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1497">Appservice</span></span>

* <span data-ttu-id="8ef6d-1498">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="8ef6d-1499">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="8ef6d-1500">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="8ef6d-1501">Consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1501">Consumption</span></span>

* <span data-ttu-id="8ef6d-1502">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1503">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1503">Container</span></span>

* <span data-ttu-id="8ef6d-1504">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1505">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1505">Monitor</span></span>

* <span data-ttu-id="8ef6d-1506">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1507">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1507">Resource</span></span>

* <span data-ttu-id="8ef6d-1508">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1509">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1509">Role</span></span>

* <span data-ttu-id="8ef6d-1510">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="8ef6d-1511">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="8ef6d-1512">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1513">SQL</span></span>

* <span data-ttu-id="8ef6d-1514">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="8ef6d-1515">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1516">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1516">VM</span></span>

* <span data-ttu-id="8ef6d-1517">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="8ef6d-1518">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1518">November 14, 2017</span></span>

<span data-ttu-id="8ef6d-1519">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1520">ACR</span></span>

* <span data-ttu-id="8ef6d-1521">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="8ef6d-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1522">ACS</span></span>

* <span data-ttu-id="8ef6d-1523">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="8ef6d-1524">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="8ef6d-1525">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="8ef6d-1526">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="8ef6d-1527">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1528">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1528">Appservice</span></span>

* <span data-ttu-id="8ef6d-1529">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="8ef6d-1530">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="8ef6d-1531">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="8ef6d-1532">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="8ef6d-1533">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="8ef6d-1534">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-1535">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1535">Batch</span></span>

* <span data-ttu-id="8ef6d-1536">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="8ef6d-1537">Batchai</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1537">Batchai</span></span>

* <span data-ttu-id="8ef6d-1538">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="8ef6d-1539">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="8ef6d-1540">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="8ef6d-1541">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="8ef6d-1542">Cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1542">Cloud</span></span>

* <span data-ttu-id="8ef6d-1543">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1544">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1544">Container</span></span>

* <span data-ttu-id="8ef6d-1545">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="8ef6d-1546">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1546">Added container group restart policy</span></span>
* <span data-ttu-id="8ef6d-1547">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="8ef6d-1548">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8ef6d-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="8ef6d-1550">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8ef6d-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1551">Data Lake Store</span></span>

* <span data-ttu-id="8ef6d-1552">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1553">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1553">Extension</span></span>

* <span data-ttu-id="8ef6d-1554">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="8ef6d-1555">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-1556">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1556">IoT</span></span>

* <span data-ttu-id="8ef6d-1557">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1558">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1558">Monitor</span></span>

* <span data-ttu-id="8ef6d-1559">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1560">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1560">Network</span></span>

* <span data-ttu-id="8ef6d-1561">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="8ef6d-1562">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="8ef6d-1563">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="8ef6d-1564">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="8ef6d-1565">Réservations</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1565">Reservations</span></span>

* <span data-ttu-id="8ef6d-1566">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1567">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1567">Resource</span></span>

* <span data-ttu-id="8ef6d-1568">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1569">SQL</span></span>

* <span data-ttu-id="8ef6d-1570">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1571">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1571">Storage</span></span>

* <span data-ttu-id="8ef6d-1572">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="8ef6d-1573">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="8ef6d-1574">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="8ef6d-1575">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="8ef6d-1576">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="8ef6d-1577">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="8ef6d-1578">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1579">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1579">VM</span></span>

* <span data-ttu-id="8ef6d-1580">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="8ef6d-1581">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="8ef6d-1582">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="8ef6d-1583">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="8ef6d-1584">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="8ef6d-1585">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1585">October 24, 2017</span></span>

<span data-ttu-id="8ef6d-1586">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1587">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1587">Core</span></span>

* <span data-ttu-id="8ef6d-1588">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1589">ACR</span></span>

* <span data-ttu-id="8ef6d-1590">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="8ef6d-1591">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="8ef6d-1592">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1593">ACS</span></span>

* <span data-ttu-id="8ef6d-1594">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="8ef6d-1595">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1596">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1596">Appservice</span></span>

* <span data-ttu-id="8ef6d-1597">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="8ef6d-1598">Composant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1598">Component</span></span>

* <span data-ttu-id="8ef6d-1599">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1600">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1600">Monitor</span></span>

* <span data-ttu-id="8ef6d-1601">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1602">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1602">Resource</span></span>

* <span data-ttu-id="8ef6d-1603">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="8ef6d-1604">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1605">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1605">VM</span></span>

* <span data-ttu-id="8ef6d-1606">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="8ef6d-1607">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1607">October 9, 2017</span></span>

<span data-ttu-id="8ef6d-1608">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1609">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1609">Core</span></span>

* <span data-ttu-id="8ef6d-1610">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1611">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1611">Appservice</span></span>

* <span data-ttu-id="8ef6d-1612">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1613">Batch</span></span>

* <span data-ttu-id="8ef6d-1614">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="8ef6d-1615">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="8ef6d-1616">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="8ef6d-1617">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="8ef6d-1618">Batchai</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1618">Batchai</span></span>

* <span data-ttu-id="8ef6d-1619">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-1620">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1620">Keyvault</span></span>

* <span data-ttu-id="8ef6d-1621">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="8ef6d-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="8ef6d-1623">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1623">Network</span></span>

* <span data-ttu-id="8ef6d-1624">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="8ef6d-1625">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1626">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1626">Resource</span></span>

* <span data-ttu-id="8ef6d-1627">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="8ef6d-1628">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="8ef6d-1629">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="8ef6d-1630">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1631">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1631">Sql</span></span>

* <span data-ttu-id="8ef6d-1632">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="8ef6d-1633">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="8ef6d-1634">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1635">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1635">Storage</span></span>

* <span data-ttu-id="8ef6d-1636">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1637">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1637">Vm</span></span>

* <span data-ttu-id="8ef6d-1638">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="8ef6d-1639">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="8ef6d-1640">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="8ef6d-1641">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="8ef6d-1642">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="8ef6d-1643">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1643">September 22, 2017</span></span>

<span data-ttu-id="8ef6d-1644">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1645">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1645">Resource</span></span>

* <span data-ttu-id="8ef6d-1646">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="8ef6d-1647">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="8ef6d-1648">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="8ef6d-1649">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1650">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1650">Network</span></span>

* <span data-ttu-id="8ef6d-1651">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="8ef6d-1652">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="8ef6d-1653">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="8ef6d-1654">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="8ef6d-1655">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1656">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1657">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1658">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1658">Storage</span></span>

* <span data-ttu-id="8ef6d-1659">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8ef6d-1660">Événement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1660">Eventgrid</span></span>

* <span data-ttu-id="8ef6d-1661">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1662">SQL</span></span>

* <span data-ttu-id="8ef6d-1663">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="8ef6d-1664">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="8ef6d-1665">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-1666">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1666">Keyvault</span></span>

* <span data-ttu-id="8ef6d-1667">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1668">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1668">VM</span></span>

* <span data-ttu-id="8ef6d-1669">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="8ef6d-1670">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="8ef6d-1671">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="8ef6d-1672">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="8ef6d-1673">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="8ef6d-1674">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1675">ACS</span></span>

* <span data-ttu-id="8ef6d-1676">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1677">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1677">Appservice</span></span>

* <span data-ttu-id="8ef6d-1678">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8ef6d-1679">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1679">Backup</span></span>

* <span data-ttu-id="8ef6d-1680">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="8ef6d-1681">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1681">September 11, 2017</span></span>

<span data-ttu-id="8ef6d-1682">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="8ef6d-1683">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1683">Core</span></span>

* <span data-ttu-id="8ef6d-1684">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="8ef6d-1685">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1686">Acs</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1686">Acs</span></span>

* <span data-ttu-id="8ef6d-1687">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="8ef6d-1688">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1689">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1689">Appservice</span></span>

* <span data-ttu-id="8ef6d-1690">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="8ef6d-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1691">CDN</span></span>

* <span data-ttu-id="8ef6d-1692">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="8ef6d-1693">Extension</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1693">Extension</span></span>

* <span data-ttu-id="8ef6d-1694">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-1695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1695">Keyvault</span></span>

* <span data-ttu-id="8ef6d-1696">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1697">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1697">Network</span></span>

* <span data-ttu-id="8ef6d-1698">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8ef6d-1699">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="8ef6d-1700">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="8ef6d-1701">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8ef6d-1702">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1703">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1703">Resource</span></span>

* <span data-ttu-id="8ef6d-1704">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="8ef6d-1705">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="8ef6d-1706">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="8ef6d-1707">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1708">SQL</span></span>

* <span data-ttu-id="8ef6d-1709">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1710">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1710">VM</span></span>

* <span data-ttu-id="8ef6d-1711">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="8ef6d-1712">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="8ef6d-1713">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="8ef6d-1714">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="8ef6d-1715">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="8ef6d-1716">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1716">August 31, 2017</span></span>

<span data-ttu-id="8ef6d-1717">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-1718">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1718">Keyvault</span></span>

* <span data-ttu-id="8ef6d-1719">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="8ef6d-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1720">Sf</span></span>

* <span data-ttu-id="8ef6d-1721">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1722">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1722">Storage</span></span>

* <span data-ttu-id="8ef6d-1723">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="8ef6d-1724">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="8ef6d-1725">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1725">August 28, 2017</span></span>

<span data-ttu-id="8ef6d-1726">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="8ef6d-1727">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1727">CLI</span></span>

* <span data-ttu-id="8ef6d-1728">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1729">ACS</span></span>

* <span data-ttu-id="8ef6d-1730">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1730">Corrected preview regions</span></span>
* <span data-ttu-id="8ef6d-1731">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="8ef6d-1732">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1733">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1733">Appservice</span></span>

* <span data-ttu-id="8ef6d-1734">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="8ef6d-1735">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="8ef6d-1736">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="8ef6d-1737">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="8ef6d-1738">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-1739">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1739">IoT</span></span>

* <span data-ttu-id="8ef6d-1740">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1741">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1741">Network</span></span>

* <span data-ttu-id="8ef6d-1742">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8ef6d-1743">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1744">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8ef6d-1745">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8ef6d-1746">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1747">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1747">Profile</span></span>

* <span data-ttu-id="8ef6d-1748">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8ef6d-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1749">Service Fabric</span></span>

* <span data-ttu-id="8ef6d-1750">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1750">Preview release</span></span>
* <span data-ttu-id="8ef6d-1751">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="8ef6d-1752">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="8ef6d-1753">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1754">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1754">Storage</span></span>

* <span data-ttu-id="8ef6d-1755">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="8ef6d-1756">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="8ef6d-1757">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="8ef6d-1758">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="8ef6d-1759">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="8ef6d-1760">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1761">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1761">VM</span></span>

* <span data-ttu-id="8ef6d-1762">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="8ef6d-1763">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="8ef6d-1764">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="8ef6d-1765">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="8ef6d-1766">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="8ef6d-1767">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="8ef6d-1768">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1768">August 15, 2017</span></span>

<span data-ttu-id="8ef6d-1769">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1770">ACS</span></span>

* <span data-ttu-id="8ef6d-1771">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1772">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1772">Appservice</span></span>

* <span data-ttu-id="8ef6d-1773">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="8ef6d-1774">Event Grid</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1774">Event Grid</span></span>

* <span data-ttu-id="8ef6d-1775">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="8ef6d-1776">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1776">August 11, 2017</span></span>

<span data-ttu-id="8ef6d-1777">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1778">ACS</span></span>

* <span data-ttu-id="8ef6d-1779">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-1780">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1780">Batch</span></span>

* <span data-ttu-id="8ef6d-1781">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="8ef6d-1782">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="8ef6d-1783">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="8ef6d-1784">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="8ef6d-1785">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="8ef6d-1786">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="8ef6d-1787">Composant</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1787">Component</span></span>

* <span data-ttu-id="8ef6d-1788">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="8ef6d-1789">Conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1789">Container</span></span>

* <span data-ttu-id="8ef6d-1790">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="8ef6d-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1791">Data Lake Store</span></span>

* <span data-ttu-id="8ef6d-1792">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="8ef6d-1793">Event Grid</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1793">Event Grid</span></span>

* <span data-ttu-id="8ef6d-1794">Version initiale</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1795">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1795">Network</span></span>

* <span data-ttu-id="8ef6d-1796">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="8ef6d-1797">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="8ef6d-1798">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="8ef6d-1799">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1800">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1800">Profile</span></span>

* <span data-ttu-id="8ef6d-1801">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1802">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1802">Storage</span></span>

* <span data-ttu-id="8ef6d-1803">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1804">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1804">VM</span></span>

* <span data-ttu-id="8ef6d-1805">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="8ef6d-1806">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="8ef6d-1807">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="8ef6d-1808">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="8ef6d-1809">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="8ef6d-1810">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1810">July 28, 2017</span></span>

<span data-ttu-id="8ef6d-1811">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1811">Version 2.0.12</span></span>

* <span data-ttu-id="8ef6d-1812">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1812">Added container commands</span></span>
* <span data-ttu-id="8ef6d-1813">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="8ef6d-1814">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1814">Core</span></span>

* <span data-ttu-id="8ef6d-1815">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="8ef6d-1816">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="8ef6d-1817">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="8ef6d-1818">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="8ef6d-1819">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="8ef6d-1820">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="8ef6d-1821">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8ef6d-1822">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="8ef6d-1823">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="8ef6d-1824">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="8ef6d-1825">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="8ef6d-1826">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="8ef6d-1827">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="8ef6d-1828">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="8ef6d-1829">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="8ef6d-1830">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="8ef6d-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1831">ACR</span></span>

* <span data-ttu-id="8ef6d-1832">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="8ef6d-1833">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="8ef6d-1834">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="8ef6d-1835">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="8ef6d-1836">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="8ef6d-1837">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1838">ACS</span></span>

* <span data-ttu-id="8ef6d-1839">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-1840">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1840">Appservice</span></span>

* <span data-ttu-id="8ef6d-1841">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="8ef6d-1842">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="8ef6d-1843">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="8ef6d-1844">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="8ef6d-1845">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="8ef6d-1846">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="8ef6d-1847">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="8ef6d-1848">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="8ef6d-1849">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="8ef6d-1850">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="8ef6d-1851">Batch</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1851">Batch</span></span>

* <span data-ttu-id="8ef6d-1852">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="8ef6d-1853">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="8ef6d-1854">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="8ef6d-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1855">CDN</span></span>

* <span data-ttu-id="8ef6d-1856">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="8ef6d-1857">Cloud</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1857">Cloud</span></span>

* <span data-ttu-id="8ef6d-1858">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="8ef6d-1859">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="8ef6d-1860">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="8ef6d-1861">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="8ef6d-1862">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-1863">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1863">CosmosDB</span></span>

* <span data-ttu-id="8ef6d-1864">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="8ef6d-1865">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8ef6d-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="8ef6d-1867">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="8ef6d-1868">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="8ef6d-1869">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8ef6d-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1870">Data Lake Store</span></span>

* <span data-ttu-id="8ef6d-1871">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="8ef6d-1872">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="8ef6d-1873">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="8ef6d-1874">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="8ef6d-1875">Interactive</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1875">Interactive</span></span>

* <span data-ttu-id="8ef6d-1876">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="8ef6d-1877">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1877">Increased test coverage</span></span>
* <span data-ttu-id="8ef6d-1878">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="8ef6d-1879">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="8ef6d-1880">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="8ef6d-1881">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="8ef6d-1882">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8ef6d-1883">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="8ef6d-1884">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="8ef6d-1885">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="8ef6d-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1886">IoT</span></span>

* <span data-ttu-id="8ef6d-1887">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="8ef6d-1888">(#3934)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="8ef6d-1889">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1889">Key vault</span></span>

* <span data-ttu-id="8ef6d-1890">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="8ef6d-1891">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="8ef6d-1892">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8ef6d-1893">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8ef6d-1894">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="8ef6d-1895">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="8ef6d-1896">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="8ef6d-1897">(#3307)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="8ef6d-1898">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1898">Lab</span></span>

* <span data-ttu-id="8ef6d-1899">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="8ef6d-1900">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-1901">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1901">Monitor</span></span>

* <span data-ttu-id="8ef6d-1902">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="8ef6d-1903">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="8ef6d-1904">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="8ef6d-1905">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="8ef6d-1906">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="8ef6d-1907">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="8ef6d-1908">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="8ef6d-1909">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="8ef6d-1910">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1910">`location` no longer required</span></span>
  * <span data-ttu-id="8ef6d-1911">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="8ef6d-1912">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="8ef6d-1913">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="8ef6d-1914">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="8ef6d-1915">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="8ef6d-1916">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="8ef6d-1917">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-1918">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1918">Network</span></span>

* <span data-ttu-id="8ef6d-1919">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="8ef6d-1920">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="8ef6d-1921">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="8ef6d-1922">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="8ef6d-1923">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="8ef6d-1924">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="8ef6d-1925">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="8ef6d-1926">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="8ef6d-1927">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="8ef6d-1928">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="8ef6d-1929">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="8ef6d-1930">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="8ef6d-1931">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="8ef6d-1932">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="8ef6d-1933">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="8ef6d-1934">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="8ef6d-1935">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="8ef6d-1936">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="8ef6d-1937">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="8ef6d-1938">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="8ef6d-1939">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="8ef6d-1940">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="8ef6d-1941">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="8ef6d-1942">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="8ef6d-1943">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="8ef6d-1944">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="8ef6d-1945">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-1946">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1946">Profile</span></span>

* <span data-ttu-id="8ef6d-1947">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="8ef6d-1948">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="8ef6d-1949">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="8ef6d-1950">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="8ef6d-1951">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="8ef6d-1952">SGBDR</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1952">RDBMS</span></span>

* <span data-ttu-id="8ef6d-1953">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="8ef6d-1954">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="8ef6d-1955">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="8ef6d-1956">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-1957">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1957">Resource</span></span>

* <span data-ttu-id="8ef6d-1958">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="8ef6d-1959">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="8ef6d-1960">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="8ef6d-1961">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="8ef6d-1962">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="8ef6d-1963">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="8ef6d-1964">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="8ef6d-1965">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-1966">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1966">Role</span></span>

* <span data-ttu-id="8ef6d-1967">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="8ef6d-1968">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="8ef6d-1969">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="8ef6d-1970">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="8ef6d-1971">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8ef6d-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1972">Service Fabric</span></span>
* <span data-ttu-id="8ef6d-1973">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="8ef6d-1974">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="8ef6d-1975">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1976">SQL</span></span>

* <span data-ttu-id="8ef6d-1977">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="8ef6d-1978">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="8ef6d-1979">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-1980">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1980">Storage</span></span>

* <span data-ttu-id="8ef6d-1981">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="8ef6d-1982">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="8ef6d-1983">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="8ef6d-1984">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="8ef6d-1985">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="8ef6d-1986">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-1987">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1987">VM</span></span>

* <span data-ttu-id="8ef6d-1988">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1988">Support configuring nsg</span></span>
* <span data-ttu-id="8ef6d-1989">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="8ef6d-1990">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1990">Support managed service identities</span></span>
* <span data-ttu-id="8ef6d-1991">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="8ef6d-1992">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="8ef6d-1993">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1993">May 10, 2017</span></span>

<span data-ttu-id="8ef6d-1994">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1994">Version 2.0.6</span></span>

* <span data-ttu-id="8ef6d-1995">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="8ef6d-1996">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="8ef6d-1997">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="8ef6d-1998">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="8ef6d-1999">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8ef6d-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="8ef6d-2000">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="8ef6d-2001">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="8ef6d-2002">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2002">Remove Container module</span></span>
* <span data-ttu-id="8ef6d-2003">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="8ef6d-2004">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="8ef6d-2005">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2005">Core</span></span>

* <span data-ttu-id="8ef6d-2006">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="8ef6d-2007">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="8ef6d-2008">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="8ef6d-2009">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="8ef6d-2010">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="8ef6d-2011">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="8ef6d-2012">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="8ef6d-2013">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="8ef6d-2014">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="8ef6d-2015">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2015">core: Improved performance</span></span>
* <span data-ttu-id="8ef6d-2016">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="8ef6d-2017">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2018">ACS</span></span>

* <span data-ttu-id="8ef6d-2019">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="8ef6d-2020">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="8ef6d-2021">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="8ef6d-2022">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2023">AppService</span></span>

* <span data-ttu-id="8ef6d-2024">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="8ef6d-2025">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="8ef6d-2026">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="8ef6d-2027">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="8ef6d-2028">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="8ef6d-2029">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="8ef6d-2030">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2030">support slot swap with preview</span></span>
* <span data-ttu-id="8ef6d-2031">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="8ef6d-2032">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8ef6d-2033">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2033">CosmosDB</span></span>

* <span data-ttu-id="8ef6d-2034">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="8ef6d-2035">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="8ef6d-2036">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="8ef6d-2037">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8ef6d-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="8ef6d-2039">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="8ef6d-2040">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="8ef6d-2041">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="8ef6d-2042">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="8ef6d-2043">Table</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2043">Table</span></span>
  * <span data-ttu-id="8ef6d-2044">Fonction table</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2044">Table valued function</span></span>
  * <span data-ttu-id="8ef6d-2045">Affichage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2045">View</span></span>
  * <span data-ttu-id="8ef6d-2046">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2046">Table Statistics.</span></span> <span data-ttu-id="8ef6d-2047">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8ef6d-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2048">Data Lake Store</span></span>

* <span data-ttu-id="8ef6d-2049">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="8ef6d-2050">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="8ef6d-2051">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2051">missed help for access show.</span></span> <span data-ttu-id="8ef6d-2052">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2052">adding it.</span></span> <span data-ttu-id="8ef6d-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="8ef6d-2054">Rechercher</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2054">Find</span></span>

* <span data-ttu-id="8ef6d-2055">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ef6d-2056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2056">KeyVault</span></span>

* <span data-ttu-id="8ef6d-2057">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="8ef6d-2058">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="8ef6d-2059">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="8ef6d-2060">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="8ef6d-2061">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="8ef6d-2062">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2062">Lab</span></span>

* <span data-ttu-id="8ef6d-2063">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="8ef6d-2064">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="8ef6d-2065">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="8ef6d-2066">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="8ef6d-2067">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="8ef6d-2068">Surveiller</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2068">Monitor</span></span>

* <span data-ttu-id="8ef6d-2069">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="8ef6d-2070">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="8ef6d-2071">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2071">Network</span></span>

* <span data-ttu-id="8ef6d-2072">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="8ef6d-2073">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="8ef6d-2074">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="8ef6d-2075">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="8ef6d-2076">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="8ef6d-2077">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="8ef6d-2078">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="8ef6d-2079">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="8ef6d-2080">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="8ef6d-2081">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="8ef6d-2082">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="8ef6d-2083">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="8ef6d-2084">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="8ef6d-2085">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="8ef6d-2086">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="8ef6d-2087">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="8ef6d-2088">Profil</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2088">Profile</span></span>

* <span data-ttu-id="8ef6d-2089">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="8ef6d-2090">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="8ef6d-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2091">Redis</span></span>

* <span data-ttu-id="8ef6d-2092">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="8ef6d-2093">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="8ef6d-2094">Ressource</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2094">Resource</span></span>

* <span data-ttu-id="8ef6d-2095">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="8ef6d-2096">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="8ef6d-2097">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="8ef6d-2098">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="8ef6d-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="8ef6d-2100">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2100">Add docs for az lock update.</span></span> <span data-ttu-id="8ef6d-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="8ef6d-2102">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="8ef6d-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="8ef6d-2104">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="8ef6d-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="8ef6d-2106">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="8ef6d-2107">Rôle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2107">Role</span></span>

* <span data-ttu-id="8ef6d-2108">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="8ef6d-2109">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="8ef6d-2110">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="8ef6d-2111">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="8ef6d-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2112">SQL</span></span>

* <span data-ttu-id="8ef6d-2113">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="8ef6d-2114">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="8ef6d-2115">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2115">Storage</span></span>

* <span data-ttu-id="8ef6d-2116">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="8ef6d-2117">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="8ef6d-2118">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="8ef6d-2119">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-2120">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2120">VM</span></span>

* <span data-ttu-id="8ef6d-2121">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="8ef6d-2122">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="8ef6d-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="8ef6d-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="8ef6d-2125">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="8ef6d-2126">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="8ef6d-2127">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="8ef6d-2128">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2128">April 3, 2017</span></span>

<span data-ttu-id="8ef6d-2129">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2129">Version 2.0.2</span></span>

<span data-ttu-id="8ef6d-2130">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="8ef6d-2131">Principal</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2131">Core</span></span>

* <span data-ttu-id="8ef6d-2132">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="8ef6d-2133">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="8ef6d-2134">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="8ef6d-2135">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8ef6d-2136">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="8ef6d-2137">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="8ef6d-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="8ef6d-2139">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="8ef6d-2140">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="8ef6d-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2141">ACS</span></span>

* <span data-ttu-id="8ef6d-2142">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="8ef6d-2143">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="8ef6d-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="8ef6d-2145">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2145">Add support for windows clusters.</span></span> <span data-ttu-id="8ef6d-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="8ef6d-2147">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="8ef6d-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="8ef6d-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2149">AppService</span></span>

* <span data-ttu-id="8ef6d-2150">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="8ef6d-2151">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="8ef6d-2152">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="8ef6d-2153">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="8ef6d-2154">DataLake</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2154">DataLake</span></span>

* <span data-ttu-id="8ef6d-2155">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="8ef6d-2156">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="8ef6d-2157">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2157">DocuemntDB</span></span>

* <span data-ttu-id="8ef6d-2158">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="8ef6d-2159">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2159">VM</span></span>

* <span data-ttu-id="8ef6d-2160">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="8ef6d-2161">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="8ef6d-2162">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="8ef6d-2163">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8ef6d-2164">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="8ef6d-2165">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="8ef6d-2166">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="8ef6d-2167">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2167">February 27, 2017</span></span>

<span data-ttu-id="8ef6d-2168">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2168">Version 2.0.0</span></span>

<span data-ttu-id="8ef6d-2169">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="8ef6d-2170">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2170">Container Service (acs)</span></span>
- <span data-ttu-id="8ef6d-2171">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="8ef6d-2172">Réseau</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2172">Networking</span></span>
- <span data-ttu-id="8ef6d-2173">Stockage</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2173">Storage</span></span>

<span data-ttu-id="8ef6d-2174">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="8ef6d-2175">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="8ef6d-2176">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="8ef6d-2177">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="8ef6d-2178">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="8ef6d-2179">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="8ef6d-2180">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="8ef6d-2181">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="8ef6d-2182">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8ef6d-2182">Provide feedback from the command line with the `az feedback` command</span></span>

