---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/05/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: b79d76480c3e6619427d6a7e3960f53b691889cc
ms.sourcegitcommit: 6aca5a788b9731e6cbeeb497c83a9197ebb7d36e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/06/2019
ms.locfileid: "66750236"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f6c21-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6c21-103">Azure CLI release notes</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="f6c21-104">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-104">June 4, 2019</span></span>

<span data-ttu-id="f6c21-105">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="f6c21-105">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-106">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-106">Core</span></span>
* <span data-ttu-id="f6c21-107">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="f6c21-107">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-108">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-108">ACR</span></span>
* <span data-ttu-id="f6c21-109">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="f6c21-109">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-110">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-110">ACS</span></span>
* <span data-ttu-id="f6c21-111">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-111">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="f6c21-112">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="f6c21-112">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-113">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-113">Batch</span></span>
* <span data-ttu-id="f6c21-114">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="f6c21-114">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-115">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-115">IoT</span></span>
* <span data-ttu-id="f6c21-116">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-116">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-117">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-117">Network</span></span>
* <span data-ttu-id="f6c21-118">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="f6c21-118">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="f6c21-119">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-119">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="f6c21-120">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-120">Resource</span></span>
* <span data-ttu-id="f6c21-121">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="f6c21-121">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-122">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-122">Role</span></span>
* <span data-ttu-id="f6c21-123">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="f6c21-123">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="f6c21-124">Calcul</span><span class="sxs-lookup"><span data-stu-id="f6c21-124">Compute</span></span>
* <span data-ttu-id="f6c21-125">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="f6c21-125">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="f6c21-126">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-126">May 21, 2019</span></span>

<span data-ttu-id="f6c21-127">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="f6c21-127">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-128">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-128">Core</span></span>
* <span data-ttu-id="f6c21-129">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="f6c21-129">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="f6c21-130">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="f6c21-130">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="f6c21-131">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="f6c21-131">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-132">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-132">ACR</span></span>
* <span data-ttu-id="f6c21-133">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="f6c21-133">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-134">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-134">ACS</span></span>
* <span data-ttu-id="f6c21-135">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="f6c21-135">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-136">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-136">AppService</span></span>
* <span data-ttu-id="f6c21-137">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="f6c21-137">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="f6c21-138">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="f6c21-138">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="f6c21-139">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="f6c21-139">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="f6c21-140">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="f6c21-140">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="f6c21-141">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6c21-141">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="f6c21-142">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="f6c21-142">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="f6c21-143">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-143">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-144">BotService</span><span class="sxs-lookup"><span data-stu-id="f6c21-144">BotService</span></span>
* <span data-ttu-id="f6c21-145">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-145">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="f6c21-146">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-146">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-147">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-147">Consumption</span></span>
* <span data-ttu-id="f6c21-148">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-148">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-149">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-149">IoT</span></span>
* <span data-ttu-id="f6c21-150">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="f6c21-150">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-151">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-151">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="f6c21-153">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="f6c21-153">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="f6c21-154">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="f6c21-154">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-155">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-155">RDBMS</span></span>
* <span data-ttu-id="f6c21-156">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="f6c21-156">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="f6c21-157">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6c21-157">RBAC</span></span>
* <span data-ttu-id="f6c21-158">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="f6c21-158">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-159">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-159">Storage</span></span>
* <span data-ttu-id="f6c21-160">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-160">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="f6c21-161">Calcul</span><span class="sxs-lookup"><span data-stu-id="f6c21-161">Compute</span></span>
* <span data-ttu-id="f6c21-162">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-162">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="f6c21-163">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="f6c21-163">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="f6c21-164">__Remarque__: il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="f6c21-164">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="f6c21-165">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-165">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="f6c21-166">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-166">May 6, 2019</span></span>

<span data-ttu-id="f6c21-167">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="f6c21-167">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-168">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-168">ACS</span></span>
* <span data-ttu-id="f6c21-169">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="f6c21-169">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="f6c21-170">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="f6c21-170">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="f6c21-171">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-171">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="f6c21-172">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-172">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-173">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-173">Appservice</span></span>
* <span data-ttu-id="f6c21-174">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="f6c21-174">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="f6c21-175">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="f6c21-175">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="f6c21-176">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6c21-176">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="f6c21-177">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="f6c21-177">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="f6c21-178">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6c21-178">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="f6c21-179">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="f6c21-179">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="f6c21-180">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="f6c21-180">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="f6c21-181">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="f6c21-181">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="f6c21-182">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-182">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="f6c21-183">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="f6c21-183">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-184">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-184">Batch</span></span>
* <span data-ttu-id="f6c21-185">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="f6c21-185">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-186">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6c21-186">Botservice</span></span>
* <span data-ttu-id="f6c21-187">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="f6c21-187">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="f6c21-188">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="f6c21-188">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="f6c21-189">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="f6c21-189">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="f6c21-190">__REMARQUE :__  `bot prepare-publish` utilise toujours l’ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-190">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="f6c21-191">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-191">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="f6c21-192">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-192">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="f6c21-193">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-193">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="f6c21-194">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="f6c21-194">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="f6c21-195">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="f6c21-195">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="f6c21-196">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="f6c21-196">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="f6c21-197">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="f6c21-197">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="f6c21-198">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="f6c21-198">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="f6c21-199">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="f6c21-199">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="f6c21-200">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="f6c21-200">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="f6c21-201">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-201">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="f6c21-202">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="f6c21-202">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="f6c21-203">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-203">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f6c21-204">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="f6c21-204">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="f6c21-205">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="f6c21-205">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="f6c21-206">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-206">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f6c21-207">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="f6c21-207">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="f6c21-208">Configuration</span><span class="sxs-lookup"><span data-stu-id="f6c21-208">Configure</span></span>
* <span data-ttu-id="f6c21-209">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="f6c21-209">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6c21-210">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="f6c21-210">Eventhubs</span></span>
* <span data-ttu-id="f6c21-211">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-211">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f6c21-212">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-212">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-213">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-213">Network</span></span>
* <span data-ttu-id="f6c21-214">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-214">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="f6c21-215">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6c21-215">Policy Insights</span></span>
* <span data-ttu-id="f6c21-216">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-216">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-217">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-217">Role</span></span>
* <span data-ttu-id="f6c21-218">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-218">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6c21-219">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6c21-219">Service Bus</span></span>
* <span data-ttu-id="f6c21-220">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-220">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f6c21-221">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-221">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="f6c21-222">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="f6c21-222">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-223">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-223">SQL</span></span>
* <span data-ttu-id="f6c21-224">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-224">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-225">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-225">VM</span></span>
* <span data-ttu-id="f6c21-226">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="f6c21-226">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="f6c21-227">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="f6c21-227">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="f6c21-228">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-228">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="f6c21-229">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="f6c21-229">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="f6c21-230">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="f6c21-230">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="f6c21-231">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-231">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="f6c21-232">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-232">April 23, 2019</span></span>

<span data-ttu-id="f6c21-233">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="f6c21-233">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-234">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-234">ACS</span></span>
* <span data-ttu-id="f6c21-235">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="f6c21-235">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="f6c21-236">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="f6c21-236">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-237">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-237">AMS</span></span>
* <span data-ttu-id="f6c21-238">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="f6c21-238">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-239">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-239">AppService</span></span>
* <span data-ttu-id="f6c21-240">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="f6c21-240">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="f6c21-241">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="f6c21-241">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="f6c21-242">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="f6c21-242">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="f6c21-243">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="f6c21-243">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="f6c21-244">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="f6c21-244">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="f6c21-245">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-245">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="f6c21-246">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="f6c21-246">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="f6c21-247">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="f6c21-247">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="f6c21-248">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="f6c21-248">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="f6c21-249">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="f6c21-249">Deployment Manager</span></span>
* <span data-ttu-id="f6c21-250">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="f6c21-250">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="f6c21-251">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-251">Lab</span></span>
* <span data-ttu-id="f6c21-252">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="f6c21-252">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-253">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-253">Network</span></span>
* <span data-ttu-id="f6c21-254">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="f6c21-254">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-255">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-255">Resource</span></span>
* <span data-ttu-id="f6c21-256">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="f6c21-256">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="f6c21-257">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="f6c21-257">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="f6c21-258">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-258">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="f6c21-259">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-259">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-260">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-260">SQL</span></span>
* <span data-ttu-id="f6c21-261">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="f6c21-261">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="f6c21-262">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-262">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="f6c21-263">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-263">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="f6c21-264">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-264">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-265">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-265">Storage</span></span>
* <span data-ttu-id="f6c21-266">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="f6c21-266">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-267">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-267">VM</span></span>
* <span data-ttu-id="f6c21-268">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="f6c21-268">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="f6c21-269">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="f6c21-269">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="f6c21-270">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="f6c21-270">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="f6c21-271">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-271">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-272">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-272">Core</span></span>
* <span data-ttu-id="f6c21-273">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="f6c21-273">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-274">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-274">ACR</span></span>
* <span data-ttu-id="f6c21-275">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="f6c21-275">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-276">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-276">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="f6c21-279">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-279">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="f6c21-280">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-280">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-281">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-281">AppService</span></span>
* <span data-ttu-id="f6c21-282">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6c21-282">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="f6c21-283">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-283">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="f6c21-284">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-284">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="f6c21-285">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="f6c21-285">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="f6c21-286">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-286">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="f6c21-287">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="f6c21-287">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="f6c21-288">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="f6c21-288">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-289">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-289">CDN</span></span>
* <span data-ttu-id="f6c21-290">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="f6c21-290">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="f6c21-291">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f6c21-291">Feedback</span></span>
* <span data-ttu-id="f6c21-292">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="f6c21-292">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="f6c21-293">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="f6c21-293">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="f6c21-294">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="f6c21-294">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-295">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-295">Monitor</span></span>
* <span data-ttu-id="f6c21-296">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-296">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="f6c21-297">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-297">Network</span></span>
* <span data-ttu-id="f6c21-298">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="f6c21-298">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="f6c21-299">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-299">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="f6c21-300">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="f6c21-300">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="f6c21-301">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-301">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="f6c21-302">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="f6c21-302">PrivateDNS</span></span>
* <span data-ttu-id="f6c21-303">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="f6c21-303">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-304">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-304">Resource</span></span>
* <span data-ttu-id="f6c21-305">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-305">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-306">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-306">Role</span></span>
* <span data-ttu-id="f6c21-307">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-307">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="f6c21-308">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-308">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-309">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-309">SQL</span></span>
* <span data-ttu-id="f6c21-310">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="f6c21-310">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-311">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-311">Storage</span></span>
* <span data-ttu-id="f6c21-312">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-312">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="f6c21-313">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="f6c21-313">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="f6c21-314">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="f6c21-314">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="f6c21-315">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="f6c21-315">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="f6c21-316">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-316">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="f6c21-317">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-317">Core</span></span>
* <span data-ttu-id="f6c21-318">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="f6c21-318">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="f6c21-319">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="f6c21-319">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="f6c21-320">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-320">Cloud</span></span>
* <span data-ttu-id="f6c21-321">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="f6c21-321">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-322">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-322">ACR</span></span>
* <span data-ttu-id="f6c21-323">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="f6c21-323">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="f6c21-324">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-324">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="f6c21-325">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="f6c21-325">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="f6c21-326">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="f6c21-326">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-327">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-327">AppService</span></span>
* <span data-ttu-id="f6c21-328">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="f6c21-328">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="f6c21-329">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="f6c21-329">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="f6c21-330">Service BOT</span><span class="sxs-lookup"><span data-stu-id="f6c21-330">BOT Service</span></span>
* <span data-ttu-id="f6c21-331">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="f6c21-331">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="f6c21-332">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="f6c21-332">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="f6c21-333">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="f6c21-333">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="f6c21-334">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="f6c21-334">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-335">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-335">CDN</span></span>
* <span data-ttu-id="f6c21-336">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-336">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="f6c21-337">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-337">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="f6c21-338">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="f6c21-338">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f6c21-339">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="f6c21-339">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-340">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f6c21-340">Cosmosdb</span></span>
* <span data-ttu-id="f6c21-341">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="f6c21-341">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="f6c21-342">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6c21-342">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-343">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-343">Interactive</span></span>
* <span data-ttu-id="f6c21-344">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="f6c21-344">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-345">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-345">Monitor</span></span>
* <span data-ttu-id="f6c21-346">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-346">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-347">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-347">Network</span></span>
* <span data-ttu-id="f6c21-348">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="f6c21-348">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-349">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-349">Profile</span></span>
* <span data-ttu-id="f6c21-350">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="f6c21-350">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="f6c21-351">Postgres</span><span class="sxs-lookup"><span data-stu-id="f6c21-351">Postgres</span></span> 
* <span data-ttu-id="f6c21-352">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="f6c21-352">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="f6c21-353">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="f6c21-353">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-354">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-354">Resource</span></span>
* <span data-ttu-id="f6c21-355">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-355">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="f6c21-356">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="f6c21-356">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="f6c21-357">Graph</span><span class="sxs-lookup"><span data-stu-id="f6c21-357">Graph</span></span>
* <span data-ttu-id="f6c21-358">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="f6c21-358">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="f6c21-359">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="f6c21-359">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="f6c21-360">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="f6c21-360">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="f6c21-361">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-361">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="f6c21-362">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="f6c21-362">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-363">storage</span><span class="sxs-lookup"><span data-stu-id="f6c21-363">storage</span></span>
* <span data-ttu-id="f6c21-364">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="f6c21-364">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="f6c21-365">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="f6c21-365">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="f6c21-366">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="f6c21-366">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="f6c21-367">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="f6c21-367">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-368">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-368">VM</span></span>
* <span data-ttu-id="f6c21-369">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-369">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="f6c21-370">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-370">March 12, 2019</span></span>

<span data-ttu-id="f6c21-371">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="f6c21-371">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-372">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-372">Core</span></span>

* <span data-ttu-id="f6c21-373">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="f6c21-373">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-374">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-374">ACR</span></span>

* <span data-ttu-id="f6c21-375">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="f6c21-375">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-376">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-376">ACS</span></span>

* <span data-ttu-id="f6c21-377">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="f6c21-377">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="f6c21-378">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-378">AppService</span></span>

* <span data-ttu-id="f6c21-379">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="f6c21-379">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="f6c21-380">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-380">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="f6c21-381">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-381">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="f6c21-382">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-382">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-383">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6c21-383">Botservice</span></span>

* <span data-ttu-id="f6c21-384">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="f6c21-384">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f6c21-385">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="f6c21-385">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f6c21-386">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-386">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="f6c21-387">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="f6c21-387">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-388">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-388">Container</span></span>

* <span data-ttu-id="f6c21-389">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-389">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6c21-390">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f6c21-390">EventHub</span></span>

* <span data-ttu-id="f6c21-391">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="f6c21-391">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="f6c21-392">Rechercher</span><span class="sxs-lookup"><span data-stu-id="f6c21-392">Find</span></span>

* <span data-ttu-id="f6c21-393">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="f6c21-393">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6c21-394">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6c21-394">HDInsight</span></span>

* <span data-ttu-id="f6c21-395">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="f6c21-395">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-396">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-396">Network</span></span>

* <span data-ttu-id="f6c21-397">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="f6c21-397">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-398">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6c21-398">Rdbms</span></span>

* <span data-ttu-id="f6c21-399">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="f6c21-399">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-400">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-400">Role</span></span>

* <span data-ttu-id="f6c21-401">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="f6c21-401">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="f6c21-402">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="f6c21-402">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6c21-403">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6c21-403">Service Fabric</span></span>

* <span data-ttu-id="f6c21-404">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="f6c21-404">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="f6c21-405">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-405">February 26, 2019</span></span>

<span data-ttu-id="f6c21-406">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="f6c21-406">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-407">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-407">Core</span></span>

* <span data-ttu-id="f6c21-408">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="f6c21-408">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-409">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-409">ACR</span></span>

* <span data-ttu-id="f6c21-410">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-410">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="f6c21-411">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="f6c21-411">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-412">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-412">ACS</span></span>

* <span data-ttu-id="f6c21-413">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="f6c21-413">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-414">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-414">AppService</span></span>

* <span data-ttu-id="f6c21-415">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="f6c21-415">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-416">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-416">Batch</span></span>
* <span data-ttu-id="f6c21-417">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="f6c21-417">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="f6c21-418">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="f6c21-418">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="f6c21-419">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="f6c21-419">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="f6c21-420">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="f6c21-420">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="f6c21-421">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="f6c21-421">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="f6c21-422">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="f6c21-422">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-423">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-423">CosmosDB</span></span>

* <span data-ttu-id="f6c21-424">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6c21-424">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="f6c21-425">Kusto</span><span class="sxs-lookup"><span data-stu-id="f6c21-425">Kusto</span></span>

* <span data-ttu-id="f6c21-426">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="f6c21-426">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-427">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-427">Network</span></span>

* <span data-ttu-id="f6c21-428">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-428">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="f6c21-429">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="f6c21-429">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="f6c21-430">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="f6c21-430">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="f6c21-431">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-431">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="f6c21-432">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-432">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="f6c21-433">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-433">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="f6c21-434">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="f6c21-434">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-435">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-435">Resource</span></span>

* <span data-ttu-id="f6c21-436">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-436">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="f6c21-437">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-437">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="f6c21-438">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-438">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="f6c21-439">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-439">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="f6c21-440">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-440">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-441">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-441">Role</span></span>

* <span data-ttu-id="f6c21-442">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-442">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-443">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-443">VM</span></span>

* <span data-ttu-id="f6c21-444">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="f6c21-444">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="f6c21-445">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-445">February 12, 2019</span></span>

<span data-ttu-id="f6c21-446">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="f6c21-446">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-447">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-447">Core</span></span>

* <span data-ttu-id="f6c21-448">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="f6c21-448">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="f6c21-449">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="f6c21-449">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-450">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-450">ACR</span></span>
* <span data-ttu-id="f6c21-451">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="f6c21-451">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="f6c21-452">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-452">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-453">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-453">ACS</span></span>
* <span data-ttu-id="f6c21-454">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-454">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="f6c21-455">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="f6c21-455">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="f6c21-456">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f6c21-456">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-457">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-457">AMS</span></span>
* <span data-ttu-id="f6c21-458">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-458">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="f6c21-459">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-459">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-460">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-460">Appservice</span></span>
* <span data-ttu-id="f6c21-461">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-461">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="f6c21-462">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="f6c21-462">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="f6c21-463">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-463">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="f6c21-464">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="f6c21-464">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="f6c21-465">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="f6c21-465">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-466">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6c21-466">Botservice</span></span>
* <span data-ttu-id="f6c21-467">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="f6c21-467">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="f6c21-468">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="f6c21-468">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="f6c21-469">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-469">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="f6c21-470">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="f6c21-470">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="f6c21-471">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="f6c21-471">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="f6c21-472">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="f6c21-472">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="f6c21-473">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="f6c21-473">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="f6c21-474">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="f6c21-474">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="f6c21-475">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="f6c21-475">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="f6c21-476">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="f6c21-476">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6c21-477">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6c21-477">Key Vault</span></span>
* <span data-ttu-id="f6c21-478">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="f6c21-478">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-479">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-479">Monitor</span></span>
* <span data-ttu-id="f6c21-480">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="f6c21-480">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-481">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-481">Network</span></span>
* <span data-ttu-id="f6c21-482">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="f6c21-482">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="f6c21-483">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="f6c21-483">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="f6c21-484">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f6c21-484">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="f6c21-485">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-485">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f6c21-486">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6c21-486">Policy Insights</span></span>
* <span data-ttu-id="f6c21-487">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="f6c21-487">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-488">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-488">RDBMS</span></span>
* <span data-ttu-id="f6c21-489">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-489">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="f6c21-490">Redis</span><span class="sxs-lookup"><span data-stu-id="f6c21-490">Redis</span></span>
* <span data-ttu-id="f6c21-491">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="f6c21-491">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="f6c21-492">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="f6c21-492">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="f6c21-493">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="f6c21-493">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="f6c21-494">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="f6c21-494">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="f6c21-495">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="f6c21-495">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="f6c21-496">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="f6c21-496">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="f6c21-497">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="f6c21-497">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-498">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-498">Role</span></span>
* <span data-ttu-id="f6c21-499">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="f6c21-499">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="f6c21-500">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-500">SQL VM</span></span>
* <span data-ttu-id="f6c21-501">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="f6c21-501">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-502">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-502">VM</span></span>
* <span data-ttu-id="f6c21-503">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="f6c21-503">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="f6c21-504">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-504">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="f6c21-505">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="f6c21-505">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="f6c21-506">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="f6c21-506">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="f6c21-507">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-507">January 31, 2019</span></span>

<span data-ttu-id="f6c21-508">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="f6c21-508">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-509">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-509">Core</span></span>

* <span data-ttu-id="f6c21-510">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="f6c21-510">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="f6c21-511">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-511">January 28, 2019</span></span>

<span data-ttu-id="f6c21-512">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="f6c21-512">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-513">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-513">ACR</span></span>
* <span data-ttu-id="f6c21-514">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="f6c21-514">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-515">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-515">ACS</span></span>
* <span data-ttu-id="f6c21-516">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="f6c21-516">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f6c21-517">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="f6c21-517">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="f6c21-518">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="f6c21-518">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-519">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-519">AMS</span></span>
* <span data-ttu-id="f6c21-520">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="f6c21-520">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="f6c21-521">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="f6c21-521">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-522">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-522">Appservice</span></span>
* <span data-ttu-id="f6c21-523">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-523">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="f6c21-524">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="f6c21-524">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="f6c21-525">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="f6c21-525">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-526">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-526">Container</span></span>
* <span data-ttu-id="f6c21-527">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="f6c21-527">Added `container start` command</span></span>
* <span data-ttu-id="f6c21-528">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-528">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6c21-529">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f6c21-529">EventGrid</span></span>
* <span data-ttu-id="f6c21-530">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-530">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="f6c21-531">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="f6c21-531">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="f6c21-532">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="f6c21-532">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="f6c21-533">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="f6c21-533">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="f6c21-534">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="f6c21-534">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6c21-535">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6c21-535">HDInsight</span></span>
* <span data-ttu-id="f6c21-536">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-536">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="f6c21-537">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="f6c21-537">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="f6c21-538">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-538">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="f6c21-539">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-539">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="f6c21-540">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="f6c21-540">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="f6c21-541">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-541">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-542">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-542">IoT</span></span>
* <span data-ttu-id="f6c21-543">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="f6c21-543">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="f6c21-544">Kusto</span><span class="sxs-lookup"><span data-stu-id="f6c21-544">Kusto</span></span>
* <span data-ttu-id="f6c21-545">Préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-545">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-546">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-546">Monitor</span></span>
* <span data-ttu-id="f6c21-547">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-547">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-548">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-548">Profile</span></span>
* <span data-ttu-id="f6c21-549">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="f6c21-549">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-550">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-550">Network</span></span>
* <span data-ttu-id="f6c21-551">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="f6c21-551">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="f6c21-552">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="f6c21-552">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-553">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-553">Resource</span></span>
* <span data-ttu-id="f6c21-554">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-554">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="f6c21-555">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-555">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="f6c21-556">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-556">SQL Virtual Machine</span></span>
* <span data-ttu-id="f6c21-557">Préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-557">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-558">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-558">Storage</span></span>
* <span data-ttu-id="f6c21-559">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="f6c21-559">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="f6c21-560">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="f6c21-560">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-561">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-561">VM</span></span>
* <span data-ttu-id="f6c21-562">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="f6c21-562">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="f6c21-563">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f6c21-563">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="f6c21-564">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="f6c21-564">January 15, 2019</span></span>

<span data-ttu-id="f6c21-565">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="f6c21-565">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-566">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-566">ACR</span></span>
* <span data-ttu-id="f6c21-567">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-567">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="f6c21-568">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="f6c21-568">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="f6c21-569">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-569">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="f6c21-570">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-570">ACS</span></span>
* <span data-ttu-id="f6c21-571">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="f6c21-571">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-572">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-572">Appservice</span></span>
* <span data-ttu-id="f6c21-573">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="f6c21-573">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="f6c21-574">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-574">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="f6c21-575">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="f6c21-575">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="f6c21-576">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="f6c21-576">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-577">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6c21-577">Botservice</span></span>
* <span data-ttu-id="f6c21-578">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-578">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="f6c21-579">Configuration</span><span class="sxs-lookup"><span data-stu-id="f6c21-579">Configure</span></span>
* <span data-ttu-id="f6c21-580">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="f6c21-580">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-581">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-581">CosmosDB</span></span>
* <span data-ttu-id="f6c21-582">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="f6c21-582">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6c21-583">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6c21-583">HDInsight</span></span>
* <span data-ttu-id="f6c21-584">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="f6c21-584">Added commands for managing applications</span></span>
* <span data-ttu-id="f6c21-585">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="f6c21-585">Added commands for managing script actions</span></span>
* <span data-ttu-id="f6c21-586">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="f6c21-586">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="f6c21-587">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="f6c21-587">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="f6c21-588">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-588">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-589">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-589">Network</span></span>
* <span data-ttu-id="f6c21-590">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-590">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="f6c21-591">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="f6c21-591">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="f6c21-592">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-592">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="f6c21-593">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-593">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-594">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-594">Role</span></span>
* <span data-ttu-id="f6c21-595">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-595">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="f6c21-596">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="f6c21-596">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="f6c21-597">Sécurité</span><span class="sxs-lookup"><span data-stu-id="f6c21-597">Security</span></span>
* <span data-ttu-id="f6c21-598">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-598">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-599">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-599">Storage</span></span>
* <span data-ttu-id="f6c21-600">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="f6c21-600">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="f6c21-601">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="f6c21-601">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="f6c21-602">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-602">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="f6c21-603">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-603">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="f6c21-604">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-604">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-605">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-605">VM</span></span>
* <span data-ttu-id="f6c21-606">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="f6c21-606">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="f6c21-607">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-607">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6c21-608">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="f6c21-608">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="f6c21-609">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-609">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="f6c21-610">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-610">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="f6c21-611">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="f6c21-611">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="f6c21-612">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-612">December 20, 2018</span></span>

<span data-ttu-id="f6c21-613">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="f6c21-613">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="f6c21-614">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-614">Appservice</span></span>
* <span data-ttu-id="f6c21-615">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6c21-615">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="f6c21-616">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="f6c21-616">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="f6c21-617">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-617">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6c21-618">IotCentral</span><span class="sxs-lookup"><span data-stu-id="f6c21-618">IoTCentral</span></span>
* <span data-ttu-id="f6c21-619">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="f6c21-619">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-620">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-620">Role</span></span>
* <span data-ttu-id="f6c21-621">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="f6c21-621">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-622">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-622">SQL</span></span>
* <span data-ttu-id="f6c21-623">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="f6c21-623">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-624">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-624">VM</span></span>
* <span data-ttu-id="f6c21-625">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-625">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="f6c21-626">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-626">December 18, 2018</span></span>

<span data-ttu-id="f6c21-627">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="f6c21-627">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="f6c21-628">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-628">ACR</span></span>
* <span data-ttu-id="f6c21-629">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="f6c21-629">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="f6c21-630">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="f6c21-630">Condensed the table layout for task list</span></span>
* <span data-ttu-id="f6c21-631">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="f6c21-631">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-632">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-632">ACS</span></span>
* <span data-ttu-id="f6c21-633">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="f6c21-633">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f6c21-634">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-634">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="f6c21-635">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-635">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="f6c21-636">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="f6c21-636">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="f6c21-637">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-637">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="f6c21-638">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="f6c21-638">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-639">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-639">Appservice</span></span>
* <span data-ttu-id="f6c21-640">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="f6c21-640">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="f6c21-641">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6c21-641">Botservice</span></span>
* <span data-ttu-id="f6c21-642">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-642">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="f6c21-643">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="f6c21-643">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="f6c21-644">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="f6c21-644">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="f6c21-645">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="f6c21-645">Reduced Kudu network calls</span></span>
* <span data-ttu-id="f6c21-646">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="f6c21-646">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-647">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-647">Consumption</span></span>
* <span data-ttu-id="f6c21-648">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="f6c21-648">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-649">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-649">CosmosDB</span></span>
* <span data-ttu-id="f6c21-650">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="f6c21-650">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="f6c21-651">Cartes</span><span class="sxs-lookup"><span data-stu-id="f6c21-651">Maps</span></span>
* <span data-ttu-id="f6c21-652">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-652">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-653">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-653">Network</span></span>
* <span data-ttu-id="f6c21-654">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="f6c21-654">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="f6c21-655">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-655">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-656">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-656">Resource</span></span>
* <span data-ttu-id="f6c21-657">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-657">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="f6c21-658">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-658">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-659">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-659">Storage</span></span>
*  <span data-ttu-id="f6c21-660">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-660">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-661">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-661">VM</span></span>
* <span data-ttu-id="f6c21-662">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="f6c21-662">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="f6c21-663">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-663">December 4, 2018</span></span>

<span data-ttu-id="f6c21-664">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="f6c21-664">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="f6c21-665">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-665">Core</span></span>
* <span data-ttu-id="f6c21-666">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="f6c21-666">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="f6c21-667">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="f6c21-667">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-668">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-668">Appservice</span></span>
* <span data-ttu-id="f6c21-669">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="f6c21-669">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="f6c21-670">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="f6c21-670">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-671">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-671">Network</span></span>
* <span data-ttu-id="f6c21-672">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="f6c21-672">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-673">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-673">Role</span></span>
* <span data-ttu-id="f6c21-674">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="f6c21-674">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="f6c21-675">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-675">VM</span></span>
* <span data-ttu-id="f6c21-676">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="f6c21-676">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="f6c21-677">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="f6c21-677">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="f6c21-678">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="f6c21-678">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="f6c21-679">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="f6c21-679">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="f6c21-680">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-680">November 20, 2018</span></span>

<span data-ttu-id="f6c21-681">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="f6c21-681">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="f6c21-682">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-682">Core</span></span>
* <span data-ttu-id="f6c21-683">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="f6c21-683">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-684">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-684">ACR</span></span>
* <span data-ttu-id="f6c21-685">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="f6c21-685">Added context token to task step</span></span>
* <span data-ttu-id="f6c21-686">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="f6c21-686">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="f6c21-687">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="f6c21-687">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-688">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-688">Appservice</span></span>
* <span data-ttu-id="f6c21-689">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="f6c21-689">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="f6c21-690">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-690">Updated the default `node_version`.</span></span> <span data-ttu-id="f6c21-691">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="f6c21-691">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="f6c21-692">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-692">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="f6c21-693">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="f6c21-693">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6c21-694">IotCentral</span><span class="sxs-lookup"><span data-stu-id="f6c21-694">IotCentral</span></span>
* <span data-ttu-id="f6c21-695">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6c21-695">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-696">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-696">KeyVault</span></span>
* <span data-ttu-id="f6c21-697">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="f6c21-697">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-698">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-698">Network</span></span>
* <span data-ttu-id="f6c21-699">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="f6c21-699">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="f6c21-700">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="f6c21-700">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="f6c21-701">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-701">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="f6c21-702">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="f6c21-702">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-703">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6c21-703">Rdbms</span></span>
* <span data-ttu-id="f6c21-704">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="f6c21-704">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="f6c21-705">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="f6c21-705">Rbac</span></span>
* <span data-ttu-id="f6c21-706">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-706">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="f6c21-707">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-707">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="f6c21-708">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-708">Storage</span></span>
* <span data-ttu-id="f6c21-709">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-709">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="f6c21-710">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-710">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="f6c21-711">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="f6c21-711">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="f6c21-712">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="f6c21-712">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-713">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-713">VM</span></span>
* <span data-ttu-id="f6c21-714">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="f6c21-714">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="f6c21-715">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="f6c21-715">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="f6c21-716">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="f6c21-716">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="f6c21-717">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="f6c21-717">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="f6c21-718">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-718">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="f6c21-719">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-719">Added `snapshot wait` command</span></span>
* <span data-ttu-id="f6c21-720">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-720">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f6c21-721">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-721">November 6, 2018</span></span>

<span data-ttu-id="f6c21-722">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f6c21-722">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-723">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-723">Core</span></span>
* <span data-ttu-id="f6c21-724">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="f6c21-724">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-725">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-725">ACR</span></span>
* <span data-ttu-id="f6c21-726">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="f6c21-726">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f6c21-727">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="f6c21-727">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-728">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-728">ACS</span></span>
* <span data-ttu-id="f6c21-729">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-729">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f6c21-730">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6c21-730">Advisor</span></span>
* <span data-ttu-id="f6c21-731">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="f6c21-731">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-732">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-732">AMS</span></span>
* <span data-ttu-id="f6c21-733">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-733">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f6c21-734">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-734">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f6c21-735">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-735">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f6c21-736">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="f6c21-736">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f6c21-737">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="f6c21-737">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f6c21-738">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="f6c21-738">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f6c21-739">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="f6c21-739">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f6c21-740">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="f6c21-740">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f6c21-741">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="f6c21-741">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f6c21-742">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="f6c21-742">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f6c21-743">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-743">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f6c21-744">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-744">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f6c21-745">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="f6c21-745">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f6c21-746">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="f6c21-746">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f6c21-747">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-747">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f6c21-748">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="f6c21-748">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f6c21-749">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="f6c21-749">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-750">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-750">AppService</span></span>
* <span data-ttu-id="f6c21-751">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="f6c21-751">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f6c21-752">Configuration</span><span class="sxs-lookup"><span data-stu-id="f6c21-752">Configure</span></span>
* <span data-ttu-id="f6c21-753">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="f6c21-753">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-754">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-754">Container</span></span>
* <span data-ttu-id="f6c21-755">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="f6c21-755">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6c21-756">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f6c21-756">EventHub</span></span>
* <span data-ttu-id="f6c21-757">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-757">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-758">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-758">Interactive</span></span>
* <span data-ttu-id="f6c21-759">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="f6c21-759">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-760">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-760">Monitor</span></span>
* <span data-ttu-id="f6c21-761">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-761">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-762">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-762">Network</span></span>
* <span data-ttu-id="f6c21-763">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="f6c21-763">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f6c21-764">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-764">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f6c21-765">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-765">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f6c21-766">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-766">Profile</span></span>
* <span data-ttu-id="f6c21-767">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="f6c21-767">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-768">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-768">RDBMS</span></span>
* <span data-ttu-id="f6c21-769">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="f6c21-769">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-770">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-770">Resource</span></span>
* <span data-ttu-id="f6c21-771">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="f6c21-771">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-772">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-772">Role</span></span>
* <span data-ttu-id="f6c21-773">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="f6c21-773">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f6c21-774">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="f6c21-774">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f6c21-775">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="f6c21-775">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-776">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-776">Storage</span></span>
* <span data-ttu-id="f6c21-777">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="f6c21-777">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-778">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-778">VM</span></span>
* <span data-ttu-id="f6c21-779">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="f6c21-779">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f6c21-780">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-780">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f6c21-781">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="f6c21-781">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f6c21-782">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="f6c21-782">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f6c21-783">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="f6c21-783">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f6c21-784">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="f6c21-784">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f6c21-785">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-785">October 23, 2018</span></span>

<span data-ttu-id="f6c21-786">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f6c21-786">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-787">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-787">Core</span></span>
* <span data-ttu-id="f6c21-788">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="f6c21-788">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f6c21-789">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="f6c21-789">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-790">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-790">ACR</span></span>
* <span data-ttu-id="f6c21-791">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="f6c21-791">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-792">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-792">CDN</span></span>
* <span data-ttu-id="f6c21-793">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="f6c21-793">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f6c21-794">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="f6c21-794">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-795">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-795">Container</span></span>
* <span data-ttu-id="f6c21-796">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="f6c21-796">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f6c21-797">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-797">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f6c21-798">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="f6c21-798">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f6c21-799">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-799">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f6c21-800">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="f6c21-800">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f6c21-801">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="f6c21-801">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f6c21-802">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-802">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-803">CosmosDB</span></span>
* <span data-ttu-id="f6c21-804">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-804">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-805">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-805">Interactive</span></span>
* <span data-ttu-id="f6c21-806">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="f6c21-806">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6c21-807">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6c21-807">IoT Central</span></span>
* <span data-ttu-id="f6c21-808">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="f6c21-808">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f6c21-809">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="f6c21-809">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-810">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-810">Monitor</span></span>
* <span data-ttu-id="f6c21-811">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="f6c21-811">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f6c21-812">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-812">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f6c21-813">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="f6c21-813">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6c21-814">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="f6c21-814">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f6c21-815">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="f6c21-815">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f6c21-816">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="f6c21-816">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f6c21-817">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="f6c21-817">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f6c21-818">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="f6c21-818">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6c21-819">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="f6c21-819">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f6c21-820">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-820">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-821">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-821">Network</span></span>
* <span data-ttu-id="f6c21-822">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-822">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f6c21-823">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-823">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f6c21-824">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f6c21-824">ServiceBus</span></span>
* <span data-ttu-id="f6c21-825">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6c21-825">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-826">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-826">SQL</span></span>
* <span data-ttu-id="f6c21-827">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-827">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-828">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-828">Storage</span></span>
* <span data-ttu-id="f6c21-829">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="f6c21-829">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f6c21-830">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="f6c21-830">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-831">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-831">VM</span></span>
* <span data-ttu-id="f6c21-832">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-832">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6c21-833">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-833">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f6c21-834">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-834">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f6c21-835">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-835">October 16, 2018</span></span>

<span data-ttu-id="f6c21-836">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f6c21-836">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-837">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-837">VM</span></span>
* <span data-ttu-id="f6c21-838">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="f6c21-838">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f6c21-839">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-839">October 9, 2018</span></span>

<span data-ttu-id="f6c21-840">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f6c21-840">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-841">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-841">Core</span></span>
* <span data-ttu-id="f6c21-842">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="f6c21-842">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-843">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-843">ACR</span></span>
* <span data-ttu-id="f6c21-844">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="f6c21-844">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-845">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-845">ACS</span></span>
* <span data-ttu-id="f6c21-846">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="f6c21-846">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f6c21-847">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="f6c21-847">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f6c21-848">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="f6c21-848">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f6c21-849">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="f6c21-849">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-850">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-850">Container</span></span>
* <span data-ttu-id="f6c21-851">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="f6c21-851">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f6c21-852">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-852">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f6c21-853">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f6c21-853">Event Hub</span></span>
* <span data-ttu-id="f6c21-854">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-854">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f6c21-855">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="f6c21-855">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f6c21-856">Extensions</span><span class="sxs-lookup"><span data-stu-id="f6c21-856">Extensions</span></span>
* <span data-ttu-id="f6c21-857">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="f6c21-857">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6c21-858">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6c21-858">HDInsight</span></span>
* <span data-ttu-id="f6c21-859">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-859">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-860">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-860">IoT</span></span>
* <span data-ttu-id="f6c21-861">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="f6c21-861">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-862">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-862">KeyVault</span></span>
* <span data-ttu-id="f6c21-863">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="f6c21-863">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-864">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-864">Network</span></span>
* <span data-ttu-id="f6c21-865">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="f6c21-865">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f6c21-866">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="f6c21-866">See #6052</span></span>
* <span data-ttu-id="f6c21-867">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-867">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f6c21-868">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="f6c21-868">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f6c21-869">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f6c21-869">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f6c21-870">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f6c21-870">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f6c21-871">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="f6c21-871">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f6c21-872">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-872">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-873">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-873">Role</span></span>
* <span data-ttu-id="f6c21-874">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="f6c21-874">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f6c21-875">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="f6c21-875">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f6c21-876">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="f6c21-876">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f6c21-877">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="f6c21-877">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6c21-878">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6c21-878">Service Bus</span></span>
* <span data-ttu-id="f6c21-879">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="f6c21-879">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-880">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-880">VM</span></span>
* <span data-ttu-id="f6c21-881">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="f6c21-881">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f6c21-882">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-882">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f6c21-883">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="f6c21-883">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f6c21-884">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="f6c21-884">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f6c21-885">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-885">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f6c21-886">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="f6c21-886">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f6c21-887">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-887">September 21, 2018</span></span>

<span data-ttu-id="f6c21-888">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f6c21-888">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-889">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-889">ACR</span></span>
* <span data-ttu-id="f6c21-890">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-890">Added ACR Task commands</span></span>
* <span data-ttu-id="f6c21-891">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="f6c21-891">Added quick run command</span></span>
* <span data-ttu-id="f6c21-892">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="f6c21-892">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f6c21-893">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-893">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f6c21-894">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="f6c21-894">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f6c21-895">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="f6c21-895">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-896">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-896">ACS</span></span>
* <span data-ttu-id="f6c21-897">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-897">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f6c21-898">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="f6c21-898">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-899">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-899">AppService</span></span>

* <span data-ttu-id="f6c21-900">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="f6c21-900">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f6c21-901">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="f6c21-901">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f6c21-902">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="f6c21-902">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f6c21-903">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="f6c21-903">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-904">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-904">Batch</span></span>
* <span data-ttu-id="f6c21-905">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="f6c21-905">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f6c21-906">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="f6c21-906">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f6c21-907">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-907">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f6c21-908">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="f6c21-908">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6c21-909">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-909">Batch AI</span></span> 
* <span data-ttu-id="f6c21-910">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-910">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6c21-911">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-911">Cognitive Services</span></span>
* <span data-ttu-id="f6c21-912">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="f6c21-912">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f6c21-913">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="f6c21-913">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f6c21-914">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="f6c21-914">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f6c21-915">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-915">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f6c21-916">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="f6c21-916">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f6c21-917">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="f6c21-917">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-918">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-918">Container</span></span>
* <span data-ttu-id="f6c21-919">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="f6c21-919">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f6c21-920">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-920">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f6c21-921">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-921">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f6c21-922">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-922">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f6c21-923">DataLake</span><span class="sxs-lookup"><span data-stu-id="f6c21-923">Datalake</span></span>
* <span data-ttu-id="f6c21-924">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-924">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f6c21-925">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="f6c21-925">Interactive Shell</span></span>
* <span data-ttu-id="f6c21-926">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-926">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f6c21-927">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="f6c21-927">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-928">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-928">IoT</span></span>
* <span data-ttu-id="f6c21-929">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-929">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6c21-930">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6c21-930">Key Vault</span></span>
* <span data-ttu-id="f6c21-931">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="f6c21-931">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-932">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-932">Network</span></span>
* <span data-ttu-id="f6c21-933">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-933">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f6c21-934">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="f6c21-934">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f6c21-935">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="f6c21-935">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f6c21-936">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-936">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f6c21-937">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-937">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f6c21-938">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-938">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f6c21-939">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-939">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f6c21-940">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="f6c21-940">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f6c21-941">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="f6c21-941">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f6c21-942">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="f6c21-942">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f6c21-943">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="f6c21-943">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f6c21-944">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="f6c21-944">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f6c21-945">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="f6c21-945">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f6c21-946">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="f6c21-946">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f6c21-947">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="f6c21-947">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f6c21-948">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="f6c21-948">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f6c21-949">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-949">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f6c21-950">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="f6c21-950">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-951">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-951">RDBMS</span></span>
* <span data-ttu-id="f6c21-952">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-952">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f6c21-953">Réservation</span><span class="sxs-lookup"><span data-stu-id="f6c21-953">Reservation</span></span>
* <span data-ttu-id="f6c21-954">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="f6c21-954">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f6c21-955">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="f6c21-955">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f6c21-956">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="f6c21-956">Manage App</span></span>
* <span data-ttu-id="f6c21-957">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="f6c21-957">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f6c21-958">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="f6c21-958">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-959">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-959">Role</span></span>
* <span data-ttu-id="f6c21-960">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="f6c21-960">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f6c21-961">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6c21-961">SignalR</span></span>
* <span data-ttu-id="f6c21-962">Première version</span><span class="sxs-lookup"><span data-stu-id="f6c21-962">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-963">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-963">Storage</span></span>
* <span data-ttu-id="f6c21-964">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="f6c21-964">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f6c21-965">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="f6c21-965">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-966">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-966">VM</span></span>
* <span data-ttu-id="f6c21-967">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="f6c21-967">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f6c21-968">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="f6c21-968">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f6c21-969">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-969">August 28, 2018</span></span>

<span data-ttu-id="f6c21-970">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f6c21-970">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-971">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-971">Core</span></span>

* <span data-ttu-id="f6c21-972">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="f6c21-972">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f6c21-973">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f6c21-973">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-974">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-974">ACR</span></span>

* <span data-ttu-id="f6c21-975">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="f6c21-975">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f6c21-976">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="f6c21-976">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-977">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-977">ACS</span></span>

* <span data-ttu-id="f6c21-978">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="f6c21-978">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f6c21-979">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="f6c21-979">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-980">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-980">AppService</span></span>

* <span data-ttu-id="f6c21-981">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="f6c21-981">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f6c21-982">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="f6c21-982">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f6c21-983">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-983">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f6c21-984">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="f6c21-984">Backup</span></span>

* <span data-ttu-id="f6c21-985">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-985">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f6c21-986">Service de robot</span><span class="sxs-lookup"><span data-stu-id="f6c21-986">Bot Service</span></span>

* <span data-ttu-id="f6c21-987">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="f6c21-987">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6c21-988">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-988">Cognitive Services</span></span>

* <span data-ttu-id="f6c21-989">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="f6c21-989">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-990">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-990">IoT</span></span>

* <span data-ttu-id="f6c21-991">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="f6c21-991">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-992">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-992">Monitor</span></span>

* <span data-ttu-id="f6c21-993">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="f6c21-993">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f6c21-994">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="f6c21-994">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-995">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-995">Network</span></span>

* <span data-ttu-id="f6c21-996">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-996">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-997">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-997">Resource</span></span>

* <span data-ttu-id="f6c21-998">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-998">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-999">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-999">Storage</span></span>

* <span data-ttu-id="f6c21-1000">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-1000">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1001">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1001">VM</span></span>

* <span data-ttu-id="f6c21-1002">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-1002">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f6c21-1003">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1003">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f6c21-1004">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1004">Auguest 14, 2018</span></span>

<span data-ttu-id="f6c21-1005">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f6c21-1005">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1006">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1006">Core</span></span>

* <span data-ttu-id="f6c21-1007">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1007">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f6c21-1008">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="f6c21-1008">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f6c21-1009">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1009">Telemetry</span></span>

* <span data-ttu-id="f6c21-1010">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1010">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1011">ACR</span></span>

* <span data-ttu-id="f6c21-1012">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1012">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f6c21-1013">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="f6c21-1013">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1014">ACS</span></span>

* <span data-ttu-id="f6c21-1015">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-1015">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f6c21-1016">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1016">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f6c21-1017">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1017">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f6c21-1018">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1018">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f6c21-1019">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="f6c21-1019">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f6c21-1020">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1020">AppService</span></span>

* <span data-ttu-id="f6c21-1021">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1021">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f6c21-1022">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="f6c21-1022">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f6c21-1023">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1023">BatchAI</span></span>

* <span data-ttu-id="f6c21-1024">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="f6c21-1024">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="f6c21-1025">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1025">Container</span></span>

* <span data-ttu-id="f6c21-1026">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1026">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f6c21-1027">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1027">IoT</span></span>

* <span data-ttu-id="f6c21-1028">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="f6c21-1028">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f6c21-1029">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1029">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6c21-1030">Iot Central</span><span class="sxs-lookup"><span data-stu-id="f6c21-1030">Iot Central</span></span>

* <span data-ttu-id="f6c21-1031">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6c21-1031">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-1032">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-1032">KeyVault</span></span>


* <span data-ttu-id="f6c21-1033">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1033">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f6c21-1034">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1034">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f6c21-1035">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="f6c21-1035">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f6c21-1036">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1036">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f6c21-1037">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1037">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f6c21-1038">Relais</span><span class="sxs-lookup"><span data-stu-id="f6c21-1038">Relay</span></span>

* <span data-ttu-id="f6c21-1039">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1039">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1040">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1040">Sql</span></span>

* <span data-ttu-id="f6c21-1041">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1041">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1042">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1042">Storage</span></span>

* <span data-ttu-id="f6c21-1043">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="f6c21-1043">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f6c21-1044">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1044">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f6c21-1045">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="f6c21-1045">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f6c21-1046">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="f6c21-1046">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f6c21-1047">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1047">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1048">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1048">VM</span></span>

* <span data-ttu-id="f6c21-1049">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1049">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f6c21-1050">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1050">July 31, 2018</span></span>

<span data-ttu-id="f6c21-1051">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f6c21-1051">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1052">ACR</span></span>

* <span data-ttu-id="f6c21-1053">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1053">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f6c21-1054">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1054">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1055">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1055">ACS</span></span>

* <span data-ttu-id="f6c21-1056">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1056">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1057">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1057">Batch</span></span>

* <span data-ttu-id="f6c21-1058">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6c21-1058">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1059">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1059">Container</span></span>

* <span data-ttu-id="f6c21-1060">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="f6c21-1060">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1061">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1061">Network</span></span>

* <span data-ttu-id="f6c21-1062">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f6c21-1062">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f6c21-1063">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1063">Resource</span></span>

* <span data-ttu-id="f6c21-1064">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1064">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f6c21-1065">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1065">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1066">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1066">Role</span></span>

* <span data-ttu-id="f6c21-1067">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1067">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f6c21-1068">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1068">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f6c21-1069">Recherche</span><span class="sxs-lookup"><span data-stu-id="f6c21-1069">Search</span></span>

* <span data-ttu-id="f6c21-1070">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="f6c21-1070">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6c21-1071">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6c21-1071">Service Bus</span></span>

* <span data-ttu-id="f6c21-1072">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="f6c21-1072">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f6c21-1073">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1073">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f6c21-1074">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1074">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f6c21-1075">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1075">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1076">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1076">Storage</span></span>

* <span data-ttu-id="f6c21-1077">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1077">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f6c21-1078">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-1078">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1079">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1079">VM</span></span>

* <span data-ttu-id="f6c21-1080">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1080">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f6c21-1081">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1081">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f6c21-1082">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="f6c21-1082">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f6c21-1083">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="f6c21-1083">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f6c21-1084">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1084">July 18, 2018</span></span>

<span data-ttu-id="f6c21-1085">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f6c21-1085">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1086">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1086">Core</span></span>

* <span data-ttu-id="f6c21-1087">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-1087">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f6c21-1088">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1088">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f6c21-1089">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="f6c21-1089">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1090">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1090">ACR</span></span>

* <span data-ttu-id="f6c21-1091">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="f6c21-1091">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f6c21-1092">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1092">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f6c21-1093">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1093">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f6c21-1094">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="f6c21-1094">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1095">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1095">ACS</span></span>

* <span data-ttu-id="f6c21-1096">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="f6c21-1096">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1097">AppService</span></span>

* <span data-ttu-id="f6c21-1098">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="f6c21-1098">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1099">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1099">Batch</span></span>

* <span data-ttu-id="f6c21-1100">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6c21-1100">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f6c21-1101">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-1101">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6c21-1102">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1102">Batch AI</span></span>

* <span data-ttu-id="f6c21-1103">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1103">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1104">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1104">Container</span></span>

* <span data-ttu-id="f6c21-1105">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="f6c21-1105">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f6c21-1106">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="f6c21-1106">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1107">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1107">Network</span></span>

* <span data-ttu-id="f6c21-1108">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1108">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f6c21-1109">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1109">Added `network nic wait`</span></span>
* <span data-ttu-id="f6c21-1110">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1110">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f6c21-1111">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1111">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f6c21-1112">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1112">Resource</span></span>

* <span data-ttu-id="f6c21-1113">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1113">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f6c21-1114">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1114">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f6c21-1115">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1115">Added `deployment wait` command</span></span>
* <span data-ttu-id="f6c21-1116">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="f6c21-1116">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1117">SQL</span></span>

* <span data-ttu-id="f6c21-1118">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1118">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f6c21-1119">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1119">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f6c21-1120">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1120">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1121">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1121">Storage</span></span>

* <span data-ttu-id="f6c21-1122">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="f6c21-1122">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1123">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1123">VM</span></span>

* <span data-ttu-id="f6c21-1124">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1124">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f6c21-1125">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1125">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f6c21-1126">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1126">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6c21-1127">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1127">July 3, 2018</span></span>

<span data-ttu-id="f6c21-1128">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f6c21-1128">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f6c21-1129">AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1129">AKS</span></span>

* <span data-ttu-id="f6c21-1130">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1130">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6c21-1131">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1131">July 3, 2018</span></span>

<span data-ttu-id="f6c21-1132">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f6c21-1132">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1133">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1133">Core</span></span>

* <span data-ttu-id="f6c21-1134">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1134">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1135">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1135">ACR</span></span>

* <span data-ttu-id="f6c21-1136">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="f6c21-1136">Added polling build status</span></span>
* <span data-ttu-id="f6c21-1137">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-1137">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f6c21-1138">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1138">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1139">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1139">ACS</span></span>

* <span data-ttu-id="f6c21-1140">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1140">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f6c21-1141">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1141">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f6c21-1142">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1142">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f6c21-1143">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1143">Added `--listen-port` support</span></span>
* <span data-ttu-id="f6c21-1144">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1144">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f6c21-1145">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="f6c21-1145">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f6c21-1146">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="f6c21-1146">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1147">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1147">AppService</span></span>

* <span data-ttu-id="f6c21-1148">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1148">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f6c21-1149">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="f6c21-1149">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f6c21-1150">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="f6c21-1150">Backup</span></span>

* <span data-ttu-id="f6c21-1151">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="f6c21-1151">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f6c21-1152">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1152">BatchAI</span></span>

* <span data-ttu-id="f6c21-1153">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1153">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f6c21-1154">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-1154">Cloud</span></span>

* <span data-ttu-id="f6c21-1155">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-1155">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1156">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1156">Container</span></span>

* <span data-ttu-id="f6c21-1157">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="f6c21-1157">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f6c21-1158">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1158">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f6c21-1159">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="f6c21-1159">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1160">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1160">Extension</span></span>

* <span data-ttu-id="f6c21-1161">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1161">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1162">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1162">Network</span></span>

* <span data-ttu-id="f6c21-1163">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f6c21-1163">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-1164">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6c21-1164">Rdbms</span></span>

* <span data-ttu-id="f6c21-1165">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1165">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1166">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1166">Resource</span></span>

* <span data-ttu-id="f6c21-1167">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1167">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1168">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1168">VM</span></span>

* <span data-ttu-id="f6c21-1169">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="f6c21-1169">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f6c21-1170">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1170">June 25, 2018</span></span>

<span data-ttu-id="f6c21-1171">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f6c21-1171">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f6c21-1172">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-1172">CLI</span></span>

* <span data-ttu-id="f6c21-1173">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1173">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f6c21-1174">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1174">June 19, 2018</span></span>

<span data-ttu-id="f6c21-1175">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f6c21-1175">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1176">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1176">Core</span></span>

* <span data-ttu-id="f6c21-1177">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1177">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1178">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1178">ACR</span></span>

* <span data-ttu-id="f6c21-1179">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="f6c21-1179">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f6c21-1180">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1180">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1181">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1181">ACS</span></span>

* <span data-ttu-id="f6c21-1182">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1182">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f6c21-1183">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1183">Added `--update` support</span></span>
* <span data-ttu-id="f6c21-1184">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1184">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f6c21-1185">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1185">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f6c21-1186">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1186">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f6c21-1187">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1187">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f6c21-1188">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1188">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f6c21-1189">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1189">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1190">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1190">AppService</span></span>

* <span data-ttu-id="f6c21-1191">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1191">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f6c21-1192">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1192">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1193">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1193">Batch</span></span>

* <span data-ttu-id="f6c21-1194">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1194">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6c21-1195">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1195">Batch AI</span></span>

* <span data-ttu-id="f6c21-1196">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1196">Added support for workspaces.</span></span> <span data-ttu-id="f6c21-1197">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1197">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f6c21-1198">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1198">Added support for experiments.</span></span> <span data-ttu-id="f6c21-1199">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1199">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f6c21-1200">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="f6c21-1200">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f6c21-1201">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1201">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f6c21-1202">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1202">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f6c21-1203">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1203">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f6c21-1204">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-1204">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f6c21-1205">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="f6c21-1205">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f6c21-1206">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1206">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f6c21-1207">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1207">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f6c21-1208">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1208">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f6c21-1209">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1209">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f6c21-1210">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1210">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f6c21-1211">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1211">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f6c21-1212">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1212">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f6c21-1213">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1213">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f6c21-1214">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1214">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f6c21-1215">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1215">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6c21-1216">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1216">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6c21-1217">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1217">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f6c21-1218">Cartes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1218">Maps</span></span>

* <span data-ttu-id="f6c21-1219">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1219">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1220">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1220">Network</span></span>

* <span data-ttu-id="f6c21-1221">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1221">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f6c21-1222">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1222">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f6c21-1223">#6502</span><span class="sxs-lookup"><span data-stu-id="f6c21-1223">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f6c21-1224">Réservations</span><span class="sxs-lookup"><span data-stu-id="f6c21-1224">Reservations</span></span>

* <span data-ttu-id="f6c21-1225">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1225">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f6c21-1226">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1226">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f6c21-1227">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1227">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f6c21-1228">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1228">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f6c21-1229">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1229">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f6c21-1230">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1230">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1231">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1231">Role</span></span>

* <span data-ttu-id="f6c21-1232">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1232">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1233">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1233">SQL</span></span>

* <span data-ttu-id="f6c21-1234">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1234">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1235">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1235">Storage</span></span>

* <span data-ttu-id="f6c21-1236">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="f6c21-1236">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1237">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1237">VM</span></span>

* <span data-ttu-id="f6c21-1238">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1238">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f6c21-1239">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1239">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f6c21-1240">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="f6c21-1240">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6c21-1241">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1241">June 13, 2018</span></span>

<span data-ttu-id="f6c21-1242">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f6c21-1242">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1243">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1243">Core</span></span>

* <span data-ttu-id="f6c21-1244">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1244">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6c21-1245">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1245">June 13, 2018</span></span>

<span data-ttu-id="f6c21-1246">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f6c21-1246">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f6c21-1247">AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1247">AKS</span></span>

* <span data-ttu-id="f6c21-1248">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1248">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f6c21-1249">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c21-1249">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f6c21-1250">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1250">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f6c21-1251">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1251">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f6c21-1252">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1252">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1253">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1253">AppService</span></span>

* <span data-ttu-id="f6c21-1254">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="f6c21-1254">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6c21-1255">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1255">June 5, 2018</span></span>

<span data-ttu-id="f6c21-1256">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f6c21-1256">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1257">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1257">Interactive</span></span>

* <span data-ttu-id="f6c21-1258">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="f6c21-1258">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6c21-1259">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1259">June 5, 2018</span></span>

<span data-ttu-id="f6c21-1260">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f6c21-1260">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1261">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1261">Core</span></span>

* <span data-ttu-id="f6c21-1262">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="f6c21-1262">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f6c21-1263">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1263">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1264">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1264">ACR</span></span>

* <span data-ttu-id="f6c21-1265">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="f6c21-1265">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f6c21-1266">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1266">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f6c21-1267">AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1267">AKS</span></span>

* <span data-ttu-id="f6c21-1268">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1268">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1269">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1269">Batch</span></span>

* <span data-ttu-id="f6c21-1270">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1270">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-1271">IOT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1271">IOT</span></span>

* <span data-ttu-id="f6c21-1272">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="f6c21-1272">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1273">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1273">Network</span></span>

* <span data-ttu-id="f6c21-1274">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="f6c21-1274">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f6c21-1275">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6c21-1275">Policy Insights</span></span>

* <span data-ttu-id="f6c21-1276">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1276">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f6c21-1277">ARM</span><span class="sxs-lookup"><span data-stu-id="f6c21-1277">ARM</span></span>

* <span data-ttu-id="f6c21-1278">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1278">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1279">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1279">SQL</span></span>

* <span data-ttu-id="f6c21-1280">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1280">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f6c21-1281">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1281">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f6c21-1282">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1282">Storage</span></span>

* <span data-ttu-id="f6c21-1283">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="f6c21-1283">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1284">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1284">VM</span></span>

* <span data-ttu-id="f6c21-1285">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1285">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f6c21-1286">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1286">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f6c21-1287">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1287">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f6c21-1288">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1288">May 22, 2018</span></span>

<span data-ttu-id="f6c21-1289">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f6c21-1289">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1290">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1290">Core</span></span>

* <span data-ttu-id="f6c21-1291">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="f6c21-1291">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1292">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1292">ACS</span></span>

* <span data-ttu-id="f6c21-1293">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1293">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f6c21-1294">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="f6c21-1294">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1295">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1295">AppService</span></span>

* <span data-ttu-id="f6c21-1296">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1296">Improved generic update commands</span></span>
* <span data-ttu-id="f6c21-1297">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1297">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1298">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1298">Container</span></span>

* <span data-ttu-id="f6c21-1299">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="f6c21-1299">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f6c21-1300">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1300">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1301">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1301">Extension</span></span>

* <span data-ttu-id="f6c21-1302">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="f6c21-1302">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1303">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1303">Interactive</span></span>

* <span data-ttu-id="f6c21-1304">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-1304">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f6c21-1305">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="f6c21-1305">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-1306">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-1306">KeyVault</span></span>

* <span data-ttu-id="f6c21-1307">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="f6c21-1307">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1308">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1308">Network</span></span>

* <span data-ttu-id="f6c21-1309">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1309">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f6c21-1310">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1310">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1311">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1311">SQL</span></span>

* <span data-ttu-id="f6c21-1312">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1312">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f6c21-1313">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1313">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f6c21-1314">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1314">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f6c21-1315">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="f6c21-1315">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f6c21-1316">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1316">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f6c21-1317">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1317">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f6c21-1318">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1318">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f6c21-1319">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1319">`edition`.</span></span> <span data-ttu-id="f6c21-1320">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1320">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f6c21-1321">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1321">`elasticPoolName`.</span></span> <span data-ttu-id="f6c21-1322">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1322">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f6c21-1323">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1323">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f6c21-1324">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1324">`edition`.</span></span> <span data-ttu-id="f6c21-1325">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1325">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f6c21-1326">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1326">`dtu`.</span></span> <span data-ttu-id="f6c21-1327">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1327">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f6c21-1328">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1328">`databaseDtuMin`.</span></span> <span data-ttu-id="f6c21-1329">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1329">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f6c21-1330">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1330">`databaseDtuMax`.</span></span> <span data-ttu-id="f6c21-1331">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1331">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f6c21-1332">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1332">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f6c21-1333">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1333">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1334">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1334">Storage</span></span>

* <span data-ttu-id="f6c21-1335">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1335">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f6c21-1336">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1336">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1337">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1337">VM</span></span>

* <span data-ttu-id="f6c21-1338">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1338">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f6c21-1339">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1339">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f6c21-1340">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1340">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f6c21-1341">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1341">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f6c21-1342">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1342">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f6c21-1343">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1343">May 7, 2018</span></span>

<span data-ttu-id="f6c21-1344">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f6c21-1344">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1345">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1345">Core</span></span>

* <span data-ttu-id="f6c21-1346">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="f6c21-1346">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f6c21-1347">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="f6c21-1347">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f6c21-1348">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1348">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f6c21-1349">#5591</span><span class="sxs-lookup"><span data-stu-id="f6c21-1349">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f6c21-1350">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1350">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f6c21-1351">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="f6c21-1351">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f6c21-1352">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1352">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f6c21-1353">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1353">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f6c21-1354">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-1354">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1355">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1355">ACR</span></span>

* <span data-ttu-id="f6c21-1356">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1356">Added ACR Build commands</span></span>
* <span data-ttu-id="f6c21-1357">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="f6c21-1357">Improved resource not found error messages</span></span>
* <span data-ttu-id="f6c21-1358">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1358">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f6c21-1359">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1359">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f6c21-1360">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="f6c21-1360">Improved repository commands error messages</span></span>
* <span data-ttu-id="f6c21-1361">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1361">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1362">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1362">ACS</span></span>

* <span data-ttu-id="f6c21-1363">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-1363">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f6c21-1364">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="f6c21-1364">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f6c21-1365">AMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1365">AMS</span></span>

* <span data-ttu-id="f6c21-1366">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-1366">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1367">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1367">Appservice</span></span>

* <span data-ttu-id="f6c21-1368">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="f6c21-1368">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f6c21-1369">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1369">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f6c21-1370">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="f6c21-1370">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f6c21-1371">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1371">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6c21-1372">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1372">Batch AI</span></span>

* <span data-ttu-id="f6c21-1373">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="f6c21-1373">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6c21-1374">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-1374">Cognitive Services</span></span>

* <span data-ttu-id="f6c21-1375">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1375">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-1376">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1376">Consumption</span></span>

* <span data-ttu-id="f6c21-1377">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="f6c21-1377">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1378">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1378">Container</span></span>

* <span data-ttu-id="f6c21-1379">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="f6c21-1379">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6c21-1380">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6c21-1380">Cosmos DB</span></span>

* <span data-ttu-id="f6c21-1381">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6c21-1381">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f6c21-1382">DMS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1382">DMS</span></span>

* <span data-ttu-id="f6c21-1383">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="f6c21-1383">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1384">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1384">Extension</span></span>

* <span data-ttu-id="f6c21-1385">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1385">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1386">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1386">Interactive</span></span>

* <span data-ttu-id="f6c21-1387">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="f6c21-1387">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f6c21-1388">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="f6c21-1388">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f6c21-1389">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="f6c21-1389">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f6c21-1390">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1390">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f6c21-1391">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-1391">Lab</span></span>

* <span data-ttu-id="f6c21-1392">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="f6c21-1392">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1393">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1393">Network</span></span>

* <span data-ttu-id="f6c21-1394">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1394">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f6c21-1395">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1395">Profile</span></span>

* <span data-ttu-id="f6c21-1396">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1396">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f6c21-1397">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1397">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f6c21-1398">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1398">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f6c21-1399">Redis</span><span class="sxs-lookup"><span data-stu-id="f6c21-1399">Redis</span></span>

* <span data-ttu-id="f6c21-1400">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1400">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f6c21-1401">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1401">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f6c21-1402">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1402">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f6c21-1403">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1403">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f6c21-1404">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1404">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1405">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1405">Role</span></span>

* <span data-ttu-id="f6c21-1406">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="f6c21-1406">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1407">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1407">Storage</span></span>

* <span data-ttu-id="f6c21-1408">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1408">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f6c21-1409">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="f6c21-1409">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f6c21-1410">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1410">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f6c21-1411">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="f6c21-1411">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f6c21-1412">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1412">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1413">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1413">VM</span></span>

* <span data-ttu-id="f6c21-1414">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="f6c21-1414">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f6c21-1415">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1415">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f6c21-1416">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1416">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f6c21-1417">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1417">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f6c21-1418">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1418">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f6c21-1419">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="f6c21-1419">Added write accelerator support</span></span>
* <span data-ttu-id="f6c21-1420">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1420">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f6c21-1421">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1421">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f6c21-1422">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="f6c21-1422">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f6c21-1423">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1423">April 10, 2018</span></span>

<span data-ttu-id="f6c21-1424">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f6c21-1424">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1425">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1425">ACR</span></span>

* <span data-ttu-id="f6c21-1426">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="f6c21-1426">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1427">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1427">ACS</span></span>

* <span data-ttu-id="f6c21-1428">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="f6c21-1428">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1429">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1429">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f6c21-1431">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="f6c21-1431">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f6c21-1432">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1432">BatchAI</span></span>

* <span data-ttu-id="f6c21-1433">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="f6c21-1433">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f6c21-1434">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-1434">Job level mounting</span></span>
  - <span data-ttu-id="f6c21-1435">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="f6c21-1435">Environment variables with secret values</span></span>
  - <span data-ttu-id="f6c21-1436">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="f6c21-1436">Performance counters settings</span></span>
  - <span data-ttu-id="f6c21-1437">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-1437">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f6c21-1438">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="f6c21-1438">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f6c21-1439">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="f6c21-1439">Usage and limits reporting</span></span>
  - <span data-ttu-id="f6c21-1440">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1440">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f6c21-1441">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1441">Support for custom images</span></span>
  - <span data-ttu-id="f6c21-1442">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1442">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f6c21-1443">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-1443">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f6c21-1444">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="f6c21-1444">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f6c21-1445">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="f6c21-1445">National clouds are supported</span></span>
* <span data-ttu-id="f6c21-1446">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="f6c21-1446">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f6c21-1447">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="f6c21-1447">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f6c21-1448">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1448">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f6c21-1449">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1449">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f6c21-1450">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1450">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f6c21-1451">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1451">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f6c21-1452">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1452">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f6c21-1453">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1453">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f6c21-1454">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="f6c21-1454">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f6c21-1455">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1455">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f6c21-1456">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-1456">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f6c21-1457">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1457">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f6c21-1458">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1458">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f6c21-1459">Facturation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1459">Billing</span></span>

* <span data-ttu-id="f6c21-1460">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="f6c21-1460">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-1461">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1461">Consumption</span></span>

* <span data-ttu-id="f6c21-1462">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1462">Added `marketplace` commands</span></span>
* <span data-ttu-id="f6c21-1463">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1463">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f6c21-1464">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1464">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f6c21-1465">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1465">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f6c21-1466">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1466">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f6c21-1467">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1467">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1468">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1468">Container</span></span>

* <span data-ttu-id="f6c21-1469">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1469">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f6c21-1470">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="f6c21-1470">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1471">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1471">Extension</span></span>

* <span data-ttu-id="f6c21-1472">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1472">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1473">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1473">Interactive</span></span>

* <span data-ttu-id="f6c21-1474">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="f6c21-1474">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f6c21-1475">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-1475">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f6c21-1476">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1476">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1477">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1477">Network</span></span>

* <span data-ttu-id="f6c21-1478">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="f6c21-1478">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f6c21-1479">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1479">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f6c21-1480">#4910</span><span class="sxs-lookup"><span data-stu-id="f6c21-1480">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f6c21-1481">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1481">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f6c21-1482">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1482">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f6c21-1483">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1483">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f6c21-1484">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1484">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f6c21-1485">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1485">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-1486">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1486">Profile</span></span>

* <span data-ttu-id="f6c21-1487">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1487">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f6c21-1488">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1488">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-1489">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1489">RDBMS</span></span>

* <span data-ttu-id="f6c21-1490">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1490">Added `georestore` command</span></span>
* <span data-ttu-id="f6c21-1491">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1491">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1492">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1492">Resource</span></span>

* <span data-ttu-id="f6c21-1493">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1493">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f6c21-1494">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1494">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1495">SQL</span></span>

* <span data-ttu-id="f6c21-1496">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1496">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1497">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1497">Storage</span></span>

* <span data-ttu-id="f6c21-1498">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1498">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1499">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1499">VM</span></span>

* <span data-ttu-id="f6c21-1500">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1500">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f6c21-1501">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1501">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f6c21-1503">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1503">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f6c21-1504">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1504">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f6c21-1505">#5718</span><span class="sxs-lookup"><span data-stu-id="f6c21-1505">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f6c21-1506">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="f6c21-1506">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f6c21-1507">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1507">March 27, 2018</span></span>

<span data-ttu-id="f6c21-1508">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f6c21-1508">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1509">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1509">Core</span></span>

* <span data-ttu-id="f6c21-1510">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="f6c21-1510">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1511">ACS</span></span>

* <span data-ttu-id="f6c21-1512">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6c21-1512">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1513">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1513">Appservice</span></span>

* <span data-ttu-id="f6c21-1514">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1514">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f6c21-1515">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1515">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6c21-1516">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="f6c21-1516">Backup</span></span>

* <span data-ttu-id="f6c21-1517">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1517">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f6c21-1518">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1518">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f6c21-1519">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1519">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f6c21-1520">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1520">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1521">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1521">Container</span></span>

* <span data-ttu-id="f6c21-1522">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1522">Added `container exec` command.</span></span> <span data-ttu-id="f6c21-1523">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1523">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f6c21-1524">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1524">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1525">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1525">Extension</span></span>

* <span data-ttu-id="f6c21-1526">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-1526">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f6c21-1527">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1527">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f6c21-1528">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1528">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1529">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1529">Interactive</span></span>

* <span data-ttu-id="f6c21-1530">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-1530">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f6c21-1531">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1531">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f6c21-1532">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="f6c21-1532">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f6c21-1533">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="f6c21-1533">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f6c21-1534">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-1534">Lab</span></span>

* <span data-ttu-id="f6c21-1535">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1535">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1536">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1536">Monitor</span></span>

* <span data-ttu-id="f6c21-1537">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1537">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f6c21-1538">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="f6c21-1538">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f6c21-1539">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1539">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1540">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1540">Network</span></span>

* <span data-ttu-id="f6c21-1541">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="f6c21-1541">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-1542">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1542">Profile</span></span>

* <span data-ttu-id="f6c21-1543">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1543">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-1544">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1544">RDBMS</span></span>

* <span data-ttu-id="f6c21-1545">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="f6c21-1545">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1546">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1546">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f6c21-1548">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1548">Role</span></span>

* <span data-ttu-id="f6c21-1549">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1549">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f6c21-1550">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="f6c21-1550">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f6c21-1551">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1551">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f6c21-1552">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1552">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f6c21-1553">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1553">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1554">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1554">Storage</span></span>

* <span data-ttu-id="f6c21-1555">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="f6c21-1555">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f6c21-1556">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="f6c21-1556">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1557">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1557">VM</span></span>

* <span data-ttu-id="f6c21-1558">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="f6c21-1558">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f6c21-1559">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1559">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f6c21-1560">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1560">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f6c21-1561">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1561">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f6c21-1562">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1562">March 13, 2018</span></span>

<span data-ttu-id="f6c21-1563">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f6c21-1563">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1564">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1564">ACR</span></span>

* <span data-ttu-id="f6c21-1565">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1565">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f6c21-1566">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1566">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f6c21-1567">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="f6c21-1567">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1568">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1568">ACS</span></span>

* <span data-ttu-id="f6c21-1569">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="f6c21-1569">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f6c21-1570">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="f6c21-1570">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f6c21-1571">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6c21-1571">Advisor</span></span>

* <span data-ttu-id="f6c21-1572">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1572">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f6c21-1573">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1573">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f6c21-1574">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1574">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f6c21-1575">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1575">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f6c21-1576">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1576">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1577">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1577">Appservice</span></span>

* <span data-ttu-id="f6c21-1578">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="f6c21-1578">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f6c21-1579">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1579">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6c21-1580">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1580">Eventhubs</span></span>

* <span data-ttu-id="f6c21-1581">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1581">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1582">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1582">Extension</span></span>

* <span data-ttu-id="f6c21-1583">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1583">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1584">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1584">Interactive</span></span>

* <span data-ttu-id="f6c21-1585">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="f6c21-1585">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f6c21-1586">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="f6c21-1586">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f6c21-1587">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="f6c21-1587">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f6c21-1588">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="f6c21-1588">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1589">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1589">Monitor</span></span>

* <span data-ttu-id="f6c21-1590">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1590">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f6c21-1591">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1591">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f6c21-1592">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1592">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f6c21-1593">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1593">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1594">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1594">Network</span></span>

* <span data-ttu-id="f6c21-1595">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1595">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f6c21-1596">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1596">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f6c21-1597">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1597">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f6c21-1598">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1598">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-1599">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1599">Profile</span></span>

* <span data-ttu-id="f6c21-1600">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1600">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f6c21-1601">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1601">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-1602">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1602">RDBMS</span></span>

* <span data-ttu-id="f6c21-1603">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-1603">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6c21-1604">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6c21-1604">Service Bus</span></span>

* <span data-ttu-id="f6c21-1605">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1605">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1606">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1606">Storage</span></span>

* <span data-ttu-id="f6c21-1607">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="f6c21-1607">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f6c21-1608">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="f6c21-1608">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1609">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1609">VM</span></span>

* <span data-ttu-id="f6c21-1610">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="f6c21-1610">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f6c21-1611">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1611">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f6c21-1612">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1612">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f6c21-1613">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="f6c21-1613">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f6c21-1614">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1614">February 27, 2018</span></span>

<span data-ttu-id="f6c21-1615">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f6c21-1615">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1616">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1616">Core</span></span>

* <span data-ttu-id="f6c21-1617">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="f6c21-1617">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f6c21-1618">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1618">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f6c21-1619">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1619">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1620">ACS</span></span>

* <span data-ttu-id="f6c21-1621">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1621">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f6c21-1622">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1622">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f6c21-1623">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1623">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f6c21-1624">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1624">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1625">Appservice</span></span>

* <span data-ttu-id="f6c21-1626">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1626">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f6c21-1627">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="f6c21-1627">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6c21-1628">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-1628">Cognitive Services</span></span>

* <span data-ttu-id="f6c21-1629">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-1629">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-1630">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1630">Consumption</span></span>

* <span data-ttu-id="f6c21-1631">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="f6c21-1631">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f6c21-1632">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1632">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1633">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1633">Container</span></span>

* <span data-ttu-id="f6c21-1634">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1634">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1635">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1635">Network</span></span>

* <span data-ttu-id="f6c21-1636">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1636">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1637">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1637">Resource</span></span>

* <span data-ttu-id="f6c21-1638">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="f6c21-1638">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1639">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1639">Role</span></span>

* <span data-ttu-id="f6c21-1640">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="f6c21-1640">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1641">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1641">SQL</span></span>

* <span data-ttu-id="f6c21-1642">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="f6c21-1642">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1643">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1643">Storage</span></span>

* <span data-ttu-id="f6c21-1644">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1644">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1645">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1645">VM</span></span>

* <span data-ttu-id="f6c21-1646">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="f6c21-1646">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f6c21-1647">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1647">February 13, 2018</span></span>

<span data-ttu-id="f6c21-1648">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f6c21-1648">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1649">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1649">Core</span></span>

* <span data-ttu-id="f6c21-1650">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1650">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1651">ACS</span></span>

* <span data-ttu-id="f6c21-1652">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="f6c21-1652">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f6c21-1653">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1653">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f6c21-1654">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1654">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f6c21-1655">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1655">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f6c21-1656">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="f6c21-1656">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f6c21-1657">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1657">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f6c21-1658">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1658">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f6c21-1659">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1659">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1660">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1660">Appservice</span></span>

* <span data-ttu-id="f6c21-1661">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="f6c21-1661">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f6c21-1662">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1662">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-1663">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-1663">CDN</span></span>

* <span data-ttu-id="f6c21-1664">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1664">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1665">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1665">Container</span></span>

* <span data-ttu-id="f6c21-1666">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="f6c21-1666">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f6c21-1667">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1667">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-1668">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-1668">CosmosDB</span></span>

* <span data-ttu-id="f6c21-1669">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="f6c21-1669">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1670">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1670">Extension</span></span>

* <span data-ttu-id="f6c21-1671">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1671">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f6c21-1672">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1672">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f6c21-1673">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f6c21-1673">Feedback</span></span>

* <span data-ttu-id="f6c21-1674">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1674">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1675">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1675">Interactive</span></span>

* <span data-ttu-id="f6c21-1676">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6c21-1676">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f6c21-1677">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="f6c21-1677">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-1678">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1678">IoT</span></span>

* <span data-ttu-id="f6c21-1679">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="f6c21-1679">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6c21-1680">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="f6c21-1680">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6c21-1681">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1681">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f6c21-1682">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="f6c21-1682">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1683">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1683">Monitor</span></span>

* <span data-ttu-id="f6c21-1684">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1684">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1685">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1685">Network</span></span>

* <span data-ttu-id="f6c21-1686">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1686">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f6c21-1687">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1687">Profile</span></span>

* <span data-ttu-id="f6c21-1688">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="f6c21-1688">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1689">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1689">Resource</span></span>

* <span data-ttu-id="f6c21-1690">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1690">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1691">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1691">Role</span></span>

* <span data-ttu-id="f6c21-1692">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1692">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1693">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1693">SQL</span></span>

* <span data-ttu-id="f6c21-1694">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1694">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f6c21-1695">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1695">Added `sql db rename`</span></span>
* <span data-ttu-id="f6c21-1696">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="f6c21-1696">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1697">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1697">Storage</span></span>

* <span data-ttu-id="f6c21-1698">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="f6c21-1698">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1699">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1699">VM</span></span>

* <span data-ttu-id="f6c21-1700">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1700">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f6c21-1701">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1701">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f6c21-1702">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="f6c21-1702">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f6c21-1703">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1703">January 31, 2018</span></span>

<span data-ttu-id="f6c21-1704">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f6c21-1704">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1705">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1705">Core</span></span>

* <span data-ttu-id="f6c21-1706">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1706">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f6c21-1707">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-1707">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f6c21-1708">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1708">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f6c21-1709">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="f6c21-1709">Use `--verbose` to see</span></span>
* <span data-ttu-id="f6c21-1710">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="f6c21-1710">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1711">ACS</span></span>

* <span data-ttu-id="f6c21-1712">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1712">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f6c21-1713">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1713">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1714">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1714">Appservice</span></span>

* <span data-ttu-id="f6c21-1715">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="f6c21-1715">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f6c21-1716">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="f6c21-1716">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-1717">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-1717">CDN</span></span>

* <span data-ttu-id="f6c21-1718">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1718">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-1719">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-1719">CosmosDB</span></span>

* <span data-ttu-id="f6c21-1720">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1720">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1721">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1721">Interactive</span></span>

* <span data-ttu-id="f6c21-1722">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="f6c21-1722">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1723">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1723">Network</span></span>

* <span data-ttu-id="f6c21-1724">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1724">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f6c21-1725">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1725">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f6c21-1726">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1726">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f6c21-1727">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1727">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f6c21-1728">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1728">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f6c21-1729">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="f6c21-1729">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f6c21-1730">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1730">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f6c21-1731">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1731">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f6c21-1732">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1732">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f6c21-1733">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1733">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-1734">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1734">Profile</span></span>

* <span data-ttu-id="f6c21-1735">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="f6c21-1735">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1736">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1736">Resource</span></span>

* <span data-ttu-id="f6c21-1737">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="f6c21-1737">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1738">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1738">Storage</span></span>

* <span data-ttu-id="f6c21-1739">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="f6c21-1739">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f6c21-1740">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1740">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f6c21-1741">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1741">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f6c21-1742">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1742">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f6c21-1743">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="f6c21-1743">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1744">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1744">VM</span></span>

* <span data-ttu-id="f6c21-1745">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="f6c21-1745">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f6c21-1746">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="f6c21-1746">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f6c21-1747">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="f6c21-1747">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f6c21-1748">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1748">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f6c21-1749">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="f6c21-1749">January 17, 2018</span></span>

<span data-ttu-id="f6c21-1750">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f6c21-1750">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1751">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1751">ACR</span></span>

* <span data-ttu-id="f6c21-1752">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-1752">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f6c21-1753">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="f6c21-1753">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1754">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1754">ACS</span></span>

* <span data-ttu-id="f6c21-1755">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1755">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f6c21-1756">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="f6c21-1756">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1757">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1757">Appservice</span></span>

* <span data-ttu-id="f6c21-1758">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="f6c21-1758">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f6c21-1759">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1759">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f6c21-1760">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1760">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f6c21-1761">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="f6c21-1761">Backup</span></span>

* <span data-ttu-id="f6c21-1762">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="f6c21-1762">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f6c21-1763">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1763">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f6c21-1764">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-1764">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f6c21-1765">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="f6c21-1765">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f6c21-1766">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1766">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1767">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1767">Batch</span></span>

* <span data-ttu-id="f6c21-1768">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="f6c21-1768">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f6c21-1769">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-1769">Cloud</span></span>

* <span data-ttu-id="f6c21-1770">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-1770">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-1771">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1771">Consumption</span></span>

* <span data-ttu-id="f6c21-1772">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1772">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6c21-1773">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6c21-1773">Event Grid</span></span>

* <span data-ttu-id="f6c21-1774">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1774">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6c21-1775">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1775">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6c21-1776">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1776">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f6c21-1777">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="f6c21-1777">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f6c21-1778">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1778">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f6c21-1779">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1779">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f6c21-1780">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1780">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f6c21-1781">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1781">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-1782">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-1782">Interactive</span></span>

* <span data-ttu-id="f6c21-1783">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="f6c21-1783">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f6c21-1784">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1784">Fixed errors on startup</span></span>
* <span data-ttu-id="f6c21-1785">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="f6c21-1785">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-1786">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1786">IoT</span></span>

* <span data-ttu-id="f6c21-1787">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="f6c21-1787">Added support for device provisioning service</span></span>
* <span data-ttu-id="f6c21-1788">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1788">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f6c21-1789">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1789">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1790">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1790">Monitor</span></span>

* <span data-ttu-id="f6c21-1791">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1791">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f6c21-1792">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1792">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f6c21-1793">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="f6c21-1793">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1794">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1794">Network</span></span>

* <span data-ttu-id="f6c21-1795">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1795">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f6c21-1796">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1796">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-1797">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-1797">Profile</span></span>

* <span data-ttu-id="f6c21-1798">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1798">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1799">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1799">Role</span></span>

* <span data-ttu-id="f6c21-1800">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1800">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6c21-1801">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6c21-1801">Service Fabric</span></span>

* <span data-ttu-id="f6c21-1802">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="f6c21-1802">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f6c21-1803">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1803">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1804">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1804">VM</span></span>

* <span data-ttu-id="f6c21-1805">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1805">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f6c21-1806">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="f6c21-1806">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f6c21-1807">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1807">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f6c21-1808">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1808">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f6c21-1809">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="f6c21-1809">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f6c21-1810">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1810">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6c21-1811">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1811">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6c21-1812">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1812">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f6c21-1813">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1813">December 19, 2017</span></span>

<span data-ttu-id="f6c21-1814">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f6c21-1814">Version 2.0.23</span></span>

* <span data-ttu-id="f6c21-1815">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1815">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1816">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1816">Container</span></span>

* <span data-ttu-id="f6c21-1817">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1817">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1818">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1818">Network</span></span>

* <span data-ttu-id="f6c21-1819">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1819">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f6c21-1820">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1820">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1821">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1821">Storage</span></span>

* <span data-ttu-id="f6c21-1822">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="f6c21-1822">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1823">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1823">VM</span></span>

* <span data-ttu-id="f6c21-1824">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1824">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f6c21-1825">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1825">December 5, 2017</span></span>

<span data-ttu-id="f6c21-1826">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f6c21-1826">Version 2.0.22</span></span>

* <span data-ttu-id="f6c21-1827">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1827">Removed `az component` commands.</span></span> <span data-ttu-id="f6c21-1828">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="f6c21-1828">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1829">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1829">Core</span></span>
* <span data-ttu-id="f6c21-1830">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="f6c21-1830">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f6c21-1831">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1831">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1832">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1832">ACS</span></span>

* <span data-ttu-id="f6c21-1833">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1833">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f6c21-1834">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1834">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f6c21-1835">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="f6c21-1835">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f6c21-1836">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6c21-1836">Advisor</span></span>

* <span data-ttu-id="f6c21-1837">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1837">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1838">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1838">Appservice</span></span>

* <span data-ttu-id="f6c21-1839">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1839">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f6c21-1840">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1840">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f6c21-1841">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1841">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f6c21-1842">Consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1842">Consumption</span></span>

* <span data-ttu-id="f6c21-1843">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="f6c21-1843">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1844">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1844">Container</span></span>

* <span data-ttu-id="f6c21-1845">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1845">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1846">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1846">Monitor</span></span>

* <span data-ttu-id="f6c21-1847">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="f6c21-1847">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1848">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1848">Resource</span></span>

* <span data-ttu-id="f6c21-1849">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1849">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-1850">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1850">Role</span></span>

* <span data-ttu-id="f6c21-1851">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1851">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f6c21-1852">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1852">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f6c21-1853">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1853">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1854">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1854">SQL</span></span>

* <span data-ttu-id="f6c21-1855">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1855">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f6c21-1856">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1856">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1857">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1857">VM</span></span>

* <span data-ttu-id="f6c21-1858">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1858">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f6c21-1859">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1859">November 14, 2017</span></span>

<span data-ttu-id="f6c21-1860">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f6c21-1860">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1861">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1861">ACR</span></span>

* <span data-ttu-id="f6c21-1862">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="f6c21-1862">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f6c21-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1863">ACS</span></span>

* <span data-ttu-id="f6c21-1864">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1864">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f6c21-1865">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1865">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f6c21-1866">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1866">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f6c21-1867">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-1867">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f6c21-1868">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="f6c21-1868">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1869">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1869">Appservice</span></span>

* <span data-ttu-id="f6c21-1870">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="f6c21-1870">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f6c21-1871">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1871">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f6c21-1872">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1872">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f6c21-1873">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1873">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f6c21-1874">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="f6c21-1874">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f6c21-1875">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="f6c21-1875">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1876">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1876">Batch</span></span>

* <span data-ttu-id="f6c21-1877">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1877">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f6c21-1878">Batchai</span><span class="sxs-lookup"><span data-stu-id="f6c21-1878">Batchai</span></span>

* <span data-ttu-id="f6c21-1879">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1879">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f6c21-1880">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1880">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f6c21-1881">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1881">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f6c21-1882">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1882">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f6c21-1883">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-1883">Cloud</span></span>

* <span data-ttu-id="f6c21-1884">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="f6c21-1884">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-1885">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-1885">Container</span></span>

* <span data-ttu-id="f6c21-1886">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="f6c21-1886">Added support to open multiple ports</span></span>
* <span data-ttu-id="f6c21-1887">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="f6c21-1887">Added container group restart policy</span></span>
* <span data-ttu-id="f6c21-1888">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="f6c21-1888">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f6c21-1889">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="f6c21-1889">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6c21-1890">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6c21-1890">Data Lake Analytics</span></span>

* <span data-ttu-id="f6c21-1891">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="f6c21-1891">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6c21-1892">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-1892">Data Lake Store</span></span>

* <span data-ttu-id="f6c21-1893">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="f6c21-1893">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-1894">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-1894">Extension</span></span>

* <span data-ttu-id="f6c21-1895">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6c21-1895">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f6c21-1896">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="f6c21-1896">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-1897">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-1897">IoT</span></span>

* <span data-ttu-id="f6c21-1898">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1898">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1899">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1899">Monitor</span></span>

* <span data-ttu-id="f6c21-1900">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1900">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1901">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1901">Network</span></span>

* <span data-ttu-id="f6c21-1902">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="f6c21-1902">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f6c21-1903">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1903">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f6c21-1904">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-1904">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f6c21-1905">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1905">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f6c21-1906">Réservations</span><span class="sxs-lookup"><span data-stu-id="f6c21-1906">Reservations</span></span>

* <span data-ttu-id="f6c21-1907">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-1907">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1908">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1908">Resource</span></span>

* <span data-ttu-id="f6c21-1909">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="f6c21-1909">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1910">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1910">SQL</span></span>

* <span data-ttu-id="f6c21-1911">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1911">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1912">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1912">Storage</span></span>

* <span data-ttu-id="f6c21-1913">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-1913">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f6c21-1914">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="f6c21-1914">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f6c21-1915">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1915">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f6c21-1916">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1916">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f6c21-1917">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1917">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f6c21-1918">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1918">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f6c21-1919">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1919">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1920">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1920">VM</span></span>

* <span data-ttu-id="f6c21-1921">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1921">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f6c21-1922">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1922">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f6c21-1923">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="f6c21-1923">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f6c21-1924">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1924">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f6c21-1925">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1925">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f6c21-1926">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1926">October 24, 2017</span></span>

<span data-ttu-id="f6c21-1927">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f6c21-1927">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1928">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1928">Core</span></span>

* <span data-ttu-id="f6c21-1929">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1929">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-1930">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-1930">ACR</span></span>

* <span data-ttu-id="f6c21-1931">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1931">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f6c21-1932">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="f6c21-1932">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f6c21-1933">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="f6c21-1933">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-1934">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-1934">ACS</span></span>

* <span data-ttu-id="f6c21-1935">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1935">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f6c21-1936">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1936">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1937">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1937">Appservice</span></span>

* <span data-ttu-id="f6c21-1938">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="f6c21-1938">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f6c21-1939">Composant</span><span class="sxs-lookup"><span data-stu-id="f6c21-1939">Component</span></span>

* <span data-ttu-id="f6c21-1940">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="f6c21-1940">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-1941">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-1941">Monitor</span></span>

* <span data-ttu-id="f6c21-1942">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1942">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1943">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1943">Resource</span></span>

* <span data-ttu-id="f6c21-1944">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1944">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f6c21-1945">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1945">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1946">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1946">VM</span></span>

* <span data-ttu-id="f6c21-1947">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1947">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f6c21-1948">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1948">October 9, 2017</span></span>

<span data-ttu-id="f6c21-1949">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f6c21-1949">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-1950">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-1950">Core</span></span>

* <span data-ttu-id="f6c21-1951">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f6c21-1951">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-1952">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-1952">Appservice</span></span>

* <span data-ttu-id="f6c21-1953">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1953">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-1954">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1954">Batch</span></span>

* <span data-ttu-id="f6c21-1955">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f6c21-1955">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f6c21-1956">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="f6c21-1956">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f6c21-1957">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-1957">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f6c21-1958">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="f6c21-1958">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f6c21-1959">Batchai</span><span class="sxs-lookup"><span data-stu-id="f6c21-1959">Batchai</span></span>

* <span data-ttu-id="f6c21-1960">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6c21-1960">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-1961">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-1961">Keyvault</span></span>

* <span data-ttu-id="f6c21-1962">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f6c21-1962">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f6c21-1963">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f6c21-1963">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f6c21-1964">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1964">Network</span></span>

* <span data-ttu-id="f6c21-1965">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="f6c21-1965">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f6c21-1966">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1966">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1967">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1967">Resource</span></span>

* <span data-ttu-id="f6c21-1968">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1968">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f6c21-1969">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-1969">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f6c21-1970">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="f6c21-1970">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f6c21-1971">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="f6c21-1971">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-1972">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-1972">Sql</span></span>

* <span data-ttu-id="f6c21-1973">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="f6c21-1973">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f6c21-1974">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="f6c21-1974">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f6c21-1975">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="f6c21-1975">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1976">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1976">Storage</span></span>

* <span data-ttu-id="f6c21-1977">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="f6c21-1977">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-1978">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-1978">Vm</span></span>

* <span data-ttu-id="f6c21-1979">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="f6c21-1979">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f6c21-1980">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1980">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f6c21-1981">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1981">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f6c21-1982">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1982">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f6c21-1983">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1983">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f6c21-1984">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-1984">September 22, 2017</span></span>

<span data-ttu-id="f6c21-1985">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f6c21-1985">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-1986">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-1986">Resource</span></span>

* <span data-ttu-id="f6c21-1987">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="f6c21-1987">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f6c21-1988">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="f6c21-1988">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f6c21-1989">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1989">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f6c21-1990">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1990">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-1991">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-1991">Network</span></span>

* <span data-ttu-id="f6c21-1992">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1992">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f6c21-1993">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1993">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f6c21-1994">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1994">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f6c21-1995">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1995">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f6c21-1996">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1996">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6c21-1997">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1997">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f6c21-1998">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-1998">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-1999">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-1999">Storage</span></span>

* <span data-ttu-id="f6c21-2000">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2000">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6c21-2001">Événement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2001">Eventgrid</span></span>

* <span data-ttu-id="f6c21-2002">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="f6c21-2002">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-2003">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-2003">SQL</span></span>

* <span data-ttu-id="f6c21-2004">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2004">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f6c21-2005">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2005">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f6c21-2006">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2006">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-2007">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-2007">Keyvault</span></span>

* <span data-ttu-id="f6c21-2008">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="f6c21-2008">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2009">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2009">VM</span></span>

* <span data-ttu-id="f6c21-2010">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2010">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f6c21-2011">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="f6c21-2011">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f6c21-2012">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2012">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f6c21-2013">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2013">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f6c21-2014">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2014">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f6c21-2015">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2015">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2016">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2016">ACS</span></span>

* <span data-ttu-id="f6c21-2017">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-2017">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2018">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2018">Appservice</span></span>

* <span data-ttu-id="f6c21-2019">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2019">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6c21-2020">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="f6c21-2020">Backup</span></span>

* <span data-ttu-id="f6c21-2021">Préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-2021">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f6c21-2022">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2022">September 11, 2017</span></span>

<span data-ttu-id="f6c21-2023">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f6c21-2023">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f6c21-2024">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-2024">Core</span></span>

* <span data-ttu-id="f6c21-2025">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="f6c21-2025">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f6c21-2026">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="f6c21-2026">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2027">Acs</span><span class="sxs-lookup"><span data-stu-id="f6c21-2027">Acs</span></span>

* <span data-ttu-id="f6c21-2028">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2028">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f6c21-2029">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="f6c21-2029">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2030">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2030">Appservice</span></span>

* <span data-ttu-id="f6c21-2031">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="f6c21-2031">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-2032">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-2032">CDN</span></span>

* <span data-ttu-id="f6c21-2033">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2033">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f6c21-2034">Extension</span><span class="sxs-lookup"><span data-stu-id="f6c21-2034">Extension</span></span>

* <span data-ttu-id="f6c21-2035">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-2035">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-2036">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-2036">Keyvault</span></span>

* <span data-ttu-id="f6c21-2037">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2037">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-2038">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2038">Network</span></span>

* <span data-ttu-id="f6c21-2039">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2039">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6c21-2040">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2040">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f6c21-2041">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2041">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f6c21-2042">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2042">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6c21-2043">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2043">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-2044">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-2044">Resource</span></span>

* <span data-ttu-id="f6c21-2045">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2045">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f6c21-2046">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2046">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f6c21-2047">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="f6c21-2047">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f6c21-2048">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="f6c21-2048">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-2049">SQL</span></span>

* <span data-ttu-id="f6c21-2050">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2050">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2051">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2051">VM</span></span>

* <span data-ttu-id="f6c21-2052">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="f6c21-2052">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f6c21-2053">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="f6c21-2053">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f6c21-2054">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2054">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f6c21-2055">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="f6c21-2055">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f6c21-2056">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="f6c21-2056">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f6c21-2057">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2057">August 31, 2017</span></span>

<span data-ttu-id="f6c21-2058">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f6c21-2058">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-2059">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-2059">Keyvault</span></span>

* <span data-ttu-id="f6c21-2060">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2060">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f6c21-2061">Sf</span><span class="sxs-lookup"><span data-stu-id="f6c21-2061">Sf</span></span>

* <span data-ttu-id="f6c21-2062">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2062">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-2063">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2063">Storage</span></span>

* <span data-ttu-id="f6c21-2064">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="f6c21-2064">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f6c21-2065">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2065">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f6c21-2066">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2066">August 28, 2017</span></span>

<span data-ttu-id="f6c21-2067">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f6c21-2067">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f6c21-2068">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-2068">CLI</span></span>

* <span data-ttu-id="f6c21-2069">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2069">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2070">ACS</span></span>

* <span data-ttu-id="f6c21-2071">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="f6c21-2071">Corrected preview regions</span></span>
* <span data-ttu-id="f6c21-2072">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2072">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f6c21-2073">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2073">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2074">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2074">Appservice</span></span>

* <span data-ttu-id="f6c21-2075">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2075">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f6c21-2076">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2076">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f6c21-2077">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2077">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f6c21-2078">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2078">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f6c21-2079">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2079">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-2080">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-2080">IoT</span></span>

* <span data-ttu-id="f6c21-2081">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="f6c21-2081">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-2082">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2082">Network</span></span>

* <span data-ttu-id="f6c21-2083">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2083">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6c21-2084">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2084">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f6c21-2085">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2085">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6c21-2086">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2086">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6c21-2087">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2087">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-2088">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-2088">Profile</span></span>

* <span data-ttu-id="f6c21-2089">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2089">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6c21-2090">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6c21-2090">Service Fabric</span></span>

* <span data-ttu-id="f6c21-2091">Préversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-2091">Preview release</span></span>
* <span data-ttu-id="f6c21-2092">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-2092">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f6c21-2093">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="f6c21-2093">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f6c21-2094">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2094">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-2095">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2095">Storage</span></span>

* <span data-ttu-id="f6c21-2096">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="f6c21-2096">Enabled setting blob tier</span></span>
* <span data-ttu-id="f6c21-2097">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="f6c21-2097">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f6c21-2098">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2098">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f6c21-2099">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="f6c21-2099">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f6c21-2100">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2100">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f6c21-2101">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="f6c21-2101">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2102">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2102">VM</span></span>

* <span data-ttu-id="f6c21-2103">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2103">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f6c21-2104">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="f6c21-2104">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f6c21-2105">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2105">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6c21-2106">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="f6c21-2106">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f6c21-2107">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="f6c21-2107">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f6c21-2108">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2108">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f6c21-2109">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2109">August 15, 2017</span></span>

<span data-ttu-id="f6c21-2110">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f6c21-2110">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2111">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2111">ACS</span></span>

* <span data-ttu-id="f6c21-2112">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="f6c21-2112">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2113">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2113">Appservice</span></span>

* <span data-ttu-id="f6c21-2114">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="f6c21-2114">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6c21-2115">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6c21-2115">Event Grid</span></span>

* <span data-ttu-id="f6c21-2116">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2116">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f6c21-2117">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2117">August 11, 2017</span></span>

<span data-ttu-id="f6c21-2118">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f6c21-2118">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2119">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2119">ACS</span></span>

* <span data-ttu-id="f6c21-2120">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="f6c21-2120">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-2121">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-2121">Batch</span></span>

* <span data-ttu-id="f6c21-2122">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="f6c21-2122">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f6c21-2123">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-2123">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f6c21-2124">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="f6c21-2124">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f6c21-2125">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="f6c21-2125">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f6c21-2126">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="f6c21-2126">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f6c21-2127">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="f6c21-2127">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f6c21-2128">Composant</span><span class="sxs-lookup"><span data-stu-id="f6c21-2128">Component</span></span>

* <span data-ttu-id="f6c21-2129">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="f6c21-2129">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f6c21-2130">Conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-2130">Container</span></span>

* <span data-ttu-id="f6c21-2131">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2131">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f6c21-2132">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2132">Data Lake Store</span></span>

* <span data-ttu-id="f6c21-2133">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="f6c21-2133">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6c21-2134">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6c21-2134">Event Grid</span></span>

* <span data-ttu-id="f6c21-2135">Version initiale</span><span class="sxs-lookup"><span data-stu-id="f6c21-2135">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-2136">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2136">Network</span></span>

* <span data-ttu-id="f6c21-2137">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="f6c21-2137">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f6c21-2138">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2138">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f6c21-2139">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2139">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f6c21-2140">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2140">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-2141">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-2141">Profile</span></span>

* <span data-ttu-id="f6c21-2142">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="f6c21-2142">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-2143">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2143">Storage</span></span>

* <span data-ttu-id="f6c21-2144">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="f6c21-2144">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2145">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2145">VM</span></span>

* <span data-ttu-id="f6c21-2146">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="f6c21-2146">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f6c21-2147">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2147">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f6c21-2148">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2148">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f6c21-2149">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="f6c21-2149">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f6c21-2150">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2150">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f6c21-2151">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2151">July 28, 2017</span></span>

<span data-ttu-id="f6c21-2152">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f6c21-2152">Version 2.0.12</span></span>

* <span data-ttu-id="f6c21-2153">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="f6c21-2153">Added container commands</span></span>
* <span data-ttu-id="f6c21-2154">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="f6c21-2154">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f6c21-2155">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-2155">Core</span></span>

* <span data-ttu-id="f6c21-2156">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="f6c21-2156">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f6c21-2157">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2157">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f6c21-2158">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2158">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f6c21-2159">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2159">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f6c21-2160">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="f6c21-2160">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f6c21-2161">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2161">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f6c21-2162">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2162">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6c21-2163">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2163">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f6c21-2164">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2164">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f6c21-2165">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2165">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f6c21-2166">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="f6c21-2166">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f6c21-2167">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2167">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f6c21-2168">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-2168">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f6c21-2169">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="f6c21-2169">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f6c21-2170">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f6c21-2170">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f6c21-2171">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2171">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f6c21-2172">ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-2172">ACR</span></span>

* <span data-ttu-id="f6c21-2173">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2173">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f6c21-2174">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2174">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f6c21-2175">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2175">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f6c21-2176">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="f6c21-2176">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f6c21-2177">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="f6c21-2177">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f6c21-2178">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="f6c21-2178">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2179">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2179">ACS</span></span>

* <span data-ttu-id="f6c21-2180">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f6c21-2180">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2181">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2181">Appservice</span></span>

* <span data-ttu-id="f6c21-2182">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="f6c21-2182">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f6c21-2183">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="f6c21-2183">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f6c21-2184">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2184">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f6c21-2185">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2185">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f6c21-2186">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2186">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f6c21-2187">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2187">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f6c21-2188">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2188">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f6c21-2189">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2189">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f6c21-2190">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2190">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f6c21-2191">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2191">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f6c21-2192">Batch</span><span class="sxs-lookup"><span data-stu-id="f6c21-2192">Batch</span></span>

* <span data-ttu-id="f6c21-2193">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="f6c21-2193">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f6c21-2194">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2194">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f6c21-2195">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2195">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6c21-2196">CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-2196">CDN</span></span>

* <span data-ttu-id="f6c21-2197">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-2197">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f6c21-2198">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6c21-2198">Cloud</span></span>

* <span data-ttu-id="f6c21-2199">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="f6c21-2199">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f6c21-2200">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2200">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f6c21-2201">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="f6c21-2201">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f6c21-2202">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="f6c21-2202">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f6c21-2203">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2203">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-2204">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-2204">CosmosDB</span></span>

* <span data-ttu-id="f6c21-2205">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2205">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f6c21-2206">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="f6c21-2206">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6c21-2207">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6c21-2207">Data Lake Analytics</span></span>

* <span data-ttu-id="f6c21-2208">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2208">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f6c21-2209">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2209">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f6c21-2210">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2210">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6c21-2211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2211">Data Lake Store</span></span>

* <span data-ttu-id="f6c21-2212">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2212">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f6c21-2213">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="f6c21-2213">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f6c21-2214">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2214">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f6c21-2215">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2215">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f6c21-2216">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6c21-2216">Interactive</span></span>

* <span data-ttu-id="f6c21-2217">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="f6c21-2217">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f6c21-2218">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="f6c21-2218">Increased test coverage</span></span>
* <span data-ttu-id="f6c21-2219">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="f6c21-2219">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f6c21-2220">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2220">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f6c21-2221">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2221">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f6c21-2222">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2222">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f6c21-2223">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2223">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6c21-2224">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2224">Added `--progress` flag</span></span>
* <span data-ttu-id="f6c21-2225">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="f6c21-2225">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f6c21-2226">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2226">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f6c21-2227">IoT</span><span class="sxs-lookup"><span data-stu-id="f6c21-2227">IoT</span></span>

* <span data-ttu-id="f6c21-2228">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2228">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f6c21-2229">(#3934)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2229">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6c21-2230">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2230">Key vault</span></span>

* <span data-ttu-id="f6c21-2231">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="f6c21-2231">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f6c21-2232">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2232">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f6c21-2233">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2233">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6c21-2234">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2234">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6c21-2235">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2235">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f6c21-2236">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2236">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f6c21-2237">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2237">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f6c21-2238">(#3307)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2238">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f6c21-2239">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2239">Lab</span></span>

* <span data-ttu-id="f6c21-2240">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2240">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f6c21-2241">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2241">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-2242">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-2242">Monitor</span></span>

* <span data-ttu-id="f6c21-2243">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2243">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f6c21-2244">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2244">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f6c21-2245">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2245">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f6c21-2246">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2246">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f6c21-2247">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2247">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f6c21-2248">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="f6c21-2248">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f6c21-2249">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="f6c21-2249">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f6c21-2250">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2250">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f6c21-2251">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2251">`location` no longer required</span></span>
  * <span data-ttu-id="f6c21-2252">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="f6c21-2252">Add name and ID support for target</span></span>
  * <span data-ttu-id="f6c21-2253">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2253">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f6c21-2254">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2254">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f6c21-2255">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="f6c21-2255">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f6c21-2256">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="f6c21-2256">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f6c21-2257">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2257">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f6c21-2258">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2258">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-2259">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2259">Network</span></span>

* <span data-ttu-id="f6c21-2260">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2260">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f6c21-2261">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2261">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f6c21-2262">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="f6c21-2262">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f6c21-2263">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="f6c21-2263">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f6c21-2264">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2264">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f6c21-2265">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2265">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f6c21-2266">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2266">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f6c21-2267">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2267">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f6c21-2268">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2268">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f6c21-2269">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2269">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f6c21-2270">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2270">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f6c21-2271">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2271">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f6c21-2272">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2272">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f6c21-2273">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2273">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f6c21-2274">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2274">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f6c21-2275">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2275">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f6c21-2276">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="f6c21-2276">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f6c21-2277">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2277">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f6c21-2278">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2278">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f6c21-2279">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2279">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f6c21-2280">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2280">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f6c21-2281">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-2281">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f6c21-2282">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2282">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f6c21-2283">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="f6c21-2283">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f6c21-2284">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="f6c21-2284">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f6c21-2285">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="f6c21-2285">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f6c21-2286">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="f6c21-2286">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-2287">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-2287">Profile</span></span>

* <span data-ttu-id="f6c21-2288">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2288">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f6c21-2289">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2289">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f6c21-2290">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="f6c21-2290">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f6c21-2291">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="f6c21-2291">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f6c21-2292">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="f6c21-2292">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6c21-2293">SGBDR</span><span class="sxs-lookup"><span data-stu-id="f6c21-2293">RDBMS</span></span>

* <span data-ttu-id="f6c21-2294">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2294">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f6c21-2295">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2295">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f6c21-2296">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2296">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f6c21-2297">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2297">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-2298">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-2298">Resource</span></span>

* <span data-ttu-id="f6c21-2299">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2299">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f6c21-2300">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="f6c21-2300">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f6c21-2301">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="f6c21-2301">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f6c21-2302">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="f6c21-2302">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f6c21-2303">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2303">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f6c21-2304">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2304">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f6c21-2305">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2305">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f6c21-2306">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="f6c21-2306">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-2307">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2307">Role</span></span>

* <span data-ttu-id="f6c21-2308">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2308">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f6c21-2309">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2309">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f6c21-2310">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="f6c21-2310">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f6c21-2311">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2311">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f6c21-2312">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2312">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6c21-2313">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6c21-2313">Service Fabric</span></span>
* <span data-ttu-id="f6c21-2314">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2314">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f6c21-2315">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2315">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f6c21-2316">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2316">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-2317">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-2317">SQL</span></span>

* <span data-ttu-id="f6c21-2318">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2318">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f6c21-2319">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2319">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f6c21-2320">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2320">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-2321">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2321">Storage</span></span>

* <span data-ttu-id="f6c21-2322">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2322">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f6c21-2323">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="f6c21-2323">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f6c21-2324">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2324">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f6c21-2325">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2325">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f6c21-2326">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2326">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f6c21-2327">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2327">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2328">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2328">VM</span></span>

* <span data-ttu-id="f6c21-2329">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2329">Support configuring nsg</span></span>
* <span data-ttu-id="f6c21-2330">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2330">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f6c21-2331">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="f6c21-2331">Support managed service identities</span></span>
* <span data-ttu-id="f6c21-2332">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2332">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f6c21-2333">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="f6c21-2333">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f6c21-2334">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2334">May 10, 2017</span></span>

<span data-ttu-id="f6c21-2335">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f6c21-2335">Version 2.0.6</span></span>

* <span data-ttu-id="f6c21-2336">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f6c21-2336">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f6c21-2337">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2337">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f6c21-2338">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2338">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f6c21-2339">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6c21-2339">Include Cognitive Services module</span></span>
* <span data-ttu-id="f6c21-2340">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6c21-2340">Include Service Fabric module</span></span>
* <span data-ttu-id="f6c21-2341">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2341">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f6c21-2342">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="f6c21-2342">Add support for CDN commands</span></span>
* <span data-ttu-id="f6c21-2343">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="f6c21-2343">Remove Container module</span></span>
* <span data-ttu-id="f6c21-2344">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2344">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f6c21-2345">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2345">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f6c21-2346">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-2346">Core</span></span>

* <span data-ttu-id="f6c21-2347">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2347">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f6c21-2348">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2348">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f6c21-2349">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2349">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f6c21-2350">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2350">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f6c21-2351">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2351">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f6c21-2352">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2352">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f6c21-2353">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2353">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f6c21-2354">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2354">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f6c21-2355">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2355">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f6c21-2356">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="f6c21-2356">core: Improved performance</span></span>
* <span data-ttu-id="f6c21-2357">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="f6c21-2357">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f6c21-2358">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="f6c21-2358">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2359">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2359">ACS</span></span>

* <span data-ttu-id="f6c21-2360">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="f6c21-2360">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f6c21-2361">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="f6c21-2361">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f6c21-2362">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="f6c21-2362">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f6c21-2363">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2363">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2364">AppService</span></span>

* <span data-ttu-id="f6c21-2365">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2365">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f6c21-2366">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="f6c21-2366">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f6c21-2367">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2367">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f6c21-2368">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="f6c21-2368">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f6c21-2369">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="f6c21-2369">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f6c21-2370">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2370">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f6c21-2371">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="f6c21-2371">support slot swap with preview</span></span>
* <span data-ttu-id="f6c21-2372">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2372">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f6c21-2373">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2373">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6c21-2374">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-2374">CosmosDB</span></span>

* <span data-ttu-id="f6c21-2375">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f6c21-2375">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f6c21-2376">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="f6c21-2376">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f6c21-2377">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="f6c21-2377">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f6c21-2378">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="f6c21-2378">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6c21-2379">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6c21-2379">Data Lake Analytics</span></span>

* <span data-ttu-id="f6c21-2380">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="f6c21-2380">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f6c21-2381">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2381">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f6c21-2382">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2382">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f6c21-2383">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="f6c21-2383">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f6c21-2384">Table</span><span class="sxs-lookup"><span data-stu-id="f6c21-2384">Table</span></span>
  * <span data-ttu-id="f6c21-2385">Fonction table</span><span class="sxs-lookup"><span data-stu-id="f6c21-2385">Table valued function</span></span>
  * <span data-ttu-id="f6c21-2386">Affichage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2386">View</span></span>
  * <span data-ttu-id="f6c21-2387">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2387">Table Statistics.</span></span> <span data-ttu-id="f6c21-2388">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="f6c21-2388">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6c21-2389">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2389">Data Lake Store</span></span>

* <span data-ttu-id="f6c21-2390">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="f6c21-2390">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f6c21-2391">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2391">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f6c21-2392">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2392">missed help for access show.</span></span> <span data-ttu-id="f6c21-2393">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2393">adding it.</span></span> <span data-ttu-id="f6c21-2394">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2394">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f6c21-2395">Rechercher</span><span class="sxs-lookup"><span data-stu-id="f6c21-2395">Find</span></span>

* <span data-ttu-id="f6c21-2396">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="f6c21-2396">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6c21-2397">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6c21-2397">KeyVault</span></span>

* <span data-ttu-id="f6c21-2398">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="f6c21-2398">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f6c21-2399">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="f6c21-2399">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f6c21-2400">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="f6c21-2400">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f6c21-2401">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-2401">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f6c21-2402">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2402">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f6c21-2403">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2403">Lab</span></span>

* <span data-ttu-id="f6c21-2404">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2404">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f6c21-2405">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2405">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f6c21-2406">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2406">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f6c21-2407">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2407">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f6c21-2408">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="f6c21-2408">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f6c21-2409">Surveiller</span><span class="sxs-lookup"><span data-stu-id="f6c21-2409">Monitor</span></span>

* <span data-ttu-id="f6c21-2410">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2410">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f6c21-2411">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2411">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f6c21-2412">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2412">Network</span></span>

* <span data-ttu-id="f6c21-2413">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2413">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f6c21-2414">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2414">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f6c21-2415">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="f6c21-2415">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f6c21-2416">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="f6c21-2416">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f6c21-2417">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="f6c21-2417">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f6c21-2418">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f6c21-2418">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f6c21-2419">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="f6c21-2419">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f6c21-2420">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="f6c21-2420">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f6c21-2421">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2421">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f6c21-2422">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="f6c21-2422">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f6c21-2423">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2423">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f6c21-2424">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2424">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f6c21-2425">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2425">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f6c21-2426">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="f6c21-2426">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f6c21-2427">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="f6c21-2427">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f6c21-2428">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="f6c21-2428">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6c21-2429">Profil</span><span class="sxs-lookup"><span data-stu-id="f6c21-2429">Profile</span></span>

* <span data-ttu-id="f6c21-2430">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2430">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f6c21-2431">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2431">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f6c21-2432">Redis</span><span class="sxs-lookup"><span data-stu-id="f6c21-2432">Redis</span></span>

* <span data-ttu-id="f6c21-2433">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="f6c21-2433">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f6c21-2434">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="f6c21-2434">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f6c21-2435">Ressource</span><span class="sxs-lookup"><span data-stu-id="f6c21-2435">Resource</span></span>

* <span data-ttu-id="f6c21-2436">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2436">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f6c21-2437">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2437">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f6c21-2438">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2438">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f6c21-2439">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2439">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f6c21-2440">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2440">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f6c21-2441">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2441">Add docs for az lock update.</span></span> <span data-ttu-id="f6c21-2442">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2442">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f6c21-2443">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2443">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f6c21-2444">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2444">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f6c21-2445">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2445">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f6c21-2446">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2446">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f6c21-2447">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2447">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f6c21-2448">Rôle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2448">Role</span></span>

* <span data-ttu-id="f6c21-2449">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2449">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f6c21-2450">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2450">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f6c21-2451">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2451">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f6c21-2452">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="f6c21-2452">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f6c21-2453">SQL</span><span class="sxs-lookup"><span data-stu-id="f6c21-2453">SQL</span></span>

* <span data-ttu-id="f6c21-2454">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="f6c21-2454">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f6c21-2455">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2455">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f6c21-2456">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2456">Storage</span></span>

* <span data-ttu-id="f6c21-2457">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f6c21-2457">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f6c21-2458">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="f6c21-2458">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f6c21-2459">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="f6c21-2459">Add support for large block blob upload</span></span>
* <span data-ttu-id="f6c21-2460">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="f6c21-2460">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2461">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2461">VM</span></span>

* <span data-ttu-id="f6c21-2462">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="f6c21-2462">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f6c21-2463">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="f6c21-2463">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f6c21-2464">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f6c21-2464">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f6c21-2465">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f6c21-2465">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f6c21-2466">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="f6c21-2466">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f6c21-2467">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="f6c21-2467">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f6c21-2468">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2468">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f6c21-2469">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2469">April 3, 2017</span></span>

<span data-ttu-id="f6c21-2470">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f6c21-2470">Version 2.0.2</span></span>

<span data-ttu-id="f6c21-2471">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="f6c21-2471">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f6c21-2472">Principal</span><span class="sxs-lookup"><span data-stu-id="f6c21-2472">Core</span></span>

* <span data-ttu-id="f6c21-2473">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-2473">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f6c21-2474">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2474">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f6c21-2475">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2475">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f6c21-2476">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2476">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6c21-2477">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2477">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f6c21-2478">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2478">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f6c21-2479">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2479">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f6c21-2480">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="f6c21-2480">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f6c21-2481">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="f6c21-2481">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f6c21-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="f6c21-2482">ACS</span></span>

* <span data-ttu-id="f6c21-2483">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2483">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f6c21-2484">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2484">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f6c21-2485">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2485">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f6c21-2486">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2486">Add support for windows clusters.</span></span> <span data-ttu-id="f6c21-2487">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2487">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f6c21-2488">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2488">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f6c21-2489">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2489">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6c21-2490">AppService</span><span class="sxs-lookup"><span data-stu-id="f6c21-2490">AppService</span></span>

* <span data-ttu-id="f6c21-2491">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2491">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f6c21-2492">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2492">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f6c21-2493">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2493">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f6c21-2494">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2494">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f6c21-2495">DataLake</span><span class="sxs-lookup"><span data-stu-id="f6c21-2495">DataLake</span></span>

* <span data-ttu-id="f6c21-2496">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6c21-2496">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f6c21-2497">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6c21-2497">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f6c21-2498">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f6c21-2498">DocuemntDB</span></span>

* <span data-ttu-id="f6c21-2499">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2499">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f6c21-2500">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="f6c21-2500">VM</span></span>

* <span data-ttu-id="f6c21-2501">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2501">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f6c21-2502">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2502">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f6c21-2503">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2503">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f6c21-2504">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2504">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6c21-2505">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2505">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f6c21-2506">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2506">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f6c21-2507">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f6c21-2507">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f6c21-2508">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="f6c21-2508">February 27, 2017</span></span>

<span data-ttu-id="f6c21-2509">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f6c21-2509">Version 2.0.0</span></span>

<span data-ttu-id="f6c21-2510">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="f6c21-2510">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f6c21-2511">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2511">Container Service (acs)</span></span>
- <span data-ttu-id="f6c21-2512">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2512">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f6c21-2513">Réseau</span><span class="sxs-lookup"><span data-stu-id="f6c21-2513">Networking</span></span>
- <span data-ttu-id="f6c21-2514">Stockage</span><span class="sxs-lookup"><span data-stu-id="f6c21-2514">Storage</span></span>

<span data-ttu-id="f6c21-2515">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2515">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f6c21-2516">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2516">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f6c21-2517">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2517">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f6c21-2518">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2518">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f6c21-2519">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f6c21-2519">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f6c21-2520">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="f6c21-2520">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f6c21-2521">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f6c21-2521">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f6c21-2522">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="f6c21-2522">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f6c21-2523">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f6c21-2523">Provide feedback from the command line with the `az feedback` command</span></span>

