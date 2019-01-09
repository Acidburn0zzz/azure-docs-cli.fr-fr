---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/18/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 10663ad8e85a15b8fedb5ac12c5d17256d07e523
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805956"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="e5aa7-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-103">Azure CLI release notes</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="e5aa7-104">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-104">December 20, 2018</span></span>

<span data-ttu-id="e5aa7-105">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="e5aa7-105">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="e5aa7-106">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-106">Appservice</span></span>
* <span data-ttu-id="e5aa7-107">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-107">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="e5aa7-108">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="e5aa7-108">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="e5aa7-109">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-109">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e5aa7-110">IotCentral</span><span class="sxs-lookup"><span data-stu-id="e5aa7-110">IoTCentral</span></span>
* <span data-ttu-id="e5aa7-111">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="e5aa7-111">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-112">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-112">Role</span></span>
* <span data-ttu-id="e5aa7-113">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-113">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-114">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-114">SQL</span></span>
* <span data-ttu-id="e5aa7-115">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-115">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-116">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-116">VM</span></span>
* <span data-ttu-id="e5aa7-117">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-117">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="e5aa7-118">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-118">December 18, 2018</span></span>

<span data-ttu-id="e5aa7-119">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="e5aa7-119">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="e5aa7-120">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-120">ACR</span></span>
* <span data-ttu-id="e5aa7-121">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-121">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="e5aa7-122">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="e5aa7-122">Condensed the table layout for task list</span></span>
* <span data-ttu-id="e5aa7-123">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="e5aa7-123">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-124">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-124">ACS</span></span>
* <span data-ttu-id="e5aa7-125">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="e5aa7-125">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e5aa7-126">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-126">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="e5aa7-127">[DÉCONSEILLÉ] Commandes `az acs` déconseillées.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-127">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="e5aa7-128">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-128">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="e5aa7-129">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-129">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="e5aa7-130">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="e5aa7-130">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-131">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-131">Appservice</span></span>
* <span data-ttu-id="e5aa7-132">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-132">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="e5aa7-133">Botservice</span><span class="sxs-lookup"><span data-stu-id="e5aa7-133">Botservice</span></span>
* <span data-ttu-id="e5aa7-134">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-134">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="e5aa7-135">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="e5aa7-135">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="e5aa7-136">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="e5aa7-136">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="e5aa7-137">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-137">Reduced Kudu network calls</span></span>
* <span data-ttu-id="e5aa7-138">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="e5aa7-138">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-139">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-139">Consumption</span></span>
* <span data-ttu-id="e5aa7-140">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="e5aa7-140">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-141">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-141">CosmosDB</span></span>
* <span data-ttu-id="e5aa7-142">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-142">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="e5aa7-143">Cartes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-143">Maps</span></span>
* <span data-ttu-id="e5aa7-144">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-144">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-145">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-145">Network</span></span>
* <span data-ttu-id="e5aa7-146">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-146">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="e5aa7-147">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="e5aa7-147">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-148">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-148">Resource</span></span>
* <span data-ttu-id="e5aa7-149">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-149">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="e5aa7-150">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-150">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-151">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-151">Storage</span></span>
*  <span data-ttu-id="e5aa7-152">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-152">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-153">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-153">VM</span></span>
* <span data-ttu-id="e5aa7-154">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-154">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="e5aa7-155">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-155">December 4, 2018</span></span>

<span data-ttu-id="e5aa7-156">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="e5aa7-156">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="e5aa7-157">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-157">Core</span></span>
* <span data-ttu-id="e5aa7-158">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-158">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="e5aa7-159">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-159">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-160">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-160">Appservice</span></span>
* <span data-ttu-id="e5aa7-161">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-161">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="e5aa7-162">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-162">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-163">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-163">Network</span></span>
* <span data-ttu-id="e5aa7-164">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="e5aa7-164">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-165">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-165">Role</span></span>
* <span data-ttu-id="e5aa7-166">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-166">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="e5aa7-167">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-167">VM</span></span>
* <span data-ttu-id="e5aa7-168">[DÉCONSEILLÉ] Le paramètre `vm extension [show|wait] --expand` est déconseillé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-168">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="e5aa7-169">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-169">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="e5aa7-170">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-170">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="e5aa7-171">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-171">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="e5aa7-172">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-172">November 20, 2018</span></span>

<span data-ttu-id="e5aa7-173">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="e5aa7-173">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="e5aa7-174">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-174">Core</span></span>
* <span data-ttu-id="e5aa7-175">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="e5aa7-175">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-176">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-176">ACR</span></span>
* <span data-ttu-id="e5aa7-177">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="e5aa7-177">Added context token to task step</span></span>
* <span data-ttu-id="e5aa7-178">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="e5aa7-178">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="e5aa7-179">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-179">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-180">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-180">Appservice</span></span>
* <span data-ttu-id="e5aa7-181">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-181">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="e5aa7-182">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-182">Updated the default `node_version`.</span></span> <span data-ttu-id="e5aa7-183">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="e5aa7-183">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="e5aa7-184">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-184">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="e5aa7-185">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="e5aa7-185">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e5aa7-186">IotCentral</span><span class="sxs-lookup"><span data-stu-id="e5aa7-186">IotCentral</span></span>
* <span data-ttu-id="e5aa7-187">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5aa7-187">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-188">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-188">KeyVault</span></span>
* <span data-ttu-id="e5aa7-189">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-189">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-190">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-190">Network</span></span>
* <span data-ttu-id="e5aa7-191">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="e5aa7-191">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="e5aa7-192">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-192">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="e5aa7-193">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-193">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="e5aa7-194">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-194">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-195">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e5aa7-195">Rdbms</span></span>
* <span data-ttu-id="e5aa7-196">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="e5aa7-196">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="e5aa7-197">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-197">Rbac</span></span>
* <span data-ttu-id="e5aa7-198">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-198">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="e5aa7-199">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-199">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="e5aa7-200">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-200">Storage</span></span>
* <span data-ttu-id="e5aa7-201">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-201">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="e5aa7-202">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-202">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="e5aa7-203">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-203">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="e5aa7-204">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-204">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-205">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-205">VM</span></span>
* <span data-ttu-id="e5aa7-206">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="e5aa7-206">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="e5aa7-207">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-207">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="e5aa7-208">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-208">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="e5aa7-209">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-209">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="e5aa7-210">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-210">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="e5aa7-211">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-211">Added `snapshot wait` command</span></span>
* <span data-ttu-id="e5aa7-212">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-212">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="e5aa7-213">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-213">November 6, 2018</span></span>

<span data-ttu-id="e5aa7-214">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="e5aa7-214">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-215">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-215">Core</span></span>
* <span data-ttu-id="e5aa7-216">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="e5aa7-216">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-217">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-217">ACR</span></span>
* <span data-ttu-id="e5aa7-218">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="e5aa7-218">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="e5aa7-219">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="e5aa7-219">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-220">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-220">ACS</span></span>
* <span data-ttu-id="e5aa7-221">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-221">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="e5aa7-222">Advisor</span><span class="sxs-lookup"><span data-stu-id="e5aa7-222">Advisor</span></span>
* <span data-ttu-id="e5aa7-223">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-223">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="e5aa7-224">AMS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-224">AMS</span></span>
* <span data-ttu-id="e5aa7-225">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-225">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="e5aa7-226">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-226">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="e5aa7-227">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-227">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="e5aa7-228">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="e5aa7-228">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="e5aa7-229">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-229">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="e5aa7-230">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-230">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="e5aa7-231">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-231">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="e5aa7-232">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-232">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="e5aa7-233">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-233">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="e5aa7-234">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-234">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="e5aa7-235">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-235">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="e5aa7-236">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-236">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="e5aa7-237">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="e5aa7-237">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="e5aa7-238">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-238">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="e5aa7-239">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-239">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="e5aa7-240">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="e5aa7-240">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="e5aa7-241">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-241">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-242">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-242">AppService</span></span>
* <span data-ttu-id="e5aa7-243">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-243">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="e5aa7-244">Configuration</span><span class="sxs-lookup"><span data-stu-id="e5aa7-244">Configure</span></span>
* <span data-ttu-id="e5aa7-245">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-245">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-246">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-246">Container</span></span>
* <span data-ttu-id="e5aa7-247">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="e5aa7-247">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5aa7-248">Event Hub</span><span class="sxs-lookup"><span data-stu-id="e5aa7-248">EventHub</span></span>
* <span data-ttu-id="e5aa7-249">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-249">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-250">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-250">Interactive</span></span>
* <span data-ttu-id="e5aa7-251">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="e5aa7-251">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-252">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-252">Monitor</span></span>
* <span data-ttu-id="e5aa7-253">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-253">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-254">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-254">Network</span></span>
* <span data-ttu-id="e5aa7-255">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-255">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="e5aa7-256">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-256">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="e5aa7-257">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-257">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="e5aa7-258">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-258">Profile</span></span>
* <span data-ttu-id="e5aa7-259">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-259">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-260">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-260">RDBMS</span></span>
* <span data-ttu-id="e5aa7-261">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="e5aa7-261">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-262">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-262">Resource</span></span>
* <span data-ttu-id="e5aa7-263">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-263">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-264">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-264">Role</span></span>
* <span data-ttu-id="e5aa7-265">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="e5aa7-265">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="e5aa7-266">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-266">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="e5aa7-267">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="e5aa7-267">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-268">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-268">Storage</span></span>
* <span data-ttu-id="e5aa7-269">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-269">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-270">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-270">VM</span></span>
* <span data-ttu-id="e5aa7-271">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-271">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="e5aa7-272">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-272">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="e5aa7-273">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="e5aa7-273">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="e5aa7-274">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="e5aa7-274">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="e5aa7-275">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="e5aa7-275">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="e5aa7-276">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-276">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="e5aa7-277">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-277">October 23, 2018</span></span>

<span data-ttu-id="e5aa7-278">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="e5aa7-278">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-279">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-279">Core</span></span>
* <span data-ttu-id="e5aa7-280">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-280">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="e5aa7-281">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-281">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-282">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-282">ACR</span></span>
* <span data-ttu-id="e5aa7-283">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="e5aa7-283">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="e5aa7-284">CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-284">CDN</span></span>
* <span data-ttu-id="e5aa7-285">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-285">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e5aa7-286">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-286">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-287">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-287">Container</span></span>
* <span data-ttu-id="e5aa7-288">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="e5aa7-288">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="e5aa7-289">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-289">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="e5aa7-290">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="e5aa7-290">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="e5aa7-291">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-291">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="e5aa7-292">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="e5aa7-292">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="e5aa7-293">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="e5aa7-293">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="e5aa7-294">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-294">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-295">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-295">CosmosDB</span></span>
* <span data-ttu-id="e5aa7-296">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-296">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-297">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-297">Interactive</span></span>
* <span data-ttu-id="e5aa7-298">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="e5aa7-298">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5aa7-299">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5aa7-299">IoT Central</span></span>
* <span data-ttu-id="e5aa7-300">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="e5aa7-300">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="e5aa7-301">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="e5aa7-301">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-302">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-302">Monitor</span></span>
* <span data-ttu-id="e5aa7-303">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-303">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="e5aa7-304">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-304">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="e5aa7-305">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="e5aa7-305">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e5aa7-306">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-306">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="e5aa7-307">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-307">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="e5aa7-308">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-308">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="e5aa7-309">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-309">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="e5aa7-310">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="e5aa7-310">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e5aa7-311">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-311">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="e5aa7-312">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-312">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-313">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-313">Network</span></span>
* <span data-ttu-id="e5aa7-314">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-314">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="e5aa7-315">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-315">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="e5aa7-316">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-316">ServiceBus</span></span>
* <span data-ttu-id="e5aa7-317">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-317">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-318">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-318">SQL</span></span>
* <span data-ttu-id="e5aa7-319">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-319">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-320">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-320">Storage</span></span>
* <span data-ttu-id="e5aa7-321">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="e5aa7-321">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="e5aa7-322">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-322">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-323">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-323">VM</span></span>
* <span data-ttu-id="e5aa7-324">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-324">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5aa7-325">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-325">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="e5aa7-326">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-326">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="e5aa7-327">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-327">October 16, 2018</span></span>

<span data-ttu-id="e5aa7-328">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="e5aa7-328">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-329">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-329">VM</span></span>
* <span data-ttu-id="e5aa7-330">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="e5aa7-330">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="e5aa7-331">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-331">October 9, 2018</span></span>

<span data-ttu-id="e5aa7-332">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="e5aa7-332">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-333">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-333">Core</span></span>
* <span data-ttu-id="e5aa7-334">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-334">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-335">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-335">ACR</span></span>
* <span data-ttu-id="e5aa7-336">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="e5aa7-336">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-337">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-337">ACS</span></span>
* <span data-ttu-id="e5aa7-338">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="e5aa7-338">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="e5aa7-339">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="e5aa7-339">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="e5aa7-340">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-340">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="e5aa7-341">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-341">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-342">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-342">Container</span></span>
* <span data-ttu-id="e5aa7-343">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-343">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="e5aa7-344">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-344">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="e5aa7-345">Event Hub</span><span class="sxs-lookup"><span data-stu-id="e5aa7-345">Event Hub</span></span>
* <span data-ttu-id="e5aa7-346">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-346">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="e5aa7-347">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-347">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="e5aa7-348">Extensions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-348">Extensions</span></span>
* <span data-ttu-id="e5aa7-349">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-349">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5aa7-350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5aa7-350">HDInsight</span></span>
* <span data-ttu-id="e5aa7-351">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-351">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-352">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-352">IoT</span></span>
* <span data-ttu-id="e5aa7-353">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="e5aa7-353">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-354">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-354">KeyVault</span></span>
* <span data-ttu-id="e5aa7-355">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="e5aa7-355">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-356">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-356">Network</span></span>
* <span data-ttu-id="e5aa7-357">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-357">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="e5aa7-358">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="e5aa7-358">See #6052</span></span>
* <span data-ttu-id="e5aa7-359">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-359">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="e5aa7-360">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="e5aa7-360">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="e5aa7-361">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-361">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="e5aa7-362">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-362">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="e5aa7-363">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-363">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="e5aa7-364">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-364">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-365">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-365">Role</span></span>
* <span data-ttu-id="e5aa7-366">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-366">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="e5aa7-367">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-367">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="e5aa7-368">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="e5aa7-368">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="e5aa7-369">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-369">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5aa7-370">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-370">Service Bus</span></span>
* <span data-ttu-id="e5aa7-371">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-371">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-372">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-372">VM</span></span>
* <span data-ttu-id="e5aa7-373">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-373">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="e5aa7-374">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-374">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="e5aa7-375">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-375">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="e5aa7-376">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-376">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="e5aa7-377">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-377">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="e5aa7-378">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-378">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="e5aa7-379">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-379">September 21, 2018</span></span>

<span data-ttu-id="e5aa7-380">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="e5aa7-380">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-381">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-381">ACR</span></span>
* <span data-ttu-id="e5aa7-382">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-382">Added ACR Task commands</span></span>
* <span data-ttu-id="e5aa7-383">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-383">Added quick run command</span></span>
* <span data-ttu-id="e5aa7-384">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-384">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="e5aa7-385">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-385">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="e5aa7-386">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-386">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="e5aa7-387">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="e5aa7-387">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-388">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-388">ACS</span></span>
* <span data-ttu-id="e5aa7-389">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-389">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="e5aa7-390">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="e5aa7-390">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-391">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-391">AppService</span></span>

* <span data-ttu-id="e5aa7-392">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-392">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="e5aa7-393">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="e5aa7-393">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="e5aa7-394">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="e5aa7-394">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="e5aa7-395">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-395">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-396">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-396">Batch</span></span>
* <span data-ttu-id="e5aa7-397">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="e5aa7-397">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="e5aa7-398">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-398">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="e5aa7-399">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-399">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="e5aa7-400">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-400">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5aa7-401">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-401">Batch AI</span></span> 
* <span data-ttu-id="e5aa7-402">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-402">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5aa7-403">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-403">Cognitive Services</span></span>
* <span data-ttu-id="e5aa7-404">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-404">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="e5aa7-405">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-405">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="e5aa7-406">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-406">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="e5aa7-407">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-407">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="e5aa7-408">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-408">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="e5aa7-409">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-409">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-410">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-410">Container</span></span>
* <span data-ttu-id="e5aa7-411">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="e5aa7-411">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="e5aa7-412">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-412">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="e5aa7-413">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-413">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="e5aa7-414">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-414">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="e5aa7-415">DataLake</span><span class="sxs-lookup"><span data-stu-id="e5aa7-415">Datalake</span></span>
* <span data-ttu-id="e5aa7-416">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-416">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="e5aa7-417">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-417">Interactive Shell</span></span>
* <span data-ttu-id="e5aa7-418">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-418">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="e5aa7-419">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-419">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-420">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-420">IoT</span></span>
* <span data-ttu-id="e5aa7-421">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-421">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5aa7-422">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-422">Key Vault</span></span>
* <span data-ttu-id="e5aa7-423">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="e5aa7-423">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-424">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-424">Network</span></span>
* <span data-ttu-id="e5aa7-425">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-425">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="e5aa7-426">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-426">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="e5aa7-427">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="e5aa7-427">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="e5aa7-428">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-428">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="e5aa7-429">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-429">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="e5aa7-430">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-430">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="e5aa7-431">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-431">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="e5aa7-432">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-432">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="e5aa7-433">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-433">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="e5aa7-434">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-434">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="e5aa7-435">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-435">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="e5aa7-436">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-436">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="e5aa7-437">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-437">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="e5aa7-438">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-438">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="e5aa7-439">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-439">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="e5aa7-440">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="e5aa7-440">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="e5aa7-441">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-441">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="e5aa7-442">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-442">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-443">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-443">RDBMS</span></span>
* <span data-ttu-id="e5aa7-444">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-444">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="e5aa7-445">Réservation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-445">Reservation</span></span>
* <span data-ttu-id="e5aa7-446">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-446">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="e5aa7-447">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-447">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="e5aa7-448">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="e5aa7-448">Manage App</span></span>
* <span data-ttu-id="e5aa7-449">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-449">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="e5aa7-450">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="e5aa7-450">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-451">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-451">Role</span></span>
* <span data-ttu-id="e5aa7-452">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-452">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="e5aa7-453">SignalR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-453">SignalR</span></span>
* <span data-ttu-id="e5aa7-454">Première version</span><span class="sxs-lookup"><span data-stu-id="e5aa7-454">First release</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-455">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-455">Storage</span></span>
* <span data-ttu-id="e5aa7-456">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="e5aa7-456">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="e5aa7-457">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="e5aa7-457">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-458">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-458">VM</span></span>
* <span data-ttu-id="e5aa7-459">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-459">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="e5aa7-460">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-460">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="e5aa7-461">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-461">August 28, 2018</span></span>

<span data-ttu-id="e5aa7-462">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="e5aa7-462">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-463">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-463">Core</span></span>

* <span data-ttu-id="e5aa7-464">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-464">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="e5aa7-465">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5aa7-465">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-466">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-466">ACR</span></span>

* <span data-ttu-id="e5aa7-467">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="e5aa7-467">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="e5aa7-468">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-468">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-469">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-469">ACS</span></span>

* <span data-ttu-id="e5aa7-470">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-470">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="e5aa7-471">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="e5aa7-471">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-472">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-472">AppService</span></span>

* <span data-ttu-id="e5aa7-473">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="e5aa7-473">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="e5aa7-474">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="e5aa7-474">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="e5aa7-475">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-475">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="e5aa7-476">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e5aa7-476">Backup</span></span>

* <span data-ttu-id="e5aa7-477">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-477">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="e5aa7-478">Service de robot</span><span class="sxs-lookup"><span data-stu-id="e5aa7-478">Bot Service</span></span>

* <span data-ttu-id="e5aa7-479">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-479">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5aa7-480">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-480">Cognitive Services</span></span>

* <span data-ttu-id="e5aa7-481">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-481">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-482">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-482">IoT</span></span>

* <span data-ttu-id="e5aa7-483">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-483">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-484">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-484">Monitor</span></span>

* <span data-ttu-id="e5aa7-485">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-485">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="e5aa7-486">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-486">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-487">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-487">Network</span></span>

* <span data-ttu-id="e5aa7-488">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-488">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-489">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-489">Resource</span></span>

* <span data-ttu-id="e5aa7-490">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-490">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-491">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-491">Storage</span></span>

* <span data-ttu-id="e5aa7-492">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-492">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-493">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-493">VM</span></span>

* <span data-ttu-id="e5aa7-494">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-494">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="e5aa7-495">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-495">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="e5aa7-496">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-496">Auguest 14, 2018</span></span>

<span data-ttu-id="e5aa7-497">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="e5aa7-497">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-498">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-498">Core</span></span>

* <span data-ttu-id="e5aa7-499">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-499">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="e5aa7-500">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="e5aa7-500">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="e5aa7-501">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-501">Telemetry</span></span>

* <span data-ttu-id="e5aa7-502">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-502">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-503">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-503">ACR</span></span>

* <span data-ttu-id="e5aa7-504">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-504">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="e5aa7-505">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-505">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-506">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-506">ACS</span></span>

* <span data-ttu-id="e5aa7-507">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-507">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="e5aa7-508">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-508">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="e5aa7-509">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-509">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="e5aa7-510">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-510">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="e5aa7-511">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="e5aa7-511">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="e5aa7-512">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-512">AppService</span></span>

* <span data-ttu-id="e5aa7-513">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-513">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="e5aa7-514">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="e5aa7-514">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="e5aa7-515">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-515">BatchAI</span></span>

* <span data-ttu-id="e5aa7-516">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="e5aa7-516">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="e5aa7-517">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-517">Container</span></span>

* <span data-ttu-id="e5aa7-518">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-518">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="e5aa7-519">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-519">IoT</span></span>

* <span data-ttu-id="e5aa7-520">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="e5aa7-520">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="e5aa7-521">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-521">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5aa7-522">Iot Central</span><span class="sxs-lookup"><span data-stu-id="e5aa7-522">Iot Central</span></span>

* <span data-ttu-id="e5aa7-523">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5aa7-523">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-524">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-524">KeyVault</span></span>


* <span data-ttu-id="e5aa7-525">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-525">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="e5aa7-526">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-526">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="e5aa7-527">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="e5aa7-527">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="e5aa7-528">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-528">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="e5aa7-529">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-529">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="e5aa7-530">Relais</span><span class="sxs-lookup"><span data-stu-id="e5aa7-530">Relay</span></span>

* <span data-ttu-id="e5aa7-531">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-531">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-532">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-532">Sql</span></span>

* <span data-ttu-id="e5aa7-533">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-533">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-534">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-534">Storage</span></span>

* <span data-ttu-id="e5aa7-535">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="e5aa7-535">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="e5aa7-536">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-536">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="e5aa7-537">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-537">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="e5aa7-538">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="e5aa7-538">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="e5aa7-539">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-539">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-540">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-540">VM</span></span>

* <span data-ttu-id="e5aa7-541">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-541">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e5aa7-542">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-542">July 31, 2018</span></span>

<span data-ttu-id="e5aa7-543">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e5aa7-543">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-544">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-544">ACR</span></span>

* <span data-ttu-id="e5aa7-545">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-545">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e5aa7-546">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-546">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-547">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-547">ACS</span></span>

* <span data-ttu-id="e5aa7-548">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-548">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-549">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-549">Batch</span></span>

* <span data-ttu-id="e5aa7-550">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5aa7-550">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-551">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-551">Container</span></span>

* <span data-ttu-id="e5aa7-552">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="e5aa7-552">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-553">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-553">Network</span></span>

* <span data-ttu-id="e5aa7-554">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5aa7-554">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e5aa7-555">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-555">Resource</span></span>

* <span data-ttu-id="e5aa7-556">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-556">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e5aa7-557">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-557">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-558">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-558">Role</span></span>

* <span data-ttu-id="e5aa7-559">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-559">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e5aa7-560">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-560">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e5aa7-561">Recherche</span><span class="sxs-lookup"><span data-stu-id="e5aa7-561">Search</span></span>

* <span data-ttu-id="e5aa7-562">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="e5aa7-562">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5aa7-563">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-563">Service Bus</span></span>

* <span data-ttu-id="e5aa7-564">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="e5aa7-564">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e5aa7-565">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-565">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e5aa7-566">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-566">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e5aa7-567">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-567">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-568">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-568">Storage</span></span>

* <span data-ttu-id="e5aa7-569">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-569">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e5aa7-570">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-570">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-571">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-571">VM</span></span>

* <span data-ttu-id="e5aa7-572">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-572">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e5aa7-573">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-573">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e5aa7-574">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="e5aa7-574">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e5aa7-575">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-575">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e5aa7-576">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-576">July 18, 2018</span></span>

<span data-ttu-id="e5aa7-577">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e5aa7-577">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-578">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-578">Core</span></span>

* <span data-ttu-id="e5aa7-579">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-579">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e5aa7-580">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-580">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e5aa7-581">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-581">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-582">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-582">ACR</span></span>

* <span data-ttu-id="e5aa7-583">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-583">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e5aa7-584">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-584">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e5aa7-585">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-585">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e5aa7-586">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-586">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-587">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-587">ACS</span></span>

* <span data-ttu-id="e5aa7-588">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="e5aa7-588">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-589">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-589">AppService</span></span>

* <span data-ttu-id="e5aa7-590">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="e5aa7-590">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-591">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-591">Batch</span></span>

* <span data-ttu-id="e5aa7-592">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5aa7-592">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e5aa7-593">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="e5aa7-593">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5aa7-594">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-594">Batch AI</span></span>

* <span data-ttu-id="e5aa7-595">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-595">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-596">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-596">Container</span></span>

* <span data-ttu-id="e5aa7-597">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="e5aa7-597">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e5aa7-598">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="e5aa7-598">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-599">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-599">Network</span></span>

* <span data-ttu-id="e5aa7-600">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-600">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e5aa7-601">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-601">Added `network nic wait`</span></span>
* <span data-ttu-id="e5aa7-602">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-602">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e5aa7-603">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-603">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e5aa7-604">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-604">Resource</span></span>

* <span data-ttu-id="e5aa7-605">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-605">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e5aa7-606">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-606">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e5aa7-607">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-607">Added `deployment wait` command</span></span>
* <span data-ttu-id="e5aa7-608">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e5aa7-608">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-609">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-609">SQL</span></span>

* <span data-ttu-id="e5aa7-610">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-610">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e5aa7-611">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-611">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e5aa7-612">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-612">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-613">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-613">Storage</span></span>

* <span data-ttu-id="e5aa7-614">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="e5aa7-614">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-615">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-615">VM</span></span>

* <span data-ttu-id="e5aa7-616">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-616">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e5aa7-617">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-617">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e5aa7-618">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-618">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e5aa7-619">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-619">July 3, 2018</span></span>

<span data-ttu-id="e5aa7-620">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e5aa7-620">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e5aa7-621">AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-621">AKS</span></span>

* <span data-ttu-id="e5aa7-622">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-622">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e5aa7-623">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-623">July 3, 2018</span></span>

<span data-ttu-id="e5aa7-624">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e5aa7-624">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-625">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-625">Core</span></span>

* <span data-ttu-id="e5aa7-626">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-626">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-627">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-627">ACR</span></span>

* <span data-ttu-id="e5aa7-628">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="e5aa7-628">Added polling build status</span></span>
* <span data-ttu-id="e5aa7-629">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="e5aa7-629">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e5aa7-630">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-630">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-631">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-631">ACS</span></span>

* <span data-ttu-id="e5aa7-632">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-632">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e5aa7-633">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-633">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e5aa7-634">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-634">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e5aa7-635">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-635">Added `--listen-port` support</span></span>
* <span data-ttu-id="e5aa7-636">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-636">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e5aa7-637">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="e5aa7-637">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e5aa7-638">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-638">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-639">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-639">AppService</span></span>

* <span data-ttu-id="e5aa7-640">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-640">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e5aa7-641">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="e5aa7-641">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e5aa7-642">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e5aa7-642">Backup</span></span>

* <span data-ttu-id="e5aa7-643">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="e5aa7-643">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e5aa7-644">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-644">BatchAI</span></span>

* <span data-ttu-id="e5aa7-645">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-645">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e5aa7-646">Cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-646">Cloud</span></span>

* <span data-ttu-id="e5aa7-647">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-647">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-648">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-648">Container</span></span>

* <span data-ttu-id="e5aa7-649">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="e5aa7-649">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e5aa7-650">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-650">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e5aa7-651">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="e5aa7-651">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-652">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-652">Extension</span></span>

* <span data-ttu-id="e5aa7-653">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-653">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-654">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-654">Network</span></span>

* <span data-ttu-id="e5aa7-655">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-655">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-656">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e5aa7-656">Rdbms</span></span>

* <span data-ttu-id="e5aa7-657">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-657">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-658">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-658">Resource</span></span>

* <span data-ttu-id="e5aa7-659">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-659">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-660">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-660">VM</span></span>

* <span data-ttu-id="e5aa7-661">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="e5aa7-661">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e5aa7-662">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-662">June 25, 2018</span></span>

<span data-ttu-id="e5aa7-663">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e5aa7-663">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e5aa7-664">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-664">CLI</span></span>

* <span data-ttu-id="e5aa7-665">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-665">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e5aa7-666">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-666">June 19, 2018</span></span>

<span data-ttu-id="e5aa7-667">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e5aa7-667">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-668">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-668">Core</span></span>

* <span data-ttu-id="e5aa7-669">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-669">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-670">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-670">ACR</span></span>

* <span data-ttu-id="e5aa7-671">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="e5aa7-671">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e5aa7-672">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-672">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-673">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-673">ACS</span></span>

* <span data-ttu-id="e5aa7-674">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-674">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e5aa7-675">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-675">Added `--update` support</span></span>
* <span data-ttu-id="e5aa7-676">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-676">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e5aa7-677">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-677">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e5aa7-678">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-678">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e5aa7-679">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-679">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e5aa7-680">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-680">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e5aa7-681">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-681">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-682">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-682">AppService</span></span>

* <span data-ttu-id="e5aa7-683">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-683">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e5aa7-684">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-684">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-685">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-685">Batch</span></span>

* <span data-ttu-id="e5aa7-686">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-686">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5aa7-687">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-687">Batch AI</span></span>

* <span data-ttu-id="e5aa7-688">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-688">Added support for workspaces.</span></span> <span data-ttu-id="e5aa7-689">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-689">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e5aa7-690">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-690">Added support for experiments.</span></span> <span data-ttu-id="e5aa7-691">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-691">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e5aa7-692">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="e5aa7-692">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e5aa7-693">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-693">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e5aa7-694">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-694">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e5aa7-695">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-695">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e5aa7-696">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-696">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e5aa7-697">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="e5aa7-697">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e5aa7-698">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-698">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e5aa7-699">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-699">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e5aa7-700">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-700">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e5aa7-701">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-701">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e5aa7-702">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-702">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e5aa7-703">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-703">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e5aa7-704">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-704">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e5aa7-705">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-705">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="e5aa7-706">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-706">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="e5aa7-707">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-707">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e5aa7-708">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-708">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e5aa7-709">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-709">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e5aa7-710">Cartes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-710">Maps</span></span>

* <span data-ttu-id="e5aa7-711">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-711">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-712">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-712">Network</span></span>

* <span data-ttu-id="e5aa7-713">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-713">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e5aa7-714">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-714">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e5aa7-715">#6502</span><span class="sxs-lookup"><span data-stu-id="e5aa7-715">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e5aa7-716">Réservations</span><span class="sxs-lookup"><span data-stu-id="e5aa7-716">Reservations</span></span>

* <span data-ttu-id="e5aa7-717">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-717">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e5aa7-718">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-718">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e5aa7-719">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-719">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e5aa7-720">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-720">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e5aa7-721">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-721">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e5aa7-722">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-722">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-723">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-723">Role</span></span>

* <span data-ttu-id="e5aa7-724">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-724">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-725">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-725">SQL</span></span>

* <span data-ttu-id="e5aa7-726">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-726">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-727">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-727">Storage</span></span>

* <span data-ttu-id="e5aa7-728">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-728">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-729">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-729">VM</span></span>

* <span data-ttu-id="e5aa7-730">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-730">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e5aa7-731">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-731">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e5aa7-732">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-732">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e5aa7-733">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-733">June 13, 2018</span></span>

<span data-ttu-id="e5aa7-734">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e5aa7-734">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-735">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-735">Core</span></span>

* <span data-ttu-id="e5aa7-736">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-736">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e5aa7-737">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-737">June 13, 2018</span></span>

<span data-ttu-id="e5aa7-738">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e5aa7-738">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e5aa7-739">AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-739">AKS</span></span>

* <span data-ttu-id="e5aa7-740">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-740">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e5aa7-741">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="e5aa7-741">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e5aa7-742">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-742">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e5aa7-743">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-743">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e5aa7-744">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-744">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-745">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-745">AppService</span></span>

* <span data-ttu-id="e5aa7-746">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="e5aa7-746">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e5aa7-747">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-747">June 5, 2018</span></span>

<span data-ttu-id="e5aa7-748">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e5aa7-748">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-749">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-749">Interactive</span></span>

* <span data-ttu-id="e5aa7-750">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-750">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e5aa7-751">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-751">June 5, 2018</span></span>

<span data-ttu-id="e5aa7-752">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e5aa7-752">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-753">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-753">Core</span></span>

* <span data-ttu-id="e5aa7-754">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="e5aa7-754">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e5aa7-755">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-755">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-756">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-756">ACR</span></span>

* <span data-ttu-id="e5aa7-757">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-757">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e5aa7-758">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-758">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e5aa7-759">AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-759">AKS</span></span>

* <span data-ttu-id="e5aa7-760">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-760">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-761">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-761">Batch</span></span>

* <span data-ttu-id="e5aa7-762">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-762">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-763">IOT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-763">IOT</span></span>

* <span data-ttu-id="e5aa7-764">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="e5aa7-764">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-765">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-765">Network</span></span>

* <span data-ttu-id="e5aa7-766">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="e5aa7-766">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e5aa7-767">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e5aa7-767">Policy Insights</span></span>

* <span data-ttu-id="e5aa7-768">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-768">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e5aa7-769">ARM</span><span class="sxs-lookup"><span data-stu-id="e5aa7-769">ARM</span></span>

* <span data-ttu-id="e5aa7-770">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-770">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-771">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-771">SQL</span></span>

* <span data-ttu-id="e5aa7-772">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-772">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e5aa7-773">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-773">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e5aa7-774">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-774">Storage</span></span>

* <span data-ttu-id="e5aa7-775">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="e5aa7-775">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-776">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-776">VM</span></span>

* <span data-ttu-id="e5aa7-777">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-777">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e5aa7-778">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-778">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e5aa7-779">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-779">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e5aa7-780">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-780">May 22, 2018</span></span>

<span data-ttu-id="e5aa7-781">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e5aa7-781">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-782">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-782">Core</span></span>

* <span data-ttu-id="e5aa7-783">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="e5aa7-783">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-784">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-784">ACS</span></span>

* <span data-ttu-id="e5aa7-785">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-785">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e5aa7-786">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-786">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-787">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-787">AppService</span></span>

* <span data-ttu-id="e5aa7-788">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-788">Improved generic update commands</span></span>
* <span data-ttu-id="e5aa7-789">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-789">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-790">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-790">Container</span></span>

* <span data-ttu-id="e5aa7-791">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="e5aa7-791">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e5aa7-792">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-792">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-793">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-793">Extension</span></span>

* <span data-ttu-id="e5aa7-794">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-794">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-795">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-795">Interactive</span></span>

* <span data-ttu-id="e5aa7-796">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-796">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e5aa7-797">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="e5aa7-797">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-798">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-798">KeyVault</span></span>

* <span data-ttu-id="e5aa7-799">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="e5aa7-799">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-800">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-800">Network</span></span>

* <span data-ttu-id="e5aa7-801">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-801">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e5aa7-802">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-802">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-803">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-803">SQL</span></span>

* <span data-ttu-id="e5aa7-804">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-804">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e5aa7-805">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-805">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e5aa7-806">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-806">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e5aa7-807">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="e5aa7-807">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e5aa7-808">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-808">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e5aa7-809">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-809">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e5aa7-810">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-810">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e5aa7-811">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-811">`edition`.</span></span> <span data-ttu-id="e5aa7-812">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-812">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e5aa7-813">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-813">`elasticPoolName`.</span></span> <span data-ttu-id="e5aa7-814">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-814">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e5aa7-815">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-815">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e5aa7-816">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-816">`edition`.</span></span> <span data-ttu-id="e5aa7-817">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-817">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e5aa7-818">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-818">`dtu`.</span></span> <span data-ttu-id="e5aa7-819">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-819">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e5aa7-820">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-820">`databaseDtuMin`.</span></span> <span data-ttu-id="e5aa7-821">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-821">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e5aa7-822">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-822">`databaseDtuMax`.</span></span> <span data-ttu-id="e5aa7-823">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-823">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e5aa7-824">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-824">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e5aa7-825">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-825">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-826">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-826">Storage</span></span>

* <span data-ttu-id="e5aa7-827">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-827">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e5aa7-828">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-828">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-829">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-829">VM</span></span>

* <span data-ttu-id="e5aa7-830">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-830">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e5aa7-831">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-831">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e5aa7-832">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-832">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e5aa7-833">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-833">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e5aa7-834">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-834">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e5aa7-835">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-835">May 7, 2018</span></span>

<span data-ttu-id="e5aa7-836">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e5aa7-836">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-837">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-837">Core</span></span>

* <span data-ttu-id="e5aa7-838">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="e5aa7-838">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e5aa7-839">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="e5aa7-839">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e5aa7-840">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-840">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e5aa7-841">#5591</span><span class="sxs-lookup"><span data-stu-id="e5aa7-841">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e5aa7-842">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-842">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e5aa7-843">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="e5aa7-843">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e5aa7-844">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-844">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e5aa7-845">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-845">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e5aa7-846">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-846">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-847">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-847">ACR</span></span>

* <span data-ttu-id="e5aa7-848">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-848">Added ACR Build commands</span></span>
* <span data-ttu-id="e5aa7-849">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="e5aa7-849">Improved resource not found error messages</span></span>
* <span data-ttu-id="e5aa7-850">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-850">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e5aa7-851">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-851">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e5aa7-852">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="e5aa7-852">Improved repository commands error messages</span></span>
* <span data-ttu-id="e5aa7-853">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-853">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-854">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-854">ACS</span></span>

* <span data-ttu-id="e5aa7-855">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="e5aa7-855">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e5aa7-856">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="e5aa7-856">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e5aa7-857">AMS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-857">AMS</span></span>

* <span data-ttu-id="e5aa7-858">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-858">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-859">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-859">Appservice</span></span>

* <span data-ttu-id="e5aa7-860">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="e5aa7-860">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e5aa7-861">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-861">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e5aa7-862">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="e5aa7-862">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e5aa7-863">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-863">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5aa7-864">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-864">Batch AI</span></span>

* <span data-ttu-id="e5aa7-865">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="e5aa7-865">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5aa7-866">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-866">Cognitive Services</span></span>

* <span data-ttu-id="e5aa7-867">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-867">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-868">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-868">Consumption</span></span>

* <span data-ttu-id="e5aa7-869">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="e5aa7-869">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-870">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-870">Container</span></span>

* <span data-ttu-id="e5aa7-871">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-871">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5aa7-872">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-872">Cosmos DB</span></span>

* <span data-ttu-id="e5aa7-873">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-873">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e5aa7-874">DMS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-874">DMS</span></span>

* <span data-ttu-id="e5aa7-875">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="e5aa7-875">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-876">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-876">Extension</span></span>

* <span data-ttu-id="e5aa7-877">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-877">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-878">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-878">Interactive</span></span>

* <span data-ttu-id="e5aa7-879">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-879">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e5aa7-880">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="e5aa7-880">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e5aa7-881">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-881">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e5aa7-882">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-882">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e5aa7-883">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-883">Lab</span></span>

* <span data-ttu-id="e5aa7-884">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="e5aa7-884">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-885">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-885">Network</span></span>

* <span data-ttu-id="e5aa7-886">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-886">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e5aa7-887">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-887">Profile</span></span>

* <span data-ttu-id="e5aa7-888">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-888">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e5aa7-889">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-889">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e5aa7-890">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-890">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e5aa7-891">Redis</span><span class="sxs-lookup"><span data-stu-id="e5aa7-891">Redis</span></span>

* <span data-ttu-id="e5aa7-892">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-892">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e5aa7-893">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-893">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e5aa7-894">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-894">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e5aa7-895">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-895">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e5aa7-896">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-896">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-897">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-897">Role</span></span>

* <span data-ttu-id="e5aa7-898">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-898">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-899">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-899">Storage</span></span>

* <span data-ttu-id="e5aa7-900">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-900">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e5aa7-901">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="e5aa7-901">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e5aa7-902">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-902">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e5aa7-903">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-903">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e5aa7-904">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-904">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-905">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-905">VM</span></span>

* <span data-ttu-id="e5aa7-906">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-906">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e5aa7-907">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-907">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e5aa7-908">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-908">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e5aa7-909">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-909">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e5aa7-910">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-910">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e5aa7-911">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="e5aa7-911">Added write accelerator support</span></span>
* <span data-ttu-id="e5aa7-912">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-912">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e5aa7-913">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-913">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e5aa7-914">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="e5aa7-914">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e5aa7-915">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-915">April 10, 2018</span></span>

<span data-ttu-id="e5aa7-916">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e5aa7-916">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-917">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-917">ACR</span></span>

* <span data-ttu-id="e5aa7-918">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="e5aa7-918">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-919">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-919">ACS</span></span>

* <span data-ttu-id="e5aa7-920">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="e5aa7-920">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-921">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-921">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e5aa7-923">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="e5aa7-923">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e5aa7-924">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-924">BatchAI</span></span>

* <span data-ttu-id="e5aa7-925">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="e5aa7-925">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="e5aa7-926">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-926">Job level mounting</span></span>
  - <span data-ttu-id="e5aa7-927">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="e5aa7-927">Environment variables with secret values</span></span>
  - <span data-ttu-id="e5aa7-928">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="e5aa7-928">Performance counters settings</span></span>
  - <span data-ttu-id="e5aa7-929">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-929">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="e5aa7-930">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="e5aa7-930">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="e5aa7-931">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="e5aa7-931">Usage and limits reporting</span></span>
  - <span data-ttu-id="e5aa7-932">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-932">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="e5aa7-933">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-933">Support for custom images</span></span>
  - <span data-ttu-id="e5aa7-934">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-934">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e5aa7-935">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-935">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e5aa7-936">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-936">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e5aa7-937">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-937">National clouds are supported</span></span>
* <span data-ttu-id="e5aa7-938">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="e5aa7-938">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e5aa7-939">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-939">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e5aa7-940">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-940">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e5aa7-941">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-941">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e5aa7-942">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-942">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e5aa7-943">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-943">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e5aa7-944">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-944">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e5aa7-945">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-945">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e5aa7-946">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="e5aa7-946">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e5aa7-947">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-947">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e5aa7-948">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-948">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e5aa7-949">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-949">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e5aa7-950">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-950">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e5aa7-951">Facturation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-951">Billing</span></span>

* <span data-ttu-id="e5aa7-952">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="e5aa7-952">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-953">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-953">Consumption</span></span>

* <span data-ttu-id="e5aa7-954">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-954">Added `marketplace` commands</span></span>
* <span data-ttu-id="e5aa7-955">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-955">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e5aa7-956">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-956">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e5aa7-957">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-957">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e5aa7-958">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-958">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e5aa7-959">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-959">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-960">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-960">Container</span></span>

* <span data-ttu-id="e5aa7-961">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-961">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e5aa7-962">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="e5aa7-962">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-963">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-963">Extension</span></span>

* <span data-ttu-id="e5aa7-964">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-964">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-965">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-965">Interactive</span></span>

* <span data-ttu-id="e5aa7-966">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="e5aa7-966">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e5aa7-967">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-967">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e5aa7-968">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-968">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-969">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-969">Network</span></span>

* <span data-ttu-id="e5aa7-970">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="e5aa7-970">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e5aa7-971">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-971">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e5aa7-972">#4910</span><span class="sxs-lookup"><span data-stu-id="e5aa7-972">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e5aa7-973">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-973">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e5aa7-974">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-974">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e5aa7-975">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-975">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e5aa7-976">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-976">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e5aa7-977">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-977">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-978">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-978">Profile</span></span>

* <span data-ttu-id="e5aa7-979">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-979">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e5aa7-980">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-980">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-981">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-981">RDBMS</span></span>

* <span data-ttu-id="e5aa7-982">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-982">Added `georestore` command</span></span>
* <span data-ttu-id="e5aa7-983">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-983">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-984">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-984">Resource</span></span>

* <span data-ttu-id="e5aa7-985">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-985">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e5aa7-986">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-986">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-987">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-987">SQL</span></span>

* <span data-ttu-id="e5aa7-988">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-988">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-989">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-989">Storage</span></span>

* <span data-ttu-id="e5aa7-990">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-990">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-991">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-991">VM</span></span>

* <span data-ttu-id="e5aa7-992">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-992">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e5aa7-993">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-993">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e5aa7-995">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-995">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e5aa7-996">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-996">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e5aa7-997">#5718</span><span class="sxs-lookup"><span data-stu-id="e5aa7-997">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e5aa7-998">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="e5aa7-998">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e5aa7-999">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-999">March 27, 2018</span></span>

<span data-ttu-id="e5aa7-1000">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1000">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1001">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1001">Core</span></span>

* <span data-ttu-id="e5aa7-1002">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1002">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1003">ACS</span></span>

* <span data-ttu-id="e5aa7-1004">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1004">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1005">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1005">Appservice</span></span>

* <span data-ttu-id="e5aa7-1006">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1006">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e5aa7-1007">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1007">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e5aa7-1008">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1008">Backup</span></span>

* <span data-ttu-id="e5aa7-1009">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1009">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e5aa7-1010">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1010">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e5aa7-1011">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1011">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e5aa7-1012">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1012">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1013">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1013">Container</span></span>

* <span data-ttu-id="e5aa7-1014">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1014">Added `container exec` command.</span></span> <span data-ttu-id="e5aa7-1015">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1015">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e5aa7-1016">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1016">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-1017">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1017">Extension</span></span>

* <span data-ttu-id="e5aa7-1018">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1018">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e5aa7-1019">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1019">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e5aa7-1020">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1020">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1021">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1021">Interactive</span></span>

* <span data-ttu-id="e5aa7-1022">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1022">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e5aa7-1023">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1023">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e5aa7-1024">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1024">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e5aa7-1025">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1025">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e5aa7-1026">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1026">Lab</span></span>

* <span data-ttu-id="e5aa7-1027">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1027">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1028">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1028">Monitor</span></span>

* <span data-ttu-id="e5aa7-1029">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1029">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e5aa7-1030">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1030">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e5aa7-1031">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1031">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1032">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1032">Network</span></span>

* <span data-ttu-id="e5aa7-1033">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1033">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1034">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1034">Profile</span></span>

* <span data-ttu-id="e5aa7-1035">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1035">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-1036">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1036">RDBMS</span></span>

* <span data-ttu-id="e5aa7-1037">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1037">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1038">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1038">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e5aa7-1040">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1040">Role</span></span>

* <span data-ttu-id="e5aa7-1041">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1041">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e5aa7-1042">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1042">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e5aa7-1043">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1043">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e5aa7-1044">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1044">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e5aa7-1045">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1045">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1046">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1046">Storage</span></span>

* <span data-ttu-id="e5aa7-1047">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1047">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e5aa7-1048">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1048">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1049">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1049">VM</span></span>

* <span data-ttu-id="e5aa7-1050">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1050">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e5aa7-1051">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1051">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e5aa7-1052">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1052">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e5aa7-1053">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1053">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e5aa7-1054">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1054">March 13, 2018</span></span>

<span data-ttu-id="e5aa7-1055">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1055">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-1056">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1056">ACR</span></span>

* <span data-ttu-id="e5aa7-1057">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1057">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e5aa7-1058">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1058">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e5aa7-1059">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1059">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1060">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1060">ACS</span></span>

* <span data-ttu-id="e5aa7-1061">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1061">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e5aa7-1062">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1062">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e5aa7-1063">Advisor</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1063">Advisor</span></span>

* <span data-ttu-id="e5aa7-1064">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1064">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e5aa7-1065">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1065">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e5aa7-1066">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1066">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e5aa7-1067">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1067">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e5aa7-1068">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1068">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1069">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1069">Appservice</span></span>

* <span data-ttu-id="e5aa7-1070">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1070">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e5aa7-1071">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1071">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e5aa7-1072">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1072">Eventhubs</span></span>

* <span data-ttu-id="e5aa7-1073">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1073">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-1074">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1074">Extension</span></span>

* <span data-ttu-id="e5aa7-1075">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1075">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1076">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1076">Interactive</span></span>

* <span data-ttu-id="e5aa7-1077">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1077">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e5aa7-1078">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1078">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e5aa7-1079">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1079">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e5aa7-1080">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1080">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1081">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1081">Monitor</span></span>

* <span data-ttu-id="e5aa7-1082">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1082">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e5aa7-1083">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1083">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e5aa7-1084">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1084">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e5aa7-1085">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1085">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1086">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1086">Network</span></span>

* <span data-ttu-id="e5aa7-1087">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1087">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e5aa7-1088">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1088">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e5aa7-1089">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1089">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e5aa7-1090">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1090">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1091">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1091">Profile</span></span>

* <span data-ttu-id="e5aa7-1092">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1092">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e5aa7-1093">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1093">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-1094">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1094">RDBMS</span></span>

* <span data-ttu-id="e5aa7-1095">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1095">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5aa7-1096">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1096">Service Bus</span></span>

* <span data-ttu-id="e5aa7-1097">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1097">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1098">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1098">Storage</span></span>

* <span data-ttu-id="e5aa7-1099">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1099">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e5aa7-1100">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1100">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1101">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1101">VM</span></span>

* <span data-ttu-id="e5aa7-1102">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1102">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e5aa7-1103">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1103">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e5aa7-1104">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1104">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e5aa7-1105">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1105">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e5aa7-1106">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1106">February 27, 2018</span></span>

<span data-ttu-id="e5aa7-1107">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1107">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1108">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1108">Core</span></span>

* <span data-ttu-id="e5aa7-1109">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1109">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e5aa7-1110">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1110">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e5aa7-1111">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1111">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1112">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1112">ACS</span></span>

* <span data-ttu-id="e5aa7-1113">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1113">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e5aa7-1114">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1114">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e5aa7-1115">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1115">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e5aa7-1116">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1116">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1117">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1117">Appservice</span></span>

* <span data-ttu-id="e5aa7-1118">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1118">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e5aa7-1119">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1119">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5aa7-1120">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1120">Cognitive Services</span></span>

* <span data-ttu-id="e5aa7-1121">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1121">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-1122">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1122">Consumption</span></span>

* <span data-ttu-id="e5aa7-1123">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1123">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e5aa7-1124">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1124">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1125">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1125">Container</span></span>

* <span data-ttu-id="e5aa7-1126">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1126">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1127">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1127">Network</span></span>

* <span data-ttu-id="e5aa7-1128">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1128">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1129">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1129">Resource</span></span>

* <span data-ttu-id="e5aa7-1130">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1130">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1131">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1131">Role</span></span>

* <span data-ttu-id="e5aa7-1132">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1132">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1133">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1133">SQL</span></span>

* <span data-ttu-id="e5aa7-1134">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1134">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1135">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1135">Storage</span></span>

* <span data-ttu-id="e5aa7-1136">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1136">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1137">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1137">VM</span></span>

* <span data-ttu-id="e5aa7-1138">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1138">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e5aa7-1139">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1139">February 13, 2018</span></span>

<span data-ttu-id="e5aa7-1140">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1140">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1141">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1141">Core</span></span>

* <span data-ttu-id="e5aa7-1142">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1142">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1143">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1143">ACS</span></span>

* <span data-ttu-id="e5aa7-1144">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1144">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e5aa7-1145">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1145">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e5aa7-1146">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1146">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e5aa7-1147">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1147">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e5aa7-1148">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1148">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e5aa7-1149">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1149">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e5aa7-1150">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1150">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e5aa7-1151">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1151">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1152">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1152">Appservice</span></span>

* <span data-ttu-id="e5aa7-1153">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1153">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e5aa7-1154">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1154">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e5aa7-1155">CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1155">CDN</span></span>

* <span data-ttu-id="e5aa7-1156">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1156">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1157">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1157">Container</span></span>

* <span data-ttu-id="e5aa7-1158">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1158">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e5aa7-1159">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1159">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-1160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1160">CosmosDB</span></span>

* <span data-ttu-id="e5aa7-1161">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1161">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-1162">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1162">Extension</span></span>

* <span data-ttu-id="e5aa7-1163">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1163">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e5aa7-1164">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1164">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e5aa7-1165">Commentaires</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1165">Feedback</span></span>

* <span data-ttu-id="e5aa7-1166">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1166">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1167">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1167">Interactive</span></span>

* <span data-ttu-id="e5aa7-1168">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1168">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e5aa7-1169">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1169">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-1170">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1170">IoT</span></span>

* <span data-ttu-id="e5aa7-1171">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1171">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e5aa7-1172">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1172">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e5aa7-1173">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1173">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1174">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1174">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1175">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1175">Monitor</span></span>

* <span data-ttu-id="e5aa7-1176">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1176">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1177">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1177">Network</span></span>

* <span data-ttu-id="e5aa7-1178">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1178">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e5aa7-1179">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1179">Profile</span></span>

* <span data-ttu-id="e5aa7-1180">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1180">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1181">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1181">Resource</span></span>

* <span data-ttu-id="e5aa7-1182">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1182">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1183">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1183">Role</span></span>

* <span data-ttu-id="e5aa7-1184">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1184">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1185">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1185">SQL</span></span>

* <span data-ttu-id="e5aa7-1186">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1186">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e5aa7-1187">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1187">Added `sql db rename`</span></span>
* <span data-ttu-id="e5aa7-1188">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1188">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1189">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1189">Storage</span></span>

* <span data-ttu-id="e5aa7-1190">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1190">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1191">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1191">VM</span></span>

* <span data-ttu-id="e5aa7-1192">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1192">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e5aa7-1193">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1193">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e5aa7-1194">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1194">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e5aa7-1195">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1195">January 31, 2018</span></span>

<span data-ttu-id="e5aa7-1196">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1196">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1197">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1197">Core</span></span>

* <span data-ttu-id="e5aa7-1198">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1198">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e5aa7-1199">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1199">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e5aa7-1200">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1200">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e5aa7-1201">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1201">Use `--verbose` to see</span></span>
* <span data-ttu-id="e5aa7-1202">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1202">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1203">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1203">ACS</span></span>

* <span data-ttu-id="e5aa7-1204">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1204">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e5aa7-1205">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1205">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1206">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1206">Appservice</span></span>

* <span data-ttu-id="e5aa7-1207">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1207">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e5aa7-1208">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1208">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e5aa7-1209">CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1209">CDN</span></span>

* <span data-ttu-id="e5aa7-1210">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1210">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-1211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1211">CosmosDB</span></span>

* <span data-ttu-id="e5aa7-1212">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1212">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1213">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1213">Interactive</span></span>

* <span data-ttu-id="e5aa7-1214">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1214">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1215">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1215">Network</span></span>

* <span data-ttu-id="e5aa7-1216">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1216">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e5aa7-1217">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1217">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e5aa7-1218">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1218">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e5aa7-1219">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1219">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e5aa7-1220">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1220">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e5aa7-1221">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1221">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e5aa7-1222">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1222">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e5aa7-1223">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1223">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e5aa7-1224">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1224">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e5aa7-1225">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1225">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1226">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1226">Profile</span></span>

* <span data-ttu-id="e5aa7-1227">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1227">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1228">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1228">Resource</span></span>

* <span data-ttu-id="e5aa7-1229">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1229">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1230">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1230">Storage</span></span>

* <span data-ttu-id="e5aa7-1231">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1231">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e5aa7-1232">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1232">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e5aa7-1233">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1233">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e5aa7-1234">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1234">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e5aa7-1235">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1235">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1236">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1236">VM</span></span>

* <span data-ttu-id="e5aa7-1237">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1237">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e5aa7-1238">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1238">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e5aa7-1239">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1239">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e5aa7-1240">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1240">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e5aa7-1241">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1241">January 17, 2018</span></span>

<span data-ttu-id="e5aa7-1242">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1242">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-1243">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1243">ACR</span></span>

* <span data-ttu-id="e5aa7-1244">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1244">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e5aa7-1245">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1245">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1246">ACS</span></span>

* <span data-ttu-id="e5aa7-1247">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1247">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e5aa7-1248">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1248">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1249">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1249">Appservice</span></span>

* <span data-ttu-id="e5aa7-1250">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1250">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e5aa7-1251">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1251">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e5aa7-1252">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1252">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e5aa7-1253">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1253">Backup</span></span>

* <span data-ttu-id="e5aa7-1254">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1254">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e5aa7-1255">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1255">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e5aa7-1256">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1256">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e5aa7-1257">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1257">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e5aa7-1258">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1258">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-1259">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1259">Batch</span></span>

* <span data-ttu-id="e5aa7-1260">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1260">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e5aa7-1261">Cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1261">Cloud</span></span>

* <span data-ttu-id="e5aa7-1262">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1262">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-1263">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1263">Consumption</span></span>

* <span data-ttu-id="e5aa7-1264">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1264">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5aa7-1265">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1265">Event Grid</span></span>

* <span data-ttu-id="e5aa7-1266">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1266">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e5aa7-1267">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1267">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e5aa7-1268">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1268">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e5aa7-1269">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1269">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e5aa7-1270">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1270">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e5aa7-1271">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1271">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e5aa7-1272">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1272">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e5aa7-1273">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1273">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1274">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1274">Interactive</span></span>

* <span data-ttu-id="e5aa7-1275">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1275">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e5aa7-1276">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1276">Fixed errors on startup</span></span>
* <span data-ttu-id="e5aa7-1277">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1277">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-1278">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1278">IoT</span></span>

* <span data-ttu-id="e5aa7-1279">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1279">Added support for device provisioning service</span></span>
* <span data-ttu-id="e5aa7-1280">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1280">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e5aa7-1281">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1281">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1282">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1282">Monitor</span></span>

* <span data-ttu-id="e5aa7-1283">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1283">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e5aa7-1284">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1284">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e5aa7-1285">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1285">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1286">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1286">Network</span></span>

* <span data-ttu-id="e5aa7-1287">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1287">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e5aa7-1288">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1288">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1289">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1289">Profile</span></span>

* <span data-ttu-id="e5aa7-1290">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1290">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1291">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1291">Role</span></span>

* <span data-ttu-id="e5aa7-1292">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1292">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5aa7-1293">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1293">Service Fabric</span></span>

* <span data-ttu-id="e5aa7-1294">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1294">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e5aa7-1295">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1295">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1296">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1296">VM</span></span>

* <span data-ttu-id="e5aa7-1297">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1297">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e5aa7-1298">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1298">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e5aa7-1299">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1299">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e5aa7-1300">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1300">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e5aa7-1301">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1301">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e5aa7-1302">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1302">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5aa7-1303">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1303">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5aa7-1304">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1304">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e5aa7-1305">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1305">December 19, 2017</span></span>

<span data-ttu-id="e5aa7-1306">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1306">Version 2.0.23</span></span>

* <span data-ttu-id="e5aa7-1307">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1307">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1308">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1308">Container</span></span>

* <span data-ttu-id="e5aa7-1309">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1309">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1310">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1310">Network</span></span>

* <span data-ttu-id="e5aa7-1311">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1311">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1312">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1312">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1313">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1313">Storage</span></span>

* <span data-ttu-id="e5aa7-1314">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1314">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1315">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1315">VM</span></span>

* <span data-ttu-id="e5aa7-1316">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1316">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e5aa7-1317">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1317">December 5, 2017</span></span>

<span data-ttu-id="e5aa7-1318">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1318">Version 2.0.22</span></span>

* <span data-ttu-id="e5aa7-1319">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1319">Removed `az component` commands.</span></span> <span data-ttu-id="e5aa7-1320">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1320">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1321">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1321">Core</span></span>
* <span data-ttu-id="e5aa7-1322">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1322">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e5aa7-1323">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1323">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1324">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1324">ACS</span></span>

* <span data-ttu-id="e5aa7-1325">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1325">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e5aa7-1326">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1326">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e5aa7-1327">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1327">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e5aa7-1328">Advisor</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1328">Advisor</span></span>

* <span data-ttu-id="e5aa7-1329">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1329">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1330">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1330">Appservice</span></span>

* <span data-ttu-id="e5aa7-1331">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1331">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e5aa7-1332">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1332">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e5aa7-1333">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1333">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e5aa7-1334">Consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1334">Consumption</span></span>

* <span data-ttu-id="e5aa7-1335">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1335">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1336">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1336">Container</span></span>

* <span data-ttu-id="e5aa7-1337">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1337">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1338">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1338">Monitor</span></span>

* <span data-ttu-id="e5aa7-1339">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1339">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1340">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1340">Resource</span></span>

* <span data-ttu-id="e5aa7-1341">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1341">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1342">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1342">Role</span></span>

* <span data-ttu-id="e5aa7-1343">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1343">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e5aa7-1344">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1344">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e5aa7-1345">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1345">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1346">SQL</span></span>

* <span data-ttu-id="e5aa7-1347">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1347">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e5aa7-1348">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1348">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1349">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1349">VM</span></span>

* <span data-ttu-id="e5aa7-1350">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1350">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e5aa7-1351">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1351">November 14, 2017</span></span>

<span data-ttu-id="e5aa7-1352">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1352">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-1353">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1353">ACR</span></span>

* <span data-ttu-id="e5aa7-1354">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1354">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e5aa7-1355">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1355">ACS</span></span>

* <span data-ttu-id="e5aa7-1356">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1356">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e5aa7-1357">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1357">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e5aa7-1358">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1358">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e5aa7-1359">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1359">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e5aa7-1360">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1360">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1361">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1361">Appservice</span></span>

* <span data-ttu-id="e5aa7-1362">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1362">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e5aa7-1363">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1363">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e5aa7-1364">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1364">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e5aa7-1365">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1365">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e5aa7-1366">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1366">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e5aa7-1367">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1367">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-1368">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1368">Batch</span></span>

* <span data-ttu-id="e5aa7-1369">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1369">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e5aa7-1370">Batchai</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1370">Batchai</span></span>

* <span data-ttu-id="e5aa7-1371">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1371">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e5aa7-1372">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1372">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e5aa7-1373">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1373">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e5aa7-1374">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1374">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e5aa7-1375">Cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1375">Cloud</span></span>

* <span data-ttu-id="e5aa7-1376">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1376">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1377">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1377">Container</span></span>

* <span data-ttu-id="e5aa7-1378">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1378">Added support to open multiple ports</span></span>
* <span data-ttu-id="e5aa7-1379">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1379">Added container group restart policy</span></span>
* <span data-ttu-id="e5aa7-1380">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1380">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e5aa7-1381">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1381">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5aa7-1382">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1382">Data Lake Analytics</span></span>

* <span data-ttu-id="e5aa7-1383">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1383">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5aa7-1384">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1384">Data Lake Store</span></span>

* <span data-ttu-id="e5aa7-1385">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1385">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-1386">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1386">Extension</span></span>

* <span data-ttu-id="e5aa7-1387">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1387">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e5aa7-1388">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1388">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-1389">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1389">IoT</span></span>

* <span data-ttu-id="e5aa7-1390">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1390">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1391">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1391">Monitor</span></span>

* <span data-ttu-id="e5aa7-1392">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1392">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1393">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1393">Network</span></span>

* <span data-ttu-id="e5aa7-1394">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1394">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e5aa7-1395">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1395">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e5aa7-1396">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1396">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e5aa7-1397">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1397">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e5aa7-1398">Réservations</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1398">Reservations</span></span>

* <span data-ttu-id="e5aa7-1399">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1399">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1400">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1400">Resource</span></span>

* <span data-ttu-id="e5aa7-1401">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1401">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1402">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1402">SQL</span></span>

* <span data-ttu-id="e5aa7-1403">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1403">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1404">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1404">Storage</span></span>

* <span data-ttu-id="e5aa7-1405">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1405">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e5aa7-1406">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1406">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e5aa7-1407">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1407">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e5aa7-1408">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1408">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e5aa7-1409">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1409">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e5aa7-1410">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1410">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e5aa7-1411">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1411">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1412">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1412">VM</span></span>

* <span data-ttu-id="e5aa7-1413">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1413">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e5aa7-1414">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1414">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e5aa7-1415">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1415">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e5aa7-1416">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1416">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e5aa7-1417">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1417">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e5aa7-1418">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1418">October 24, 2017</span></span>

<span data-ttu-id="e5aa7-1419">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1419">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1420">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1420">Core</span></span>

* <span data-ttu-id="e5aa7-1421">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1421">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1422">ACR</span></span>

* <span data-ttu-id="e5aa7-1423">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1423">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e5aa7-1424">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1424">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e5aa7-1425">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1425">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1426">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1426">ACS</span></span>

* <span data-ttu-id="e5aa7-1427">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1427">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e5aa7-1428">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1428">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1429">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1429">Appservice</span></span>

* <span data-ttu-id="e5aa7-1430">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1430">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e5aa7-1431">Composant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1431">Component</span></span>

* <span data-ttu-id="e5aa7-1432">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1432">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1433">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1433">Monitor</span></span>

* <span data-ttu-id="e5aa7-1434">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1434">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1435">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1435">Resource</span></span>

* <span data-ttu-id="e5aa7-1436">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1436">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e5aa7-1437">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1437">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1438">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1438">VM</span></span>

* <span data-ttu-id="e5aa7-1439">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1439">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e5aa7-1440">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1440">October 9, 2017</span></span>

<span data-ttu-id="e5aa7-1441">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1441">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1442">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1442">Core</span></span>

* <span data-ttu-id="e5aa7-1443">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1443">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1444">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1444">Appservice</span></span>

* <span data-ttu-id="e5aa7-1445">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1445">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-1446">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1446">Batch</span></span>

* <span data-ttu-id="e5aa7-1447">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1447">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e5aa7-1448">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1448">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e5aa7-1449">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1449">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e5aa7-1450">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1450">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e5aa7-1451">Batchai</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1451">Batchai</span></span>

* <span data-ttu-id="e5aa7-1452">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1452">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-1453">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1453">Keyvault</span></span>

* <span data-ttu-id="e5aa7-1454">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1454">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e5aa7-1455">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1455">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e5aa7-1456">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1456">Network</span></span>

* <span data-ttu-id="e5aa7-1457">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1457">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e5aa7-1458">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1458">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1459">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1459">Resource</span></span>

* <span data-ttu-id="e5aa7-1460">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1460">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e5aa7-1461">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1461">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e5aa7-1462">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1462">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e5aa7-1463">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1463">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1464">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1464">Sql</span></span>

* <span data-ttu-id="e5aa7-1465">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1465">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e5aa7-1466">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1466">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e5aa7-1467">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1467">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1468">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1468">Storage</span></span>

* <span data-ttu-id="e5aa7-1469">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1469">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1470">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1470">Vm</span></span>

* <span data-ttu-id="e5aa7-1471">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1471">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e5aa7-1472">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1472">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e5aa7-1473">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1473">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e5aa7-1474">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1474">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e5aa7-1475">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1475">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e5aa7-1476">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1476">September 22, 2017</span></span>

<span data-ttu-id="e5aa7-1477">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1477">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1478">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1478">Resource</span></span>

* <span data-ttu-id="e5aa7-1479">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1479">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e5aa7-1480">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1480">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e5aa7-1481">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1481">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e5aa7-1482">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1482">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1483">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1483">Network</span></span>

* <span data-ttu-id="e5aa7-1484">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1484">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e5aa7-1485">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1485">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e5aa7-1486">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1486">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e5aa7-1487">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1487">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e5aa7-1488">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1488">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1489">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1489">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1490">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1490">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1491">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1491">Storage</span></span>

* <span data-ttu-id="e5aa7-1492">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1492">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5aa7-1493">Événement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1493">Eventgrid</span></span>

* <span data-ttu-id="e5aa7-1494">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1494">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1495">SQL</span></span>

* <span data-ttu-id="e5aa7-1496">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1496">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e5aa7-1497">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1497">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e5aa7-1498">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1498">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-1499">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1499">Keyvault</span></span>

* <span data-ttu-id="e5aa7-1500">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1500">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1501">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1501">VM</span></span>

* <span data-ttu-id="e5aa7-1502">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1502">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e5aa7-1503">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1503">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e5aa7-1504">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1504">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e5aa7-1505">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1505">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e5aa7-1506">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1506">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e5aa7-1507">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1507">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1508">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1508">ACS</span></span>

* <span data-ttu-id="e5aa7-1509">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1509">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1510">Appservice</span></span>

* <span data-ttu-id="e5aa7-1511">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1511">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e5aa7-1512">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1512">Backup</span></span>

* <span data-ttu-id="e5aa7-1513">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1513">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e5aa7-1514">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1514">September 11, 2017</span></span>

<span data-ttu-id="e5aa7-1515">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1515">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e5aa7-1516">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1516">Core</span></span>

* <span data-ttu-id="e5aa7-1517">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1517">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e5aa7-1518">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1518">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1519">Acs</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1519">Acs</span></span>

* <span data-ttu-id="e5aa7-1520">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1520">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e5aa7-1521">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1521">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1522">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1522">Appservice</span></span>

* <span data-ttu-id="e5aa7-1523">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1523">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e5aa7-1524">CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1524">CDN</span></span>

* <span data-ttu-id="e5aa7-1525">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1525">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e5aa7-1526">Extension</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1526">Extension</span></span>

* <span data-ttu-id="e5aa7-1527">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1527">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-1528">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1528">Keyvault</span></span>

* <span data-ttu-id="e5aa7-1529">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1529">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1530">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1530">Network</span></span>

* <span data-ttu-id="e5aa7-1531">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1531">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e5aa7-1532">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1532">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e5aa7-1533">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1533">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e5aa7-1534">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1534">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e5aa7-1535">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1535">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1536">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1536">Resource</span></span>

* <span data-ttu-id="e5aa7-1537">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1537">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e5aa7-1538">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1538">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e5aa7-1539">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1539">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e5aa7-1540">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1540">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1541">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1541">SQL</span></span>

* <span data-ttu-id="e5aa7-1542">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1542">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1543">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1543">VM</span></span>

* <span data-ttu-id="e5aa7-1544">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1544">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e5aa7-1545">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1545">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e5aa7-1546">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1546">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e5aa7-1547">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1547">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e5aa7-1548">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1548">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e5aa7-1549">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1549">August 31, 2017</span></span>

<span data-ttu-id="e5aa7-1550">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1550">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-1551">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1551">Keyvault</span></span>

* <span data-ttu-id="e5aa7-1552">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1552">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e5aa7-1553">Sf</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1553">Sf</span></span>

* <span data-ttu-id="e5aa7-1554">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1554">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1555">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1555">Storage</span></span>

* <span data-ttu-id="e5aa7-1556">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1556">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e5aa7-1557">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1557">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e5aa7-1558">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1558">August 28, 2017</span></span>

<span data-ttu-id="e5aa7-1559">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1559">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e5aa7-1560">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1560">CLI</span></span>

* <span data-ttu-id="e5aa7-1561">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1561">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1562">ACS</span></span>

* <span data-ttu-id="e5aa7-1563">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1563">Corrected preview regions</span></span>
* <span data-ttu-id="e5aa7-1564">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1564">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e5aa7-1565">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1565">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1566">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1566">Appservice</span></span>

* <span data-ttu-id="e5aa7-1567">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1567">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e5aa7-1568">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1568">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e5aa7-1569">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1569">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e5aa7-1570">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1570">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e5aa7-1571">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1571">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-1572">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1572">IoT</span></span>

* <span data-ttu-id="e5aa7-1573">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1573">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1574">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1574">Network</span></span>

* <span data-ttu-id="e5aa7-1575">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1575">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e5aa7-1576">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1576">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1577">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1577">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e5aa7-1578">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1578">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e5aa7-1579">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1579">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1580">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1580">Profile</span></span>

* <span data-ttu-id="e5aa7-1581">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1581">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5aa7-1582">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1582">Service Fabric</span></span>

* <span data-ttu-id="e5aa7-1583">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1583">Preview release</span></span>
* <span data-ttu-id="e5aa7-1584">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1584">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e5aa7-1585">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1585">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e5aa7-1586">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1586">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1587">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1587">Storage</span></span>

* <span data-ttu-id="e5aa7-1588">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1588">Enabled setting blob tier</span></span>
* <span data-ttu-id="e5aa7-1589">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1589">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e5aa7-1590">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1590">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e5aa7-1591">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1591">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e5aa7-1592">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1592">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e5aa7-1593">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1593">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1594">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1594">VM</span></span>

* <span data-ttu-id="e5aa7-1595">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1595">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e5aa7-1596">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1596">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e5aa7-1597">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1597">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5aa7-1598">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1598">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e5aa7-1599">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1599">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e5aa7-1600">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1600">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e5aa7-1601">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1601">August 15, 2017</span></span>

<span data-ttu-id="e5aa7-1602">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1602">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1603">ACS</span></span>

* <span data-ttu-id="e5aa7-1604">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1604">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1605">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1605">Appservice</span></span>

* <span data-ttu-id="e5aa7-1606">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1606">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5aa7-1607">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1607">Event Grid</span></span>

* <span data-ttu-id="e5aa7-1608">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1608">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e5aa7-1609">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1609">August 11, 2017</span></span>

<span data-ttu-id="e5aa7-1610">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1610">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1611">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1611">ACS</span></span>

* <span data-ttu-id="e5aa7-1612">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1612">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-1613">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1613">Batch</span></span>

* <span data-ttu-id="e5aa7-1614">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1614">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e5aa7-1615">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1615">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e5aa7-1616">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1616">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e5aa7-1617">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1617">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e5aa7-1618">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1618">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e5aa7-1619">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1619">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e5aa7-1620">Composant</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1620">Component</span></span>

* <span data-ttu-id="e5aa7-1621">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1621">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e5aa7-1622">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1622">Container</span></span>

* <span data-ttu-id="e5aa7-1623">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1623">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e5aa7-1624">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1624">Data Lake Store</span></span>

* <span data-ttu-id="e5aa7-1625">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1625">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5aa7-1626">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1626">Event Grid</span></span>

* <span data-ttu-id="e5aa7-1627">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1627">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1628">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1628">Network</span></span>

* <span data-ttu-id="e5aa7-1629">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1629">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e5aa7-1630">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1630">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e5aa7-1631">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1631">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e5aa7-1632">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1632">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1633">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1633">Profile</span></span>

* <span data-ttu-id="e5aa7-1634">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1634">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1635">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1635">Storage</span></span>

* <span data-ttu-id="e5aa7-1636">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1636">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1637">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1637">VM</span></span>

* <span data-ttu-id="e5aa7-1638">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1638">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e5aa7-1639">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1639">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e5aa7-1640">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1640">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e5aa7-1641">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1641">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e5aa7-1642">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1642">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e5aa7-1643">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1643">July 28, 2017</span></span>

<span data-ttu-id="e5aa7-1644">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1644">Version 2.0.12</span></span>

* <span data-ttu-id="e5aa7-1645">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1645">Added container commands</span></span>
* <span data-ttu-id="e5aa7-1646">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1646">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e5aa7-1647">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1647">Core</span></span>

* <span data-ttu-id="e5aa7-1648">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1648">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e5aa7-1649">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1649">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e5aa7-1650">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1650">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e5aa7-1651">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1651">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e5aa7-1652">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1652">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e5aa7-1653">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1653">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e5aa7-1654">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1654">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e5aa7-1655">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1655">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e5aa7-1656">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1656">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e5aa7-1657">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1657">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e5aa7-1658">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1658">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e5aa7-1659">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1659">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e5aa7-1660">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1660">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e5aa7-1661">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1661">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e5aa7-1662">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1662">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e5aa7-1663">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1663">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e5aa7-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1664">ACR</span></span>

* <span data-ttu-id="e5aa7-1665">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1665">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e5aa7-1666">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1666">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e5aa7-1667">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1667">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e5aa7-1668">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1668">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e5aa7-1669">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1669">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e5aa7-1670">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1670">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1671">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1671">ACS</span></span>

* <span data-ttu-id="e5aa7-1672">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1672">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1673">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1673">Appservice</span></span>

* <span data-ttu-id="e5aa7-1674">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1674">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e5aa7-1675">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1675">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e5aa7-1676">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1676">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e5aa7-1677">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1677">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e5aa7-1678">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1678">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e5aa7-1679">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1679">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e5aa7-1680">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1680">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e5aa7-1681">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1681">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e5aa7-1682">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1682">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e5aa7-1683">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1683">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e5aa7-1684">Batch</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1684">Batch</span></span>

* <span data-ttu-id="e5aa7-1685">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1685">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e5aa7-1686">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1686">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e5aa7-1687">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1687">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e5aa7-1688">CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1688">CDN</span></span>

* <span data-ttu-id="e5aa7-1689">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1689">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e5aa7-1690">Cloud</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1690">Cloud</span></span>

* <span data-ttu-id="e5aa7-1691">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1691">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e5aa7-1692">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1692">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e5aa7-1693">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1693">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e5aa7-1694">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1694">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e5aa7-1695">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1695">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-1696">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1696">CosmosDB</span></span>

* <span data-ttu-id="e5aa7-1697">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1697">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e5aa7-1698">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1698">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5aa7-1699">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1699">Data Lake Analytics</span></span>

* <span data-ttu-id="e5aa7-1700">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1700">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e5aa7-1701">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1701">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e5aa7-1702">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1702">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5aa7-1703">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1703">Data Lake Store</span></span>

* <span data-ttu-id="e5aa7-1704">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1704">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e5aa7-1705">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1705">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e5aa7-1706">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1706">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e5aa7-1707">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1707">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e5aa7-1708">Interactive</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1708">Interactive</span></span>

* <span data-ttu-id="e5aa7-1709">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1709">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e5aa7-1710">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1710">Increased test coverage</span></span>
* <span data-ttu-id="e5aa7-1711">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1711">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e5aa7-1712">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1712">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e5aa7-1713">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1713">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e5aa7-1714">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1714">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e5aa7-1715">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1715">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e5aa7-1716">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1716">Added `--progress` flag</span></span>
* <span data-ttu-id="e5aa7-1717">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1717">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e5aa7-1718">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1718">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e5aa7-1719">IoT</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1719">IoT</span></span>

* <span data-ttu-id="e5aa7-1720">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1720">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e5aa7-1721">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1721">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5aa7-1722">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1722">Key vault</span></span>

* <span data-ttu-id="e5aa7-1723">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1723">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e5aa7-1724">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1724">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e5aa7-1725">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1725">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e5aa7-1726">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1726">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e5aa7-1727">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1727">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e5aa7-1728">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1728">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e5aa7-1729">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1729">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e5aa7-1730">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1730">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e5aa7-1731">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1731">Lab</span></span>

* <span data-ttu-id="e5aa7-1732">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1732">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e5aa7-1733">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1733">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1734">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1734">Monitor</span></span>

* <span data-ttu-id="e5aa7-1735">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1735">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e5aa7-1736">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1736">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e5aa7-1737">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1737">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e5aa7-1738">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1738">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e5aa7-1739">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1739">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e5aa7-1740">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1740">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e5aa7-1741">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1741">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e5aa7-1742">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1742">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e5aa7-1743">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1743">`location` no longer required</span></span>
  * <span data-ttu-id="e5aa7-1744">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1744">Add name and ID support for target</span></span>
  * <span data-ttu-id="e5aa7-1745">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1745">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e5aa7-1746">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1746">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e5aa7-1747">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1747">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e5aa7-1748">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1748">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e5aa7-1749">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1749">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e5aa7-1750">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1750">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1751">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1751">Network</span></span>

* <span data-ttu-id="e5aa7-1752">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1752">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e5aa7-1753">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1753">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e5aa7-1754">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1754">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e5aa7-1755">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1755">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e5aa7-1756">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1756">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e5aa7-1757">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1757">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e5aa7-1758">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1758">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e5aa7-1759">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1759">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e5aa7-1760">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1760">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e5aa7-1761">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1761">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e5aa7-1762">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1762">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e5aa7-1763">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1763">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e5aa7-1764">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1764">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e5aa7-1765">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1765">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e5aa7-1766">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1766">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e5aa7-1767">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1767">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e5aa7-1768">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1768">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e5aa7-1769">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1769">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e5aa7-1770">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1770">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e5aa7-1771">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1771">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e5aa7-1772">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1772">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e5aa7-1773">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1773">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e5aa7-1774">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1774">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e5aa7-1775">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1775">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e5aa7-1776">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1776">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e5aa7-1777">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1777">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e5aa7-1778">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1778">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1779">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1779">Profile</span></span>

* <span data-ttu-id="e5aa7-1780">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1780">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e5aa7-1781">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1781">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e5aa7-1782">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1782">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e5aa7-1783">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1783">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e5aa7-1784">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1784">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5aa7-1785">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1785">RDBMS</span></span>

* <span data-ttu-id="e5aa7-1786">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1786">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e5aa7-1787">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1787">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e5aa7-1788">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1788">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e5aa7-1789">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1789">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1790">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1790">Resource</span></span>

* <span data-ttu-id="e5aa7-1791">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1791">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e5aa7-1792">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1792">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e5aa7-1793">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1793">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e5aa7-1794">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1794">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e5aa7-1795">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1795">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e5aa7-1796">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1796">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e5aa7-1797">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1797">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e5aa7-1798">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1798">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1799">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1799">Role</span></span>

* <span data-ttu-id="e5aa7-1800">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1800">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e5aa7-1801">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1801">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e5aa7-1802">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1802">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e5aa7-1803">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1803">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e5aa7-1804">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1804">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5aa7-1805">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1805">Service Fabric</span></span>
* <span data-ttu-id="e5aa7-1806">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1806">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e5aa7-1807">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1807">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e5aa7-1808">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1808">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1809">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1809">SQL</span></span>

* <span data-ttu-id="e5aa7-1810">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1810">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e5aa7-1811">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1811">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e5aa7-1812">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1812">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1813">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1813">Storage</span></span>

* <span data-ttu-id="e5aa7-1814">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1814">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e5aa7-1815">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1815">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e5aa7-1816">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1816">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e5aa7-1817">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1817">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e5aa7-1818">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1818">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e5aa7-1819">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1819">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1820">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1820">VM</span></span>

* <span data-ttu-id="e5aa7-1821">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1821">Support configuring nsg</span></span>
* <span data-ttu-id="e5aa7-1822">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1822">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e5aa7-1823">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1823">Support managed service identities</span></span>
* <span data-ttu-id="e5aa7-1824">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1824">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e5aa7-1825">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1825">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e5aa7-1826">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1826">May 10, 2017</span></span>

<span data-ttu-id="e5aa7-1827">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1827">Version 2.0.6</span></span>

* <span data-ttu-id="e5aa7-1828">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1828">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e5aa7-1829">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1829">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e5aa7-1830">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1830">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e5aa7-1831">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1831">Include Cognitive Services module</span></span>
* <span data-ttu-id="e5aa7-1832">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1832">Include Service Fabric module</span></span>
* <span data-ttu-id="e5aa7-1833">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1833">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e5aa7-1834">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1834">Add support for CDN commands</span></span>
* <span data-ttu-id="e5aa7-1835">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1835">Remove Container module</span></span>
* <span data-ttu-id="e5aa7-1836">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1836">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e5aa7-1837">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1837">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e5aa7-1838">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1838">Core</span></span>

* <span data-ttu-id="e5aa7-1839">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1839">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e5aa7-1840">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1840">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e5aa7-1841">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1841">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e5aa7-1842">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1842">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e5aa7-1843">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1843">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e5aa7-1844">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1844">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e5aa7-1845">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1845">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e5aa7-1846">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1846">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e5aa7-1847">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1847">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e5aa7-1848">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1848">core: Improved performance</span></span>
* <span data-ttu-id="e5aa7-1849">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1849">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e5aa7-1850">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1850">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1851">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1851">ACS</span></span>

* <span data-ttu-id="e5aa7-1852">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1852">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e5aa7-1853">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1853">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e5aa7-1854">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1854">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e5aa7-1855">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1855">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1856">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1856">AppService</span></span>

* <span data-ttu-id="e5aa7-1857">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1857">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e5aa7-1858">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1858">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e5aa7-1859">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1859">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e5aa7-1860">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1860">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e5aa7-1861">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1861">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e5aa7-1862">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1862">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e5aa7-1863">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1863">support slot swap with preview</span></span>
* <span data-ttu-id="e5aa7-1864">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1864">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e5aa7-1865">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1865">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5aa7-1866">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1866">CosmosDB</span></span>

* <span data-ttu-id="e5aa7-1867">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1867">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e5aa7-1868">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1868">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e5aa7-1869">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1869">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e5aa7-1870">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1870">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5aa7-1871">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1871">Data Lake Analytics</span></span>

* <span data-ttu-id="e5aa7-1872">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1872">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e5aa7-1873">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1873">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e5aa7-1874">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1874">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e5aa7-1875">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1875">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e5aa7-1876">Table</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1876">Table</span></span>
  * <span data-ttu-id="e5aa7-1877">Fonction table</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1877">Table valued function</span></span>
  * <span data-ttu-id="e5aa7-1878">Affichage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1878">View</span></span>
  * <span data-ttu-id="e5aa7-1879">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1879">Table Statistics.</span></span> <span data-ttu-id="e5aa7-1880">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1880">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5aa7-1881">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1881">Data Lake Store</span></span>

* <span data-ttu-id="e5aa7-1882">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1882">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e5aa7-1883">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1883">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e5aa7-1884">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1884">missed help for access show.</span></span> <span data-ttu-id="e5aa7-1885">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1885">adding it.</span></span> <span data-ttu-id="e5aa7-1886">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1886">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e5aa7-1887">Rechercher</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1887">Find</span></span>

* <span data-ttu-id="e5aa7-1888">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1888">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5aa7-1889">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1889">KeyVault</span></span>

* <span data-ttu-id="e5aa7-1890">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1890">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e5aa7-1891">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1891">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e5aa7-1892">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1892">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e5aa7-1893">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1893">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e5aa7-1894">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1894">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e5aa7-1895">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1895">Lab</span></span>

* <span data-ttu-id="e5aa7-1896">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1896">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e5aa7-1897">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1897">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e5aa7-1898">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1898">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e5aa7-1899">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1899">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e5aa7-1900">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1900">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e5aa7-1901">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1901">Monitor</span></span>

* <span data-ttu-id="e5aa7-1902">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1902">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e5aa7-1903">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1903">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e5aa7-1904">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1904">Network</span></span>

* <span data-ttu-id="e5aa7-1905">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1905">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e5aa7-1906">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1906">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e5aa7-1907">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1907">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e5aa7-1908">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1908">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e5aa7-1909">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1909">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e5aa7-1910">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1910">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e5aa7-1911">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1911">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e5aa7-1912">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1912">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e5aa7-1913">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1913">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e5aa7-1914">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1914">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e5aa7-1915">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1915">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e5aa7-1916">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1916">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e5aa7-1917">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1917">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e5aa7-1918">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1918">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e5aa7-1919">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1919">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e5aa7-1920">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1920">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e5aa7-1921">Profil</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1921">Profile</span></span>

* <span data-ttu-id="e5aa7-1922">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1922">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e5aa7-1923">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1923">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e5aa7-1924">Redis</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1924">Redis</span></span>

* <span data-ttu-id="e5aa7-1925">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1925">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e5aa7-1926">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1926">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e5aa7-1927">Ressource</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1927">Resource</span></span>

* <span data-ttu-id="e5aa7-1928">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1928">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e5aa7-1929">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1929">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e5aa7-1930">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1930">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e5aa7-1931">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1931">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e5aa7-1932">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1932">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e5aa7-1933">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1933">Add docs for az lock update.</span></span> <span data-ttu-id="e5aa7-1934">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1934">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e5aa7-1935">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1935">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e5aa7-1936">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1936">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e5aa7-1937">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1937">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e5aa7-1938">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1938">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e5aa7-1939">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1939">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e5aa7-1940">Rôle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1940">Role</span></span>

* <span data-ttu-id="e5aa7-1941">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1941">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e5aa7-1942">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1942">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e5aa7-1943">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1943">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e5aa7-1944">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1944">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e5aa7-1945">SQL</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1945">SQL</span></span>

* <span data-ttu-id="e5aa7-1946">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1946">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e5aa7-1947">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1947">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e5aa7-1948">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1948">Storage</span></span>

* <span data-ttu-id="e5aa7-1949">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1949">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e5aa7-1950">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1950">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e5aa7-1951">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1951">Add support for large block blob upload</span></span>
* <span data-ttu-id="e5aa7-1952">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1952">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1953">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1953">VM</span></span>

* <span data-ttu-id="e5aa7-1954">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1954">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e5aa7-1955">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1955">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e5aa7-1956">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1956">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e5aa7-1957">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1957">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e5aa7-1958">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1958">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e5aa7-1959">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1959">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e5aa7-1960">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1960">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e5aa7-1961">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1961">April 3, 2017</span></span>

<span data-ttu-id="e5aa7-1962">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1962">Version 2.0.2</span></span>

<span data-ttu-id="e5aa7-1963">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1963">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e5aa7-1964">Principal</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1964">Core</span></span>

* <span data-ttu-id="e5aa7-1965">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1965">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e5aa7-1966">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1966">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e5aa7-1967">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1967">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e5aa7-1968">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1968">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e5aa7-1969">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1969">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e5aa7-1970">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1970">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e5aa7-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e5aa7-1972">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1972">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e5aa7-1973">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1973">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e5aa7-1974">ACS</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1974">ACS</span></span>

* <span data-ttu-id="e5aa7-1975">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1975">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e5aa7-1976">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1976">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e5aa7-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e5aa7-1978">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1978">Add support for windows clusters.</span></span> <span data-ttu-id="e5aa7-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e5aa7-1980">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1980">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e5aa7-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e5aa7-1982">AppService</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1982">AppService</span></span>

* <span data-ttu-id="e5aa7-1983">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1983">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e5aa7-1984">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1984">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e5aa7-1985">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1985">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e5aa7-1986">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1986">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e5aa7-1987">DataLake</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1987">DataLake</span></span>

* <span data-ttu-id="e5aa7-1988">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1988">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e5aa7-1989">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1989">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e5aa7-1990">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1990">DocuemntDB</span></span>

* <span data-ttu-id="e5aa7-1991">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1991">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e5aa7-1992">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1992">VM</span></span>

* <span data-ttu-id="e5aa7-1993">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1993">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e5aa7-1994">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1994">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e5aa7-1995">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1995">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e5aa7-1996">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1996">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e5aa7-1997">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1997">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e5aa7-1998">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1998">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="e5aa7-1999">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e5aa7-1999">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e5aa7-2000">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2000">February 27, 2017</span></span>

<span data-ttu-id="e5aa7-2001">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2001">Version 2.0.0</span></span>

<span data-ttu-id="e5aa7-2002">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2002">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e5aa7-2003">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2003">Container Service (acs)</span></span>
- <span data-ttu-id="e5aa7-2004">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2004">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e5aa7-2005">Réseau</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2005">Networking</span></span>
- <span data-ttu-id="e5aa7-2006">Stockage</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2006">Storage</span></span>

<span data-ttu-id="e5aa7-2007">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2007">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e5aa7-2008">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2008">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e5aa7-2009">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2009">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e5aa7-2010">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2010">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e5aa7-2011">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2011">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e5aa7-2012">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2012">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e5aa7-2013">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2013">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e5aa7-2014">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2014">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e5aa7-2015">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e5aa7-2015">Provide feedback from the command line with the `az feedback` command</span></span>

