---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/30/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 673014c3fd86e20148fe5ffa9fa5160e490da0cb
ms.sourcegitcommit: d29d86d33916d5551b4aeb984b06d7a85c4f6b06
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2019
ms.locfileid: "68658936"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="c209a-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c209a-103">Azure CLI release notes</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="c209a-104">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-104">July 30, 2019</span></span>

<span data-ttu-id="c209a-105">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="c209a-105">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-106">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-106">ACR</span></span>

* <span data-ttu-id="c209a-107">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="c209a-107">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="c209a-108">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="c209a-108">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-109">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-109">Appservice</span></span>

* <span data-ttu-id="c209a-110">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="c209a-110">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="c209a-111">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="c209a-111">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="c209a-112">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="c209a-112">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="c209a-113">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-113">Network</span></span>

* <span data-ttu-id="c209a-114">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="c209a-114">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="c209a-115">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="c209a-115">Fixes #9604.</span></span> <span data-ttu-id="c209a-116">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c209a-116">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="c209a-117">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="c209a-117">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="c209a-118">RBAC</span><span class="sxs-lookup"><span data-stu-id="c209a-118">RBAC</span></span>

* <span data-ttu-id="c209a-119">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="c209a-119">Added `user update` command</span></span>
* <span data-ttu-id="c209a-120">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c209a-120">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="c209a-121">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="c209a-121">Use replacement argument `--id`</span></span>
* <span data-ttu-id="c209a-122">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c209a-122">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-123">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-123">SQL</span></span>

* <span data-ttu-id="c209a-124">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="c209a-124">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-125">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-125">Storage</span></span>

* <span data-ttu-id="c209a-126">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="c209a-126">Added `storage remove` command</span></span>
* <span data-ttu-id="c209a-127">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="c209a-127">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-128">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-128">VM</span></span>

* <span data-ttu-id="c209a-129">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="c209a-129">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="c209a-130">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c209a-130">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="c209a-131">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-131">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="c209a-132">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="c209a-132">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="c209a-133">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-133">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="c209a-134">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-134">July 16, 2019</span></span>

<span data-ttu-id="c209a-135">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="c209a-135">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-136">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-136">Appservice</span></span>

* <span data-ttu-id="c209a-137">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="c209a-137">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="c209a-138">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="c209a-138">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="c209a-139">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="c209a-139">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="c209a-140">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-140">Core</span></span>

* <span data-ttu-id="c209a-141">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="c209a-141">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-142">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-142">Batch</span></span>

* <span data-ttu-id="c209a-143">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="c209a-143">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="c209a-144">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="c209a-144">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="c209a-145">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="c209a-145">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="c209a-146">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-146">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c209a-147">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c209a-147">Eventhubs</span></span>

* <span data-ttu-id="c209a-148">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="c209a-148">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-149">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-149">RDBMS</span></span>

* <span data-ttu-id="c209a-150">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="c209a-150">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="c209a-151">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="c209a-151">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="c209a-152">Relais</span><span class="sxs-lookup"><span data-stu-id="c209a-152">Relay</span></span>

* <span data-ttu-id="c209a-153">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="c209a-153">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="c209a-154">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="c209a-154">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="c209a-155">Servicebus</span><span class="sxs-lookup"><span data-stu-id="c209a-155">Servicebus</span></span>

* <span data-ttu-id="c209a-156">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="c209a-156">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-157">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-157">Storage</span></span>

* <span data-ttu-id="c209a-158">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-158">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="c209a-159">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="c209a-159">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="c209a-160">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-160">July 2, 2019</span></span>

<span data-ttu-id="c209a-161">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="c209a-161">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="c209a-162">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-162">Core</span></span>

* <span data-ttu-id="c209a-163">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="c209a-163">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="c209a-164">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="c209a-164">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="c209a-165">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="c209a-165">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-166">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-166">ACR</span></span>

* <span data-ttu-id="c209a-167">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="c209a-167">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-168">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-168">Appservice</span></span>

* <span data-ttu-id="c209a-169">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-169">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="c209a-170">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="c209a-170">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="c209a-171">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="c209a-171">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="c209a-172">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="c209a-172">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c209a-173">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c209a-173">Cosmos DB</span></span>

* <span data-ttu-id="c209a-174">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="c209a-174">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="c209a-175">DLS</span><span class="sxs-lookup"><span data-stu-id="c209a-175">DLS</span></span>

* <span data-ttu-id="c209a-176">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="c209a-176">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="c209a-177">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c209a-177">Feedback</span></span>

* <span data-ttu-id="c209a-178">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="c209a-178">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-179">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-179">HDInsight</span></span>

* <span data-ttu-id="c209a-180">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="c209a-180">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="c209a-181">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="c209a-181">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="c209a-182">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="c209a-182">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="c209a-183">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="c209a-183">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="c209a-184">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="c209a-184">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="c209a-185">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-185">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="c209a-186">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="c209a-186">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="c209a-187">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="c209a-187">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="c209a-188">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="c209a-188">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="c209a-189">Services gérés</span><span class="sxs-lookup"><span data-stu-id="c209a-189">Managed Services</span></span>

* <span data-ttu-id="c209a-190">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-190">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-191">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-191">Profile</span></span>
* <span data-ttu-id="c209a-192">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="c209a-192">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="c209a-193">RBAC</span><span class="sxs-lookup"><span data-stu-id="c209a-193">RBAC</span></span>

* <span data-ttu-id="c209a-194">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c209a-194">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="c209a-195">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="c209a-195">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="c209a-196">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="c209a-196">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="c209a-197">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="c209a-197">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-198">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-198">RDBMS</span></span>

* <span data-ttu-id="c209a-199">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="c209a-199">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-200">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-200">SQL</span></span>

* <span data-ttu-id="c209a-201">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-201">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-202">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-202">Storage</span></span>

* <span data-ttu-id="c209a-203">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c209a-203">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="c209a-204">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c209a-204">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="c209a-205">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-205">VM</span></span>

* <span data-ttu-id="c209a-206">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-206">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="c209a-207">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="c209a-207">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="c209a-208">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="c209a-208">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="c209a-209">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="c209a-209">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="c209a-210">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-210">June 18, 2019</span></span>

<span data-ttu-id="c209a-211">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="c209a-211">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="c209a-212">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-212">Core</span></span>

<span data-ttu-id="c209a-213">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="c209a-213">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="c209a-214">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="c209a-214">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="c209a-215">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="c209a-215">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="c209a-216">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="c209a-216">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="c209a-217">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="c209a-217">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="c209a-218">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="c209a-218">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="c209a-219">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="c209a-219">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-220">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-220">ACR</span></span>
* <span data-ttu-id="c209a-221">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="c209a-221">Added 'acr check-health' command</span></span>
* <span data-ttu-id="c209a-222">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="c209a-222">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-223">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-223">ACS</span></span>
* <span data-ttu-id="c209a-224">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="c209a-224">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-225">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-225">AMS</span></span>
* <span data-ttu-id="c209a-226">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="c209a-226">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-227">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-227">AppService</span></span>
* <span data-ttu-id="c209a-228">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="c209a-228">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="c209a-229">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c209a-229">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="c209a-230">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="c209a-230">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="c209a-231">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-231">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="c209a-232">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="c209a-232">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="c209a-233">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="c209a-233">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-234">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-234">Batch</span></span>
* <span data-ttu-id="c209a-235">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="c209a-235">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-236">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-236">BatchAI</span></span>
* <span data-ttu-id="c209a-237">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="c209a-237">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-238">BotService</span><span class="sxs-lookup"><span data-stu-id="c209a-238">BotService</span></span>
* <span data-ttu-id="c209a-239">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="c209a-239">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-240">CosmosDB</span></span>
* <span data-ttu-id="c209a-241">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="c209a-241">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="c209a-242">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="c209a-242">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="c209a-243">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="c209a-243">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="c209a-244">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="c209a-244">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c209a-245">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c209a-245">EventGrid</span></span>
* <span data-ttu-id="c209a-246">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="c209a-246">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="c209a-247">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="c209a-247">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="c209a-248">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="c209a-248">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="c209a-249">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="c209a-249">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="c209a-250">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-250">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-251">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-251">HDInsight</span></span>
* <span data-ttu-id="c209a-252">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c209a-252">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-253">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-253">IoT</span></span>
* <span data-ttu-id="c209a-254">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="c209a-254">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="c209a-255">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="c209a-255">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="c209a-256">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-256">Network</span></span>
* <span data-ttu-id="c209a-257">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="c209a-257">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="c209a-258">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="c209a-258">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="c209a-259">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="c209a-259">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="c209a-260">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="c209a-260">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-261">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-261">Resource</span></span>
* <span data-ttu-id="c209a-262">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="c209a-262">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="c209a-263">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="c209a-263">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="c209a-264">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c209a-264">ServiceBus</span></span>
* <span data-ttu-id="c209a-265">Correction d’une erreur liée à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="c209a-265">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-266">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-266">SQL</span></span>
* <span data-ttu-id="c209a-267">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c209a-267">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="c209a-268">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="c209a-268">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="c209a-269">SQLVm</span><span class="sxs-lookup"><span data-stu-id="c209a-269">SQLVm</span></span>
* <span data-ttu-id="c209a-270">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="c209a-270">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="c209a-271">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-271">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-272">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-272">Storage</span></span>
* <span data-ttu-id="c209a-273">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c209a-273">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="c209a-274">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-274">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-275">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-275">VM</span></span>
* <span data-ttu-id="c209a-276">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-276">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="c209a-277">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-277">June 4, 2019</span></span>

<span data-ttu-id="c209a-278">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="c209a-278">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="c209a-279">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-279">Core</span></span>
* <span data-ttu-id="c209a-280">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="c209a-280">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-281">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-281">ACR</span></span>
* <span data-ttu-id="c209a-282">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="c209a-282">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-283">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-283">ACS</span></span>
* <span data-ttu-id="c209a-284">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-284">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="c209a-285">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="c209a-285">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-286">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-286">Batch</span></span>
* <span data-ttu-id="c209a-287">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="c209a-287">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-288">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-288">IoT</span></span>
* <span data-ttu-id="c209a-289">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c209a-289">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="c209a-290">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-290">Network</span></span>
* <span data-ttu-id="c209a-291">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="c209a-291">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="c209a-292">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-292">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="c209a-293">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-293">Resource</span></span>
* <span data-ttu-id="c209a-294">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="c209a-294">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="c209a-295">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-295">Role</span></span>
* <span data-ttu-id="c209a-296">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="c209a-296">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="c209a-297">Calcul</span><span class="sxs-lookup"><span data-stu-id="c209a-297">Compute</span></span>
* <span data-ttu-id="c209a-298">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="c209a-298">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="c209a-299">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-299">May 21, 2019</span></span>

<span data-ttu-id="c209a-300">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="c209a-300">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="c209a-301">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-301">Core</span></span>
* <span data-ttu-id="c209a-302">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="c209a-302">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="c209a-303">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="c209a-303">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="c209a-304">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="c209a-304">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-305">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-305">ACR</span></span>
* <span data-ttu-id="c209a-306">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="c209a-306">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-307">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-307">ACS</span></span>
* <span data-ttu-id="c209a-308">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="c209a-308">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-309">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-309">AppService</span></span>
* <span data-ttu-id="c209a-310">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="c209a-310">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="c209a-311">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="c209a-311">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="c209a-312">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="c209a-312">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="c209a-313">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="c209a-313">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="c209a-314">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c209a-314">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="c209a-315">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="c209a-315">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="c209a-316">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c209a-316">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-317">BotService</span><span class="sxs-lookup"><span data-stu-id="c209a-317">BotService</span></span>
* <span data-ttu-id="c209a-318">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-318">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="c209a-319">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-319">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-320">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-320">Consumption</span></span>
* <span data-ttu-id="c209a-321">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-321">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-322">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-322">IoT</span></span>
* <span data-ttu-id="c209a-323">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="c209a-323">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="c209a-324">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-324">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="c209a-326">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="c209a-326">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="c209a-327">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="c209a-327">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-328">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-328">RDBMS</span></span>
* <span data-ttu-id="c209a-329">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="c209a-329">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="c209a-330">RBAC</span><span class="sxs-lookup"><span data-stu-id="c209a-330">RBAC</span></span>
* <span data-ttu-id="c209a-331">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="c209a-331">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-332">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-332">Storage</span></span>
* <span data-ttu-id="c209a-333">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-333">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="c209a-334">Calcul</span><span class="sxs-lookup"><span data-stu-id="c209a-334">Compute</span></span>
* <span data-ttu-id="c209a-335">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-335">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="c209a-336">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="c209a-336">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="c209a-337">__Remarque__: il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="c209a-337">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="c209a-338">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="c209a-338">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="c209a-339">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-339">May 6, 2019</span></span>

<span data-ttu-id="c209a-340">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="c209a-340">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-341">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-341">ACS</span></span>
* <span data-ttu-id="c209a-342">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="c209a-342">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="c209a-343">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="c209a-343">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="c209a-344">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="c209a-344">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="c209a-345">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="c209a-345">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-346">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-346">Appservice</span></span>
* <span data-ttu-id="c209a-347">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="c209a-347">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="c209a-348">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="c209a-348">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="c209a-349">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c209a-349">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="c209a-350">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="c209a-350">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="c209a-351">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c209a-351">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="c209a-352">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="c209a-352">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="c209a-353">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="c209a-353">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="c209a-354">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="c209a-354">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="c209a-355">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-355">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="c209a-356">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="c209a-356">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-357">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-357">Batch</span></span>
* <span data-ttu-id="c209a-358">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="c209a-358">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-359">Botservice</span><span class="sxs-lookup"><span data-stu-id="c209a-359">Botservice</span></span>
* <span data-ttu-id="c209a-360">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="c209a-360">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="c209a-361">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="c209a-361">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="c209a-362">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="c209a-362">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="c209a-363">__REMARQUE :__  `bot prepare-publish` utilise toujours l’ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-363">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="c209a-364">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="c209a-364">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="c209a-365">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-365">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="c209a-366">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="c209a-366">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="c209a-367">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="c209a-367">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="c209a-368">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="c209a-368">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="c209a-369">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="c209a-369">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="c209a-370">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="c209a-370">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="c209a-371">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="c209a-371">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="c209a-372">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="c209a-372">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="c209a-373">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="c209a-373">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="c209a-374">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-374">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="c209a-375">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="c209a-375">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="c209a-376">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="c209a-376">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="c209a-377">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="c209a-377">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="c209a-378">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c209a-378">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="c209a-379">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="c209a-379">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="c209a-380">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="c209a-380">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="c209a-381">Configuration</span><span class="sxs-lookup"><span data-stu-id="c209a-381">Configure</span></span>
* <span data-ttu-id="c209a-382">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="c209a-382">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c209a-383">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c209a-383">Eventhubs</span></span>
* <span data-ttu-id="c209a-384">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-384">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="c209a-385">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-385">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-386">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-386">Network</span></span>
* <span data-ttu-id="c209a-387">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-387">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="c209a-388">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c209a-388">Policy Insights</span></span>
* <span data-ttu-id="c209a-389">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-389">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="c209a-390">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-390">Role</span></span>
* <span data-ttu-id="c209a-391">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-391">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="c209a-392">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c209a-392">Service Bus</span></span>
* <span data-ttu-id="c209a-393">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-393">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="c209a-394">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-394">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="c209a-395">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="c209a-395">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-396">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-396">SQL</span></span>
* <span data-ttu-id="c209a-397">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="c209a-397">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-398">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-398">VM</span></span>
* <span data-ttu-id="c209a-399">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="c209a-399">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="c209a-400">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="c209a-400">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="c209a-401">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-401">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="c209a-402">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="c209a-402">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="c209a-403">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="c209a-403">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="c209a-404">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="c209a-404">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="c209a-405">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-405">April 23, 2019</span></span>

<span data-ttu-id="c209a-406">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="c209a-406">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-407">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-407">ACS</span></span>
* <span data-ttu-id="c209a-408">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="c209a-408">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="c209a-409">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="c209a-409">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-410">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-410">AMS</span></span>
* <span data-ttu-id="c209a-411">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="c209a-411">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-412">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-412">AppService</span></span>
* <span data-ttu-id="c209a-413">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="c209a-413">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="c209a-414">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="c209a-414">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="c209a-415">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="c209a-415">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="c209a-416">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="c209a-416">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="c209a-417">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="c209a-417">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="c209a-418">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-418">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="c209a-419">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="c209a-419">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="c209a-420">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="c209a-420">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="c209a-421">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="c209a-421">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="c209a-422">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="c209a-422">Deployment Manager</span></span>
* <span data-ttu-id="c209a-423">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="c209a-423">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="c209a-424">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-424">Lab</span></span>
* <span data-ttu-id="c209a-425">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="c209a-425">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="c209a-426">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-426">Network</span></span>
* <span data-ttu-id="c209a-427">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="c209a-427">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-428">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-428">Resource</span></span>
* <span data-ttu-id="c209a-429">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="c209a-429">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="c209a-430">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="c209a-430">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="c209a-431">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-431">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="c209a-432">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-432">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-433">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-433">SQL</span></span>
* <span data-ttu-id="c209a-434">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="c209a-434">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="c209a-435">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="c209a-435">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="c209a-436">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-436">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="c209a-437">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-437">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-438">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-438">Storage</span></span>
* <span data-ttu-id="c209a-439">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c209a-439">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-440">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-440">VM</span></span>
* <span data-ttu-id="c209a-441">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="c209a-441">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="c209a-442">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="c209a-442">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="c209a-443">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="c209a-443">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="c209a-444">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-444">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="c209a-445">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-445">Core</span></span>
* <span data-ttu-id="c209a-446">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="c209a-446">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-447">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-447">ACR</span></span>
* <span data-ttu-id="c209a-448">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="c209a-448">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-449">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-449">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="c209a-452">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c209a-452">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="c209a-453">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="c209a-453">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-454">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-454">AppService</span></span>
* <span data-ttu-id="c209a-455">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c209a-455">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="c209a-456">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="c209a-456">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="c209a-457">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="c209a-457">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="c209a-458">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="c209a-458">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="c209a-459">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-459">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="c209a-460">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="c209a-460">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="c209a-461">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="c209a-461">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-462">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-462">CDN</span></span>
* <span data-ttu-id="c209a-463">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="c209a-463">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="c209a-464">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c209a-464">Feedback</span></span>
* <span data-ttu-id="c209a-465">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="c209a-465">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="c209a-466">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="c209a-466">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="c209a-467">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="c209a-467">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-468">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-468">Monitor</span></span>
* <span data-ttu-id="c209a-469">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-469">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="c209a-470">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-470">Network</span></span>
* <span data-ttu-id="c209a-471">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="c209a-471">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="c209a-472">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-472">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="c209a-473">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="c209a-473">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="c209a-474">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="c209a-474">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="c209a-475">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="c209a-475">PrivateDNS</span></span>
* <span data-ttu-id="c209a-476">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c209a-476">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-477">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-477">Resource</span></span>
* <span data-ttu-id="c209a-478">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c209a-478">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="c209a-479">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-479">Role</span></span>
* <span data-ttu-id="c209a-480">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-480">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="c209a-481">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-481">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-482">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-482">SQL</span></span>
* <span data-ttu-id="c209a-483">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="c209a-483">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-484">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-484">Storage</span></span>
* <span data-ttu-id="c209a-485">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-485">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="c209a-486">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="c209a-486">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="c209a-487">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="c209a-487">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="c209a-488">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="c209a-488">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="c209a-489">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-489">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="c209a-490">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-490">Core</span></span>
* <span data-ttu-id="c209a-491">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="c209a-491">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="c209a-492">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="c209a-492">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="c209a-493">Cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-493">Cloud</span></span>
* <span data-ttu-id="c209a-494">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="c209a-494">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-495">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-495">ACR</span></span>
* <span data-ttu-id="c209a-496">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c209a-496">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="c209a-497">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c209a-497">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="c209a-498">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="c209a-498">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="c209a-499">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="c209a-499">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-500">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-500">AppService</span></span>
* <span data-ttu-id="c209a-501">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="c209a-501">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="c209a-502">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="c209a-502">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="c209a-503">Service BOT</span><span class="sxs-lookup"><span data-stu-id="c209a-503">BOT Service</span></span>
* <span data-ttu-id="c209a-504">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="c209a-504">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="c209a-505">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="c209a-505">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="c209a-506">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="c209a-506">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="c209a-507">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c209a-507">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-508">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-508">CDN</span></span>
* <span data-ttu-id="c209a-509">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="c209a-509">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="c209a-510">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="c209a-510">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="c209a-511">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="c209a-511">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c209a-512">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c209a-512">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-513">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c209a-513">Cosmosdb</span></span>
* <span data-ttu-id="c209a-514">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="c209a-514">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="c209a-515">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c209a-515">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-516">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-516">Interactive</span></span>
* <span data-ttu-id="c209a-517">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="c209a-517">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-518">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-518">Monitor</span></span>
* <span data-ttu-id="c209a-519">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-519">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-520">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-520">Network</span></span>
* <span data-ttu-id="c209a-521">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="c209a-521">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-522">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-522">Profile</span></span>
* <span data-ttu-id="c209a-523">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="c209a-523">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="c209a-524">Postgres</span><span class="sxs-lookup"><span data-stu-id="c209a-524">Postgres</span></span> 
* <span data-ttu-id="c209a-525">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="c209a-525">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="c209a-526">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="c209a-526">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-527">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-527">Resource</span></span>
* <span data-ttu-id="c209a-528">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-528">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="c209a-529">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="c209a-529">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="c209a-530">Graph</span><span class="sxs-lookup"><span data-stu-id="c209a-530">Graph</span></span>
* <span data-ttu-id="c209a-531">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="c209a-531">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="c209a-532">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="c209a-532">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="c209a-533">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="c209a-533">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="c209a-534">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-534">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="c209a-535">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="c209a-535">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-536">storage</span><span class="sxs-lookup"><span data-stu-id="c209a-536">storage</span></span>
* <span data-ttu-id="c209a-537">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="c209a-537">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="c209a-538">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="c209a-538">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="c209a-539">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c209a-539">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="c209a-540">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="c209a-540">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-541">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-541">VM</span></span>
* <span data-ttu-id="c209a-542">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="c209a-542">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="c209a-543">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-543">March 12, 2019</span></span>

<span data-ttu-id="c209a-544">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="c209a-544">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="c209a-545">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-545">Core</span></span>

* <span data-ttu-id="c209a-546">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="c209a-546">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-547">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-547">ACR</span></span>

* <span data-ttu-id="c209a-548">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c209a-548">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-549">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-549">ACS</span></span>

* <span data-ttu-id="c209a-550">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="c209a-550">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="c209a-551">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-551">AppService</span></span>

* <span data-ttu-id="c209a-552">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="c209a-552">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="c209a-553">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c209a-553">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="c209a-554">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-554">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="c209a-555">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="c209a-555">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-556">Botservice</span><span class="sxs-lookup"><span data-stu-id="c209a-556">Botservice</span></span>

* <span data-ttu-id="c209a-557">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c209a-557">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c209a-558">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c209a-558">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c209a-559">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="c209a-559">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="c209a-560">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="c209a-560">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="c209a-561">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-561">Container</span></span>

* <span data-ttu-id="c209a-562">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="c209a-562">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="c209a-563">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c209a-563">EventHub</span></span>

* <span data-ttu-id="c209a-564">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="c209a-564">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="c209a-565">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c209a-565">Find</span></span>

* <span data-ttu-id="c209a-566">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c209a-566">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-567">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-567">HDInsight</span></span>

* <span data-ttu-id="c209a-568">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="c209a-568">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="c209a-569">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-569">Network</span></span>

* <span data-ttu-id="c209a-570">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="c209a-570">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-571">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c209a-571">Rdbms</span></span>

* <span data-ttu-id="c209a-572">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="c209a-572">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="c209a-573">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-573">Role</span></span>

* <span data-ttu-id="c209a-574">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="c209a-574">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="c209a-575">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="c209a-575">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c209a-576">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c209a-576">Service Fabric</span></span>

* <span data-ttu-id="c209a-577">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="c209a-577">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="c209a-578">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-578">February 26, 2019</span></span>

<span data-ttu-id="c209a-579">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="c209a-579">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="c209a-580">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-580">Core</span></span>

* <span data-ttu-id="c209a-581">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="c209a-581">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-582">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-582">ACR</span></span>

* <span data-ttu-id="c209a-583">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c209a-583">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="c209a-584">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="c209a-584">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-585">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-585">ACS</span></span>

* <span data-ttu-id="c209a-586">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="c209a-586">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-587">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-587">AppService</span></span>

* <span data-ttu-id="c209a-588">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="c209a-588">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-589">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-589">Batch</span></span>
* <span data-ttu-id="c209a-590">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="c209a-590">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="c209a-591">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="c209a-591">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="c209a-592">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="c209a-592">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="c209a-593">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="c209a-593">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="c209a-594">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="c209a-594">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="c209a-595">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="c209a-595">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-596">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-596">CosmosDB</span></span>

* <span data-ttu-id="c209a-597">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c209a-597">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="c209a-598">Kusto</span><span class="sxs-lookup"><span data-stu-id="c209a-598">Kusto</span></span>

* <span data-ttu-id="c209a-599">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="c209a-599">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="c209a-600">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-600">Network</span></span>

* <span data-ttu-id="c209a-601">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-601">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="c209a-602">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="c209a-602">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="c209a-603">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="c209a-603">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="c209a-604">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-604">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="c209a-605">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-605">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="c209a-606">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-606">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="c209a-607">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="c209a-607">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-608">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-608">Resource</span></span>

* <span data-ttu-id="c209a-609">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-609">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="c209a-610">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c209a-610">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="c209a-611">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="c209a-611">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="c209a-612">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c209a-612">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="c209a-613">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-613">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="c209a-614">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-614">Role</span></span>

* <span data-ttu-id="c209a-615">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-615">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-616">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-616">VM</span></span>

* <span data-ttu-id="c209a-617">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="c209a-617">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="c209a-618">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-618">February 12, 2019</span></span>

<span data-ttu-id="c209a-619">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="c209a-619">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="c209a-620">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-620">Core</span></span>

* <span data-ttu-id="c209a-621">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="c209a-621">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="c209a-622">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="c209a-622">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-623">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-623">ACR</span></span>
* <span data-ttu-id="c209a-624">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="c209a-624">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="c209a-625">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-625">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-626">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-626">ACS</span></span>
* <span data-ttu-id="c209a-627">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="c209a-627">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="c209a-628">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="c209a-628">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="c209a-629">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c209a-629">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-630">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-630">AMS</span></span>
* <span data-ttu-id="c209a-631">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-631">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="c209a-632">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-632">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-633">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-633">Appservice</span></span>
* <span data-ttu-id="c209a-634">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-634">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="c209a-635">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="c209a-635">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="c209a-636">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="c209a-636">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="c209a-637">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="c209a-637">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="c209a-638">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="c209a-638">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-639">Botservice</span><span class="sxs-lookup"><span data-stu-id="c209a-639">Botservice</span></span>
* <span data-ttu-id="c209a-640">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="c209a-640">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="c209a-641">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="c209a-641">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="c209a-642">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="c209a-642">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="c209a-643">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="c209a-643">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="c209a-644">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="c209a-644">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="c209a-645">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="c209a-645">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="c209a-646">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="c209a-646">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="c209a-647">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="c209a-647">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="c209a-648">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="c209a-648">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="c209a-649">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="c209a-649">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="c209a-650">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c209a-650">Key Vault</span></span>
* <span data-ttu-id="c209a-651">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="c209a-651">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-652">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-652">Monitor</span></span>
* <span data-ttu-id="c209a-653">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="c209a-653">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-654">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-654">Network</span></span>
* <span data-ttu-id="c209a-655">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="c209a-655">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="c209a-656">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c209a-656">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="c209a-657">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="c209a-657">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="c209a-658">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-658">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c209a-659">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c209a-659">Policy Insights</span></span>
* <span data-ttu-id="c209a-660">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="c209a-660">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-661">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-661">RDBMS</span></span>
* <span data-ttu-id="c209a-662">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-662">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="c209a-663">Redis</span><span class="sxs-lookup"><span data-stu-id="c209a-663">Redis</span></span>
* <span data-ttu-id="c209a-664">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c209a-664">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="c209a-665">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c209a-665">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="c209a-666">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="c209a-666">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="c209a-667">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="c209a-667">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="c209a-668">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="c209a-668">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="c209a-669">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="c209a-669">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="c209a-670">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="c209a-670">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="c209a-671">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-671">Role</span></span>
* <span data-ttu-id="c209a-672">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="c209a-672">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="c209a-673">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-673">SQL VM</span></span>
* <span data-ttu-id="c209a-674">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="c209a-674">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-675">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-675">VM</span></span>
* <span data-ttu-id="c209a-676">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="c209a-676">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="c209a-677">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-677">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="c209a-678">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="c209a-678">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="c209a-679">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="c209a-679">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="c209a-680">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-680">January 31, 2019</span></span>

<span data-ttu-id="c209a-681">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="c209a-681">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="c209a-682">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-682">Core</span></span>

* <span data-ttu-id="c209a-683">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="c209a-683">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="c209a-684">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-684">January 28, 2019</span></span>

<span data-ttu-id="c209a-685">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="c209a-685">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-686">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-686">ACR</span></span>
* <span data-ttu-id="c209a-687">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="c209a-687">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-688">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-688">ACS</span></span>
* <span data-ttu-id="c209a-689">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c209a-689">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c209a-690">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="c209a-690">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="c209a-691">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="c209a-691">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-692">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-692">AMS</span></span>
* <span data-ttu-id="c209a-693">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="c209a-693">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="c209a-694">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="c209a-694">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-695">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-695">Appservice</span></span>
* <span data-ttu-id="c209a-696">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="c209a-696">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="c209a-697">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="c209a-697">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="c209a-698">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="c209a-698">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="c209a-699">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-699">Container</span></span>
* <span data-ttu-id="c209a-700">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="c209a-700">Added `container start` command</span></span>
* <span data-ttu-id="c209a-701">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-701">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c209a-702">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c209a-702">EventGrid</span></span>
* <span data-ttu-id="c209a-703">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-703">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="c209a-704">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="c209a-704">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="c209a-705">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="c209a-705">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="c209a-706">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="c209a-706">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="c209a-707">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="c209a-707">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-708">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-708">HDInsight</span></span>
* <span data-ttu-id="c209a-709">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-709">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="c209a-710">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c209a-710">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="c209a-711">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c209a-711">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="c209a-712">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c209a-712">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="c209a-713">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="c209a-713">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="c209a-714">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="c209a-714">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-715">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-715">IoT</span></span>
* <span data-ttu-id="c209a-716">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="c209a-716">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="c209a-717">Kusto</span><span class="sxs-lookup"><span data-stu-id="c209a-717">Kusto</span></span>
* <span data-ttu-id="c209a-718">Préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-718">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-719">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-719">Monitor</span></span>
* <span data-ttu-id="c209a-720">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-720">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-721">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-721">Profile</span></span>
* <span data-ttu-id="c209a-722">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="c209a-722">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-723">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-723">Network</span></span>
* <span data-ttu-id="c209a-724">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="c209a-724">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="c209a-725">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="c209a-725">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-726">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-726">Resource</span></span>
* <span data-ttu-id="c209a-727">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c209a-727">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="c209a-728">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-728">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="c209a-729">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-729">SQL Virtual Machine</span></span>
* <span data-ttu-id="c209a-730">Préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-730">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-731">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-731">Storage</span></span>
* <span data-ttu-id="c209a-732">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="c209a-732">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="c209a-733">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="c209a-733">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-734">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-734">VM</span></span>
* <span data-ttu-id="c209a-735">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="c209a-735">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="c209a-736">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c209a-736">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="c209a-737">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c209a-737">January 15, 2019</span></span>

<span data-ttu-id="c209a-738">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="c209a-738">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-739">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-739">ACR</span></span>
* <span data-ttu-id="c209a-740">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c209a-740">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="c209a-741">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c209a-741">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="c209a-742">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="c209a-742">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="c209a-743">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-743">ACS</span></span>
* <span data-ttu-id="c209a-744">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="c209a-744">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-745">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-745">Appservice</span></span>
* <span data-ttu-id="c209a-746">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="c209a-746">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="c209a-747">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-747">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="c209a-748">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="c209a-748">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="c209a-749">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="c209a-749">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-750">Botservice</span><span class="sxs-lookup"><span data-stu-id="c209a-750">Botservice</span></span>
* <span data-ttu-id="c209a-751">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="c209a-751">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="c209a-752">Configuration</span><span class="sxs-lookup"><span data-stu-id="c209a-752">Configure</span></span>
* <span data-ttu-id="c209a-753">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="c209a-753">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-754">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-754">CosmosDB</span></span>
* <span data-ttu-id="c209a-755">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="c209a-755">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-756">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-756">HDInsight</span></span>
* <span data-ttu-id="c209a-757">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="c209a-757">Added commands for managing applications</span></span>
* <span data-ttu-id="c209a-758">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="c209a-758">Added commands for managing script actions</span></span>
* <span data-ttu-id="c209a-759">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="c209a-759">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="c209a-760">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="c209a-760">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="c209a-761">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c209a-761">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-762">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-762">Network</span></span>
* <span data-ttu-id="c209a-763">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-763">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="c209a-764">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="c209a-764">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="c209a-765">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-765">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="c209a-766">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-766">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="c209a-767">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-767">Role</span></span>
* <span data-ttu-id="c209a-768">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="c209a-768">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="c209a-769">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="c209a-769">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="c209a-770">Sécurité</span><span class="sxs-lookup"><span data-stu-id="c209a-770">Security</span></span>
* <span data-ttu-id="c209a-771">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-771">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-772">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-772">Storage</span></span>
* <span data-ttu-id="c209a-773">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="c209a-773">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="c209a-774">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="c209a-774">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="c209a-775">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c209a-775">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="c209a-776">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c209a-776">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="c209a-777">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="c209a-777">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-778">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-778">VM</span></span>
* <span data-ttu-id="c209a-779">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="c209a-779">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="c209a-780">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-780">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c209a-781">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="c209a-781">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="c209a-782">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="c209a-782">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="c209a-783">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-783">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="c209a-784">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="c209a-784">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="c209a-785">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-785">December 20, 2018</span></span>

<span data-ttu-id="c209a-786">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="c209a-786">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="c209a-787">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-787">Appservice</span></span>
* <span data-ttu-id="c209a-788">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c209a-788">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="c209a-789">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="c209a-789">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="c209a-790">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-790">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c209a-791">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c209a-791">IoTCentral</span></span>
* <span data-ttu-id="c209a-792">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="c209a-792">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="c209a-793">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-793">Role</span></span>
* <span data-ttu-id="c209a-794">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="c209a-794">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-795">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-795">SQL</span></span>
* <span data-ttu-id="c209a-796">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="c209a-796">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-797">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-797">VM</span></span>
* <span data-ttu-id="c209a-798">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c209a-798">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="c209a-799">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-799">December 18, 2018</span></span>

<span data-ttu-id="c209a-800">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="c209a-800">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="c209a-801">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-801">ACR</span></span>
* <span data-ttu-id="c209a-802">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="c209a-802">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="c209a-803">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="c209a-803">Condensed the table layout for task list</span></span>
* <span data-ttu-id="c209a-804">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="c209a-804">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-805">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-805">ACS</span></span>
* <span data-ttu-id="c209a-806">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c209a-806">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c209a-807">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-807">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="c209a-808">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="c209a-808">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="c209a-809">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="c209a-809">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="c209a-810">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-810">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="c209a-811">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="c209a-811">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-812">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-812">Appservice</span></span>
* <span data-ttu-id="c209a-813">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="c209a-813">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="c209a-814">Botservice</span><span class="sxs-lookup"><span data-stu-id="c209a-814">Botservice</span></span>
* <span data-ttu-id="c209a-815">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="c209a-815">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="c209a-816">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="c209a-816">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="c209a-817">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="c209a-817">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="c209a-818">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="c209a-818">Reduced Kudu network calls</span></span>
* <span data-ttu-id="c209a-819">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="c209a-819">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-820">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-820">Consumption</span></span>
* <span data-ttu-id="c209a-821">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="c209a-821">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-822">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-822">CosmosDB</span></span>
* <span data-ttu-id="c209a-823">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="c209a-823">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="c209a-824">Cartes</span><span class="sxs-lookup"><span data-stu-id="c209a-824">Maps</span></span>
* <span data-ttu-id="c209a-825">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-825">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-826">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-826">Network</span></span>
* <span data-ttu-id="c209a-827">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="c209a-827">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="c209a-828">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c209a-828">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-829">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-829">Resource</span></span>
* <span data-ttu-id="c209a-830">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-830">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="c209a-831">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-831">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-832">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-832">Storage</span></span>
*  <span data-ttu-id="c209a-833">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="c209a-833">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-834">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-834">VM</span></span>
* <span data-ttu-id="c209a-835">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="c209a-835">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="c209a-836">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-836">December 4, 2018</span></span>

<span data-ttu-id="c209a-837">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="c209a-837">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="c209a-838">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-838">Core</span></span>
* <span data-ttu-id="c209a-839">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="c209a-839">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="c209a-840">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c209a-840">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-841">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-841">Appservice</span></span>
* <span data-ttu-id="c209a-842">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="c209a-842">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="c209a-843">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c209a-843">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="c209a-844">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-844">Network</span></span>
* <span data-ttu-id="c209a-845">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="c209a-845">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="c209a-846">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-846">Role</span></span>
* <span data-ttu-id="c209a-847">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="c209a-847">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="c209a-848">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-848">VM</span></span>
* <span data-ttu-id="c209a-849">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="c209a-849">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="c209a-850">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="c209a-850">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="c209a-851">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="c209a-851">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="c209a-852">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="c209a-852">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="c209a-853">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-853">November 20, 2018</span></span>

<span data-ttu-id="c209a-854">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="c209a-854">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="c209a-855">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-855">Core</span></span>
* <span data-ttu-id="c209a-856">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="c209a-856">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-857">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-857">ACR</span></span>
* <span data-ttu-id="c209a-858">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="c209a-858">Added context token to task step</span></span>
* <span data-ttu-id="c209a-859">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="c209a-859">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="c209a-860">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c209a-860">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-861">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-861">Appservice</span></span>
* <span data-ttu-id="c209a-862">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="c209a-862">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="c209a-863">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="c209a-863">Updated the default `node_version`.</span></span> <span data-ttu-id="c209a-864">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="c209a-864">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="c209a-865">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-865">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="c209a-866">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="c209a-866">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c209a-867">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c209a-867">IotCentral</span></span>
* <span data-ttu-id="c209a-868">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="c209a-868">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-869">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-869">KeyVault</span></span>
* <span data-ttu-id="c209a-870">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="c209a-870">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="c209a-871">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-871">Network</span></span>
* <span data-ttu-id="c209a-872">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="c209a-872">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="c209a-873">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="c209a-873">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="c209a-874">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c209a-874">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="c209a-875">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="c209a-875">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-876">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c209a-876">Rdbms</span></span>
* <span data-ttu-id="c209a-877">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="c209a-877">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="c209a-878">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="c209a-878">Rbac</span></span>
* <span data-ttu-id="c209a-879">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c209a-879">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="c209a-880">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="c209a-880">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="c209a-881">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-881">Storage</span></span>
* <span data-ttu-id="c209a-882">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-882">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="c209a-883">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="c209a-883">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="c209a-884">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="c209a-884">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="c209a-885">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="c209a-885">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-886">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-886">VM</span></span>
* <span data-ttu-id="c209a-887">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="c209a-887">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="c209a-888">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="c209a-888">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="c209a-889">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="c209a-889">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="c209a-890">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="c209a-890">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="c209a-891">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="c209a-891">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="c209a-892">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-892">Added `snapshot wait` command</span></span>
* <span data-ttu-id="c209a-893">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-893">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="c209a-894">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-894">November 6, 2018</span></span>

<span data-ttu-id="c209a-895">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="c209a-895">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="c209a-896">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-896">Core</span></span>
* <span data-ttu-id="c209a-897">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="c209a-897">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-898">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-898">ACR</span></span>
* <span data-ttu-id="c209a-899">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="c209a-899">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="c209a-900">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="c209a-900">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-901">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-901">ACS</span></span>
* <span data-ttu-id="c209a-902">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-902">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="c209a-903">Advisor</span><span class="sxs-lookup"><span data-stu-id="c209a-903">Advisor</span></span>
* <span data-ttu-id="c209a-904">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c209a-904">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-905">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-905">AMS</span></span>
* <span data-ttu-id="c209a-906">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="c209a-906">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="c209a-907">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="c209a-907">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="c209a-908">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c209a-908">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="c209a-909">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="c209a-909">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="c209a-910">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="c209a-910">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="c209a-911">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="c209a-911">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="c209a-912">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="c209a-912">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="c209a-913">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="c209a-913">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="c209a-914">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c209a-914">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="c209a-915">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c209a-915">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="c209a-916">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="c209a-916">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="c209a-917">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="c209a-917">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="c209a-918">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="c209a-918">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="c209a-919">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="c209a-919">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="c209a-920">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="c209a-920">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="c209a-921">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="c209a-921">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="c209a-922">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="c209a-922">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-923">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-923">AppService</span></span>
* <span data-ttu-id="c209a-924">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="c209a-924">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="c209a-925">Configuration</span><span class="sxs-lookup"><span data-stu-id="c209a-925">Configure</span></span>
* <span data-ttu-id="c209a-926">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="c209a-926">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="c209a-927">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-927">Container</span></span>
* <span data-ttu-id="c209a-928">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="c209a-928">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="c209a-929">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c209a-929">EventHub</span></span>
* <span data-ttu-id="c209a-930">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-930">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-931">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-931">Interactive</span></span>
* <span data-ttu-id="c209a-932">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="c209a-932">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-933">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-933">Monitor</span></span>
* <span data-ttu-id="c209a-934">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-934">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-935">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-935">Network</span></span>
* <span data-ttu-id="c209a-936">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="c209a-936">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="c209a-937">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="c209a-937">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="c209a-938">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c209a-938">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="c209a-939">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-939">Profile</span></span>
* <span data-ttu-id="c209a-940">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="c209a-940">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-941">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-941">RDBMS</span></span>
* <span data-ttu-id="c209a-942">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="c209a-942">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-943">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-943">Resource</span></span>
* <span data-ttu-id="c209a-944">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="c209a-944">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="c209a-945">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-945">Role</span></span>
* <span data-ttu-id="c209a-946">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="c209a-946">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="c209a-947">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="c209a-947">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="c209a-948">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="c209a-948">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-949">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-949">Storage</span></span>
* <span data-ttu-id="c209a-950">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="c209a-950">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-951">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-951">VM</span></span>
* <span data-ttu-id="c209a-952">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="c209a-952">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="c209a-953">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="c209a-953">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="c209a-954">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="c209a-954">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="c209a-955">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="c209a-955">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="c209a-956">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="c209a-956">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="c209a-957">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="c209a-957">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="c209a-958">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-958">October 23, 2018</span></span>

<span data-ttu-id="c209a-959">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="c209a-959">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="c209a-960">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-960">Core</span></span>
* <span data-ttu-id="c209a-961">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="c209a-961">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="c209a-962">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="c209a-962">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-963">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-963">ACR</span></span>
* <span data-ttu-id="c209a-964">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="c209a-964">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-965">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-965">CDN</span></span>
* <span data-ttu-id="c209a-966">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="c209a-966">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c209a-967">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c209a-967">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="c209a-968">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-968">Container</span></span>
* <span data-ttu-id="c209a-969">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="c209a-969">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="c209a-970">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-970">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="c209a-971">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="c209a-971">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="c209a-972">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-972">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="c209a-973">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c209a-973">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="c209a-974">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="c209a-974">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="c209a-975">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="c209a-975">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-976">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-976">CosmosDB</span></span>
* <span data-ttu-id="c209a-977">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="c209a-977">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-978">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-978">Interactive</span></span>
* <span data-ttu-id="c209a-979">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="c209a-979">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="c209a-980">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c209a-980">IoT Central</span></span>
* <span data-ttu-id="c209a-981">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="c209a-981">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="c209a-982">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="c209a-982">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-983">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-983">Monitor</span></span>
* <span data-ttu-id="c209a-984">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="c209a-984">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="c209a-985">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-985">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="c209a-986">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c209a-986">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c209a-987">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c209a-987">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="c209a-988">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="c209a-988">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="c209a-989">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c209a-989">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="c209a-990">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="c209a-990">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="c209a-991">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c209a-991">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c209a-992">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c209a-992">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="c209a-993">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c209a-993">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-994">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-994">Network</span></span>
* <span data-ttu-id="c209a-995">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-995">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="c209a-996">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-996">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="c209a-997">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c209a-997">ServiceBus</span></span>
* <span data-ttu-id="c209a-998">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="c209a-998">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-999">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-999">SQL</span></span>
* <span data-ttu-id="c209a-1000">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c209a-1000">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1001">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1001">Storage</span></span>
* <span data-ttu-id="c209a-1002">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="c209a-1002">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="c209a-1003">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="c209a-1003">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1004">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1004">VM</span></span>
* <span data-ttu-id="c209a-1005">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1005">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="c209a-1006">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1006">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="c209a-1007">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1007">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="c209a-1008">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1008">October 16, 2018</span></span>

<span data-ttu-id="c209a-1009">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="c209a-1009">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1010">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1010">VM</span></span>
* <span data-ttu-id="c209a-1011">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="c209a-1011">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="c209a-1012">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1012">October 9, 2018</span></span>

<span data-ttu-id="c209a-1013">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="c209a-1013">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1014">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1014">Core</span></span>
* <span data-ttu-id="c209a-1015">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="c209a-1015">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1016">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1016">ACR</span></span>
* <span data-ttu-id="c209a-1017">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="c209a-1017">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1018">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1018">ACS</span></span>
* <span data-ttu-id="c209a-1019">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="c209a-1019">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="c209a-1020">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="c209a-1020">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="c209a-1021">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="c209a-1021">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="c209a-1022">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="c209a-1022">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1023">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1023">Container</span></span>
* <span data-ttu-id="c209a-1024">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="c209a-1024">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="c209a-1025">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-1025">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="c209a-1026">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c209a-1026">Event Hub</span></span>
* <span data-ttu-id="c209a-1027">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1027">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="c209a-1028">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c209a-1028">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="c209a-1029">Extensions</span><span class="sxs-lookup"><span data-stu-id="c209a-1029">Extensions</span></span>
* <span data-ttu-id="c209a-1030">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="c209a-1030">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c209a-1031">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c209a-1031">HDInsight</span></span>
* <span data-ttu-id="c209a-1032">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-1032">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1033">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1033">IoT</span></span>
* <span data-ttu-id="c209a-1034">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="c209a-1034">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-1035">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-1035">KeyVault</span></span>
* <span data-ttu-id="c209a-1036">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="c209a-1036">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1037">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1037">Network</span></span>
* <span data-ttu-id="c209a-1038">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="c209a-1038">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="c209a-1039">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="c209a-1039">See #6052</span></span>
* <span data-ttu-id="c209a-1040">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1040">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="c209a-1041">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="c209a-1041">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="c209a-1042">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c209a-1042">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="c209a-1043">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c209a-1043">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="c209a-1044">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="c209a-1044">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="c209a-1045">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1045">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1046">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1046">Role</span></span>
* <span data-ttu-id="c209a-1047">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="c209a-1047">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="c209a-1048">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="c209a-1048">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="c209a-1049">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="c209a-1049">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="c209a-1050">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="c209a-1050">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="c209a-1051">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c209a-1051">Service Bus</span></span>
* <span data-ttu-id="c209a-1052">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c209a-1052">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1053">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1053">VM</span></span>
* <span data-ttu-id="c209a-1054">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="c209a-1054">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="c209a-1055">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1055">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="c209a-1056">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="c209a-1056">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="c209a-1057">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="c209a-1057">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="c209a-1058">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1058">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="c209a-1059">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="c209a-1059">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="c209a-1060">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1060">September 21, 2018</span></span>

<span data-ttu-id="c209a-1061">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="c209a-1061">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1062">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1062">ACR</span></span>
* <span data-ttu-id="c209a-1063">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1063">Added ACR Task commands</span></span>
* <span data-ttu-id="c209a-1064">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="c209a-1064">Added quick run command</span></span>
* <span data-ttu-id="c209a-1065">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c209a-1065">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="c209a-1066">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1066">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="c209a-1067">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="c209a-1067">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="c209a-1068">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="c209a-1068">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1069">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1069">ACS</span></span>
* <span data-ttu-id="c209a-1070">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-1070">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="c209a-1071">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="c209a-1071">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1072">AppService</span></span>

* <span data-ttu-id="c209a-1073">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="c209a-1073">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="c209a-1074">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="c209a-1074">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="c209a-1075">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="c209a-1075">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="c209a-1076">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="c209a-1076">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1077">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1077">Batch</span></span>
* <span data-ttu-id="c209a-1078">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="c209a-1078">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="c209a-1079">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="c209a-1079">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="c209a-1080">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1080">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="c209a-1081">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="c209a-1081">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c209a-1082">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1082">Batch AI</span></span> 
* <span data-ttu-id="c209a-1083">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1083">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c209a-1084">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1084">Cognitive Services</span></span>
* <span data-ttu-id="c209a-1085">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="c209a-1085">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="c209a-1086">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="c209a-1086">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="c209a-1087">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="c209a-1087">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="c209a-1088">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1088">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="c209a-1089">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c209a-1089">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="c209a-1090">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="c209a-1090">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1091">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1091">Container</span></span>
* <span data-ttu-id="c209a-1092">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="c209a-1092">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="c209a-1093">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1093">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="c209a-1094">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c209a-1094">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="c209a-1095">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1095">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="c209a-1096">DataLake</span><span class="sxs-lookup"><span data-stu-id="c209a-1096">Datalake</span></span>
* <span data-ttu-id="c209a-1097">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c209a-1097">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="c209a-1098">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="c209a-1098">Interactive Shell</span></span>
* <span data-ttu-id="c209a-1099">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-1099">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="c209a-1100">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="c209a-1100">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1101">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1101">IoT</span></span>
* <span data-ttu-id="c209a-1102">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1102">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="c209a-1103">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c209a-1103">Key Vault</span></span>
* <span data-ttu-id="c209a-1104">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="c209a-1104">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1105">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1105">Network</span></span>
* <span data-ttu-id="c209a-1106">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1106">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="c209a-1107">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="c209a-1107">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="c209a-1108">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="c209a-1108">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="c209a-1109">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1109">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="c209a-1110">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1110">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="c209a-1111">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1111">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="c209a-1112">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1112">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="c209a-1113">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="c209a-1113">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="c209a-1114">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="c209a-1114">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="c209a-1115">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="c209a-1115">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="c209a-1116">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="c209a-1116">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="c209a-1117">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="c209a-1117">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="c209a-1118">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="c209a-1118">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="c209a-1119">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="c209a-1119">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="c209a-1120">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="c209a-1120">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="c209a-1121">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="c209a-1121">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="c209a-1122">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1122">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="c209a-1123">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="c209a-1123">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-1124">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-1124">RDBMS</span></span>
* <span data-ttu-id="c209a-1125">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="c209a-1125">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="c209a-1126">Réservation</span><span class="sxs-lookup"><span data-stu-id="c209a-1126">Reservation</span></span>
* <span data-ttu-id="c209a-1127">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="c209a-1127">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="c209a-1128">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="c209a-1128">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="c209a-1129">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="c209a-1129">Manage App</span></span>
* <span data-ttu-id="c209a-1130">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="c209a-1130">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="c209a-1131">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="c209a-1131">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1132">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1132">Role</span></span>
* <span data-ttu-id="c209a-1133">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="c209a-1133">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="c209a-1134">SignalR</span><span class="sxs-lookup"><span data-stu-id="c209a-1134">SignalR</span></span>
* <span data-ttu-id="c209a-1135">Première version</span><span class="sxs-lookup"><span data-stu-id="c209a-1135">First release</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1136">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1136">Storage</span></span>
* <span data-ttu-id="c209a-1137">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="c209a-1137">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="c209a-1138">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="c209a-1138">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1139">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1139">VM</span></span>
* <span data-ttu-id="c209a-1140">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="c209a-1140">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="c209a-1141">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="c209a-1141">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="c209a-1142">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1142">August 28, 2018</span></span>

<span data-ttu-id="c209a-1143">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="c209a-1143">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1144">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1144">Core</span></span>

* <span data-ttu-id="c209a-1145">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="c209a-1145">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="c209a-1146">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c209a-1146">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1147">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1147">ACR</span></span>

* <span data-ttu-id="c209a-1148">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c209a-1148">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="c209a-1149">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="c209a-1149">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1150">ACS</span></span>

* <span data-ttu-id="c209a-1151">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="c209a-1151">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="c209a-1152">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="c209a-1152">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1153">AppService</span></span>

* <span data-ttu-id="c209a-1154">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="c209a-1154">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="c209a-1155">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="c209a-1155">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="c209a-1156">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1156">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="c209a-1157">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c209a-1157">Backup</span></span>

* <span data-ttu-id="c209a-1158">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1158">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="c209a-1159">Service de robot</span><span class="sxs-lookup"><span data-stu-id="c209a-1159">Bot Service</span></span>

* <span data-ttu-id="c209a-1160">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="c209a-1160">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c209a-1161">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1161">Cognitive Services</span></span>

* <span data-ttu-id="c209a-1162">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="c209a-1162">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1163">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1163">IoT</span></span>

* <span data-ttu-id="c209a-1164">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="c209a-1164">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-1165">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-1165">Monitor</span></span>

* <span data-ttu-id="c209a-1166">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="c209a-1166">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="c209a-1167">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="c209a-1167">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1168">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1168">Network</span></span>

* <span data-ttu-id="c209a-1169">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1169">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1170">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1170">Resource</span></span>

* <span data-ttu-id="c209a-1171">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1171">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1172">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1172">Storage</span></span>

* <span data-ttu-id="c209a-1173">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1173">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1174">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1174">VM</span></span>

* <span data-ttu-id="c209a-1175">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1175">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="c209a-1176">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1176">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="c209a-1177">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1177">Auguest 14, 2018</span></span>

<span data-ttu-id="c209a-1178">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="c209a-1178">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1179">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1179">Core</span></span>

* <span data-ttu-id="c209a-1180">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="c209a-1180">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="c209a-1181">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="c209a-1181">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="c209a-1182">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="c209a-1182">Telemetry</span></span>

* <span data-ttu-id="c209a-1183">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c209a-1183">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1184">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1184">ACR</span></span>

* <span data-ttu-id="c209a-1185">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="c209a-1185">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="c209a-1186">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c209a-1186">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1187">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1187">ACS</span></span>

* <span data-ttu-id="c209a-1188">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-1188">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="c209a-1189">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-1189">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="c209a-1190">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c209a-1190">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="c209a-1191">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c209a-1191">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="c209a-1192">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="c209a-1192">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="c209a-1193">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1193">AppService</span></span>

* <span data-ttu-id="c209a-1194">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c209a-1194">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="c209a-1195">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="c209a-1195">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-1196">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1196">BatchAI</span></span>

* <span data-ttu-id="c209a-1197">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="c209a-1197">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="c209a-1198">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1198">Container</span></span>

* <span data-ttu-id="c209a-1199">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1199">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="c209a-1200">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1200">IoT</span></span>

* <span data-ttu-id="c209a-1201">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="c209a-1201">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="c209a-1202">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="c209a-1202">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="c209a-1203">Iot Central</span><span class="sxs-lookup"><span data-stu-id="c209a-1203">Iot Central</span></span>

* <span data-ttu-id="c209a-1204">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="c209a-1204">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-1205">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-1205">KeyVault</span></span>


* <span data-ttu-id="c209a-1206">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="c209a-1206">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="c209a-1207">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1207">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="c209a-1208">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="c209a-1208">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="c209a-1209">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c209a-1209">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="c209a-1210">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c209a-1210">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="c209a-1211">Relais</span><span class="sxs-lookup"><span data-stu-id="c209a-1211">Relay</span></span>

* <span data-ttu-id="c209a-1212">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-1212">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1213">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1213">Sql</span></span>

* <span data-ttu-id="c209a-1214">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="c209a-1214">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1215">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1215">Storage</span></span>

* <span data-ttu-id="c209a-1216">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="c209a-1216">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="c209a-1217">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="c209a-1217">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="c209a-1218">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="c209a-1218">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="c209a-1219">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="c209a-1219">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="c209a-1220">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1220">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1221">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1221">VM</span></span>

* <span data-ttu-id="c209a-1222">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="c209a-1222">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="c209a-1223">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1223">July 31, 2018</span></span>

<span data-ttu-id="c209a-1224">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="c209a-1224">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1225">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1225">ACR</span></span>

* <span data-ttu-id="c209a-1226">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1226">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="c209a-1227">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="c209a-1227">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1228">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1228">ACS</span></span>

* <span data-ttu-id="c209a-1229">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="c209a-1229">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1230">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1230">Batch</span></span>

* <span data-ttu-id="c209a-1231">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c209a-1231">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1232">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1232">Container</span></span>

* <span data-ttu-id="c209a-1233">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="c209a-1233">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1234">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1234">Network</span></span>

* <span data-ttu-id="c209a-1235">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c209a-1235">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="c209a-1236">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1236">Resource</span></span>

* <span data-ttu-id="c209a-1237">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-1237">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="c209a-1238">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-1238">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1239">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1239">Role</span></span>

* <span data-ttu-id="c209a-1240">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="c209a-1240">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="c209a-1241">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-1241">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="c209a-1242">Recherche</span><span class="sxs-lookup"><span data-stu-id="c209a-1242">Search</span></span>

* <span data-ttu-id="c209a-1243">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="c209a-1243">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="c209a-1244">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c209a-1244">Service Bus</span></span>

* <span data-ttu-id="c209a-1245">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="c209a-1245">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="c209a-1246">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1246">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="c209a-1247">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="c209a-1247">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="c209a-1248">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="c209a-1248">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1249">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1249">Storage</span></span>

* <span data-ttu-id="c209a-1250">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="c209a-1250">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="c209a-1251">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1251">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1252">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1252">VM</span></span>

* <span data-ttu-id="c209a-1253">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1253">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="c209a-1254">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="c209a-1254">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="c209a-1255">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="c209a-1255">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="c209a-1256">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="c209a-1256">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="c209a-1257">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1257">July 18, 2018</span></span>

<span data-ttu-id="c209a-1258">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="c209a-1258">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1259">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1259">Core</span></span>

* <span data-ttu-id="c209a-1260">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-1260">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="c209a-1261">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c209a-1261">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="c209a-1262">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c209a-1262">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1263">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1263">ACR</span></span>

* <span data-ttu-id="c209a-1264">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="c209a-1264">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="c209a-1265">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="c209a-1265">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="c209a-1266">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="c209a-1266">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="c209a-1267">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="c209a-1267">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1268">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1268">ACS</span></span>

* <span data-ttu-id="c209a-1269">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="c209a-1269">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1270">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1270">AppService</span></span>

* <span data-ttu-id="c209a-1271">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="c209a-1271">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1272">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1272">Batch</span></span>

* <span data-ttu-id="c209a-1273">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c209a-1273">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="c209a-1274">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-1274">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c209a-1275">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1275">Batch AI</span></span>

* <span data-ttu-id="c209a-1276">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="c209a-1276">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1277">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1277">Container</span></span>

* <span data-ttu-id="c209a-1278">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="c209a-1278">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="c209a-1279">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="c209a-1279">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1280">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1280">Network</span></span>

* <span data-ttu-id="c209a-1281">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1281">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="c209a-1282">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-1282">Added `network nic wait`</span></span>
* <span data-ttu-id="c209a-1283">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1283">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="c209a-1284">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1284">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="c209a-1285">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1285">Resource</span></span>

* <span data-ttu-id="c209a-1286">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-1286">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="c209a-1287">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-1287">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="c209a-1288">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-1288">Added `deployment wait` command</span></span>
* <span data-ttu-id="c209a-1289">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="c209a-1289">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1290">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1290">SQL</span></span>

* <span data-ttu-id="c209a-1291">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1291">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="c209a-1292">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="c209a-1292">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="c209a-1293">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="c209a-1293">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1294">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1294">Storage</span></span>

* <span data-ttu-id="c209a-1295">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="c209a-1295">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1296">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1296">VM</span></span>

* <span data-ttu-id="c209a-1297">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1297">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="c209a-1298">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1298">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="c209a-1299">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="c209a-1299">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c209a-1300">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1300">July 3, 2018</span></span>

<span data-ttu-id="c209a-1301">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="c209a-1301">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="c209a-1302">AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-1302">AKS</span></span>

* <span data-ttu-id="c209a-1303">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1303">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c209a-1304">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1304">July 3, 2018</span></span>

<span data-ttu-id="c209a-1305">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="c209a-1305">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1306">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1306">Core</span></span>

* <span data-ttu-id="c209a-1307">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1307">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1308">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1308">ACR</span></span>

* <span data-ttu-id="c209a-1309">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="c209a-1309">Added polling build status</span></span>
* <span data-ttu-id="c209a-1310">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-1310">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="c209a-1311">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c209a-1311">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1312">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1312">ACS</span></span>

* <span data-ttu-id="c209a-1313">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1313">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="c209a-1314">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1314">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="c209a-1315">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1315">Updated options for `aks browse` command.</span></span> <span data-ttu-id="c209a-1316">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="c209a-1316">Added `--listen-port` support</span></span>
* <span data-ttu-id="c209a-1317">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1317">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="c209a-1318">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="c209a-1318">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="c209a-1319">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="c209a-1319">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1320">AppService</span></span>

* <span data-ttu-id="c209a-1321">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="c209a-1321">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="c209a-1322">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="c209a-1322">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="c209a-1323">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c209a-1323">Backup</span></span>

* <span data-ttu-id="c209a-1324">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="c209a-1324">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-1325">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1325">BatchAI</span></span>

* <span data-ttu-id="c209a-1326">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1326">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="c209a-1327">Cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-1327">Cloud</span></span>

* <span data-ttu-id="c209a-1328">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-1328">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1329">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1329">Container</span></span>

* <span data-ttu-id="c209a-1330">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="c209a-1330">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="c209a-1331">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="c209a-1331">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="c209a-1332">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="c209a-1332">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1333">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1333">Extension</span></span>

* <span data-ttu-id="c209a-1334">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="c209a-1334">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1335">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1335">Network</span></span>

* <span data-ttu-id="c209a-1336">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="c209a-1336">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-1337">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c209a-1337">Rdbms</span></span>

* <span data-ttu-id="c209a-1338">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-1338">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1339">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1339">Resource</span></span>

* <span data-ttu-id="c209a-1340">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="c209a-1340">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1341">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1341">VM</span></span>

* <span data-ttu-id="c209a-1342">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="c209a-1342">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="c209a-1343">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1343">June 25, 2018</span></span>

<span data-ttu-id="c209a-1344">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="c209a-1344">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="c209a-1345">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-1345">CLI</span></span>

* <span data-ttu-id="c209a-1346">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1346">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="c209a-1347">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1347">June 19, 2018</span></span>

<span data-ttu-id="c209a-1348">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="c209a-1348">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1349">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1349">Core</span></span>

* <span data-ttu-id="c209a-1350">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1350">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1351">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1351">ACR</span></span>

* <span data-ttu-id="c209a-1352">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="c209a-1352">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="c209a-1353">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1353">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1354">ACS</span></span>

* <span data-ttu-id="c209a-1355">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1355">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="c209a-1356">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1356">Added `--update` support</span></span>
* <span data-ttu-id="c209a-1357">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="c209a-1357">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="c209a-1358">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="c209a-1358">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="c209a-1359">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="c209a-1359">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="c209a-1360">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c209a-1360">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="c209a-1361">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c209a-1361">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="c209a-1362">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c209a-1362">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1363">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1363">AppService</span></span>

* <span data-ttu-id="c209a-1364">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="c209a-1364">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="c209a-1365">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c209a-1365">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1366">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1366">Batch</span></span>

* <span data-ttu-id="c209a-1367">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="c209a-1367">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c209a-1368">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1368">Batch AI</span></span>

* <span data-ttu-id="c209a-1369">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="c209a-1369">Added support for workspaces.</span></span> <span data-ttu-id="c209a-1370">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="c209a-1370">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="c209a-1371">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="c209a-1371">Added support for experiments.</span></span> <span data-ttu-id="c209a-1372">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="c209a-1372">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="c209a-1373">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="c209a-1373">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="c209a-1374">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1374">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="c209a-1375">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="c209a-1375">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="c209a-1376">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="c209a-1376">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="c209a-1377">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="c209a-1377">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="c209a-1378">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="c209a-1378">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="c209a-1379">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1379">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="c209a-1380">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="c209a-1380">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="c209a-1381">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1381">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="c209a-1382">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="c209a-1382">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="c209a-1383">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="c209a-1383">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="c209a-1384">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="c209a-1384">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="c209a-1385">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1385">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="c209a-1386">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="c209a-1386">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="c209a-1387">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="c209a-1387">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="c209a-1388">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c209a-1388">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c209a-1389">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c209a-1389">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c209a-1390">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="c209a-1390">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="c209a-1391">Cartes</span><span class="sxs-lookup"><span data-stu-id="c209a-1391">Maps</span></span>

* <span data-ttu-id="c209a-1392">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="c209a-1392">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1393">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1393">Network</span></span>

* <span data-ttu-id="c209a-1394">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="c209a-1394">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="c209a-1395">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="c209a-1395">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="c209a-1396">#6502</span><span class="sxs-lookup"><span data-stu-id="c209a-1396">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="c209a-1397">Réservations</span><span class="sxs-lookup"><span data-stu-id="c209a-1397">Reservations</span></span>

* <span data-ttu-id="c209a-1398">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1398">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="c209a-1399">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1399">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="c209a-1400">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="c209a-1400">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="c209a-1401">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c209a-1401">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="c209a-1402">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c209a-1402">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="c209a-1403">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1403">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1404">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1404">Role</span></span>

* <span data-ttu-id="c209a-1405">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1405">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1406">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1406">SQL</span></span>

* <span data-ttu-id="c209a-1407">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1407">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1408">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1408">Storage</span></span>

* <span data-ttu-id="c209a-1409">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="c209a-1409">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1410">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1410">VM</span></span>

* <span data-ttu-id="c209a-1411">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1411">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="c209a-1412">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="c209a-1412">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="c209a-1413">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="c209a-1413">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c209a-1414">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1414">June 13, 2018</span></span>

<span data-ttu-id="c209a-1415">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="c209a-1415">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1416">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1416">Core</span></span>

* <span data-ttu-id="c209a-1417">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1417">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c209a-1418">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1418">June 13, 2018</span></span>

<span data-ttu-id="c209a-1419">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="c209a-1419">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="c209a-1420">AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-1420">AKS</span></span>

* <span data-ttu-id="c209a-1421">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1421">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="c209a-1422">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="c209a-1422">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="c209a-1423">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1423">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="c209a-1424">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1424">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="c209a-1425">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1425">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1426">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1426">AppService</span></span>

* <span data-ttu-id="c209a-1427">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="c209a-1427">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c209a-1428">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1428">June 5, 2018</span></span>

<span data-ttu-id="c209a-1429">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="c209a-1429">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1430">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1430">Interactive</span></span>

* <span data-ttu-id="c209a-1431">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c209a-1431">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c209a-1432">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1432">June 5, 2018</span></span>

<span data-ttu-id="c209a-1433">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="c209a-1433">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1434">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1434">Core</span></span>

* <span data-ttu-id="c209a-1435">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="c209a-1435">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="c209a-1436">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c209a-1436">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1437">ACR</span></span>

* <span data-ttu-id="c209a-1438">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="c209a-1438">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="c209a-1439">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="c209a-1439">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="c209a-1440">AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-1440">AKS</span></span>

* <span data-ttu-id="c209a-1441">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="c209a-1441">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1442">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1442">Batch</span></span>

* <span data-ttu-id="c209a-1443">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="c209a-1443">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1444">IOT</span><span class="sxs-lookup"><span data-stu-id="c209a-1444">IOT</span></span>

* <span data-ttu-id="c209a-1445">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="c209a-1445">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1446">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1446">Network</span></span>

* <span data-ttu-id="c209a-1447">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="c209a-1447">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c209a-1448">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c209a-1448">Policy Insights</span></span>

* <span data-ttu-id="c209a-1449">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-1449">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="c209a-1450">ARM</span><span class="sxs-lookup"><span data-stu-id="c209a-1450">ARM</span></span>

* <span data-ttu-id="c209a-1451">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1451">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1452">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1452">SQL</span></span>

* <span data-ttu-id="c209a-1453">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="c209a-1453">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="c209a-1454">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="c209a-1454">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="c209a-1455">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1455">Storage</span></span>

* <span data-ttu-id="c209a-1456">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="c209a-1456">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1457">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1457">VM</span></span>

* <span data-ttu-id="c209a-1458">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="c209a-1458">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="c209a-1459">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1459">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="c209a-1460">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1460">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="c209a-1461">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1461">May 22, 2018</span></span>

<span data-ttu-id="c209a-1462">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="c209a-1462">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1463">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1463">Core</span></span>

* <span data-ttu-id="c209a-1464">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="c209a-1464">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1465">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1465">ACS</span></span>

* <span data-ttu-id="c209a-1466">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="c209a-1466">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="c209a-1467">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="c209a-1467">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1468">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1468">AppService</span></span>

* <span data-ttu-id="c209a-1469">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c209a-1469">Improved generic update commands</span></span>
* <span data-ttu-id="c209a-1470">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="c209a-1470">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1471">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1471">Container</span></span>

* <span data-ttu-id="c209a-1472">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="c209a-1472">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="c209a-1473">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1473">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1474">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1474">Extension</span></span>

* <span data-ttu-id="c209a-1475">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="c209a-1475">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1476">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1476">Interactive</span></span>

* <span data-ttu-id="c209a-1477">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1477">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="c209a-1478">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="c209a-1478">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-1479">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-1479">KeyVault</span></span>

* <span data-ttu-id="c209a-1480">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c209a-1480">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1481">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1481">Network</span></span>

* <span data-ttu-id="c209a-1482">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="c209a-1482">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="c209a-1483">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="c209a-1483">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1484">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1484">SQL</span></span>

* <span data-ttu-id="c209a-1485">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="c209a-1485">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="c209a-1486">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="c209a-1486">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="c209a-1487">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="c209a-1487">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="c209a-1488">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c209a-1488">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="c209a-1489">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c209a-1489">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="c209a-1490">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1490">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="c209a-1491">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="c209a-1491">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="c209a-1492">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1492">`edition`.</span></span> <span data-ttu-id="c209a-1493">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="c209a-1493">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="c209a-1494">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1494">`elasticPoolName`.</span></span> <span data-ttu-id="c209a-1495">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="c209a-1495">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="c209a-1496">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c209a-1496">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="c209a-1497">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1497">`edition`.</span></span> <span data-ttu-id="c209a-1498">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="c209a-1498">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="c209a-1499">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1499">`dtu`.</span></span> <span data-ttu-id="c209a-1500">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="c209a-1500">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="c209a-1501">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1501">`databaseDtuMin`.</span></span> <span data-ttu-id="c209a-1502">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="c209a-1502">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="c209a-1503">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1503">`databaseDtuMax`.</span></span> <span data-ttu-id="c209a-1504">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="c209a-1504">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="c209a-1505">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c209a-1505">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="c209a-1506">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c209a-1506">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1507">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1507">Storage</span></span>

* <span data-ttu-id="c209a-1508">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-1508">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="c209a-1509">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="c209a-1509">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1510">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1510">VM</span></span>

* <span data-ttu-id="c209a-1511">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1511">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="c209a-1512">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="c209a-1512">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="c209a-1513">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="c209a-1513">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="c209a-1514">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="c209a-1514">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="c209a-1515">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1515">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="c209a-1516">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1516">May 7, 2018</span></span>

<span data-ttu-id="c209a-1517">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="c209a-1517">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1518">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1518">Core</span></span>

* <span data-ttu-id="c209a-1519">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="c209a-1519">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="c209a-1520">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="c209a-1520">Added limited support for positional arguments</span></span>
* <span data-ttu-id="c209a-1521">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1521">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="c209a-1522">#5591</span><span class="sxs-lookup"><span data-stu-id="c209a-1522">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="c209a-1523">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1523">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="c209a-1524">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="c209a-1524">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="c209a-1525">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1525">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="c209a-1526">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="c209a-1526">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="c209a-1527">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-1527">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1528">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1528">ACR</span></span>

* <span data-ttu-id="c209a-1529">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1529">Added ACR Build commands</span></span>
* <span data-ttu-id="c209a-1530">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="c209a-1530">Improved resource not found error messages</span></span>
* <span data-ttu-id="c209a-1531">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1531">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="c209a-1532">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="c209a-1532">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="c209a-1533">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="c209a-1533">Improved repository commands error messages</span></span>
* <span data-ttu-id="c209a-1534">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="c209a-1534">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1535">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1535">ACS</span></span>

* <span data-ttu-id="c209a-1536">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-1536">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="c209a-1537">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c209a-1537">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="c209a-1538">AMS</span><span class="sxs-lookup"><span data-stu-id="c209a-1538">AMS</span></span>

* <span data-ttu-id="c209a-1539">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1539">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1540">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1540">Appservice</span></span>

* <span data-ttu-id="c209a-1541">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="c209a-1541">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="c209a-1542">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1542">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="c209a-1543">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="c209a-1543">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="c209a-1544">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1544">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c209a-1545">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1545">Batch AI</span></span>

* <span data-ttu-id="c209a-1546">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="c209a-1546">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c209a-1547">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1547">Cognitive Services</span></span>

* <span data-ttu-id="c209a-1548">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="c209a-1548">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-1549">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-1549">Consumption</span></span>

* <span data-ttu-id="c209a-1550">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="c209a-1550">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1551">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1551">Container</span></span>

* <span data-ttu-id="c209a-1552">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="c209a-1552">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c209a-1553">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c209a-1553">Cosmos DB</span></span>

* <span data-ttu-id="c209a-1554">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c209a-1554">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="c209a-1555">DMS</span><span class="sxs-lookup"><span data-stu-id="c209a-1555">DMS</span></span>

* <span data-ttu-id="c209a-1556">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="c209a-1556">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1557">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1557">Extension</span></span>

* <span data-ttu-id="c209a-1558">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="c209a-1558">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1559">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1559">Interactive</span></span>

* <span data-ttu-id="c209a-1560">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="c209a-1560">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="c209a-1561">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="c209a-1561">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="c209a-1562">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="c209a-1562">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="c209a-1563">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1563">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="c209a-1564">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-1564">Lab</span></span>

* <span data-ttu-id="c209a-1565">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="c209a-1565">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1566">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1566">Network</span></span>

* <span data-ttu-id="c209a-1567">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="c209a-1567">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="c209a-1568">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1568">Profile</span></span>

* <span data-ttu-id="c209a-1569">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1569">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="c209a-1570">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="c209a-1570">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="c209a-1571">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="c209a-1571">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="c209a-1572">Redis</span><span class="sxs-lookup"><span data-stu-id="c209a-1572">Redis</span></span>

* <span data-ttu-id="c209a-1573">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1573">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="c209a-1574">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="c209a-1574">Deprecated `redis list-all`.</span></span> <span data-ttu-id="c209a-1575">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1575">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="c209a-1576">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="c209a-1576">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="c209a-1577">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1577">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1578">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1578">Role</span></span>

* <span data-ttu-id="c209a-1579">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c209a-1579">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1580">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1580">Storage</span></span>

* <span data-ttu-id="c209a-1581">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="c209a-1581">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="c209a-1582">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="c209a-1582">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="c209a-1583">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="c209a-1583">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="c209a-1584">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="c209a-1584">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="c209a-1585">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1585">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1586">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1586">VM</span></span>

* <span data-ttu-id="c209a-1587">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="c209a-1587">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="c209a-1588">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c209a-1588">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="c209a-1589">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="c209a-1589">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="c209a-1590">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="c209a-1590">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="c209a-1591">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="c209a-1591">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="c209a-1592">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="c209a-1592">Added write accelerator support</span></span>
* <span data-ttu-id="c209a-1593">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c209a-1593">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="c209a-1594">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1594">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="c209a-1595">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="c209a-1595">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="c209a-1596">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1596">April 10, 2018</span></span>

<span data-ttu-id="c209a-1597">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="c209a-1597">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1598">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1598">ACR</span></span>

* <span data-ttu-id="c209a-1599">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="c209a-1599">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1600">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1600">ACS</span></span>

* <span data-ttu-id="c209a-1601">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="c209a-1601">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1602">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1602">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="c209a-1604">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="c209a-1604">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-1605">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1605">BatchAI</span></span>

* <span data-ttu-id="c209a-1606">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="c209a-1606">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="c209a-1607">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="c209a-1607">Job level mounting</span></span>
  - <span data-ttu-id="c209a-1608">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="c209a-1608">Environment variables with secret values</span></span>
  - <span data-ttu-id="c209a-1609">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="c209a-1609">Performance counters settings</span></span>
  - <span data-ttu-id="c209a-1610">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="c209a-1610">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="c209a-1611">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="c209a-1611">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="c209a-1612">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="c209a-1612">Usage and limits reporting</span></span>
  - <span data-ttu-id="c209a-1613">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="c209a-1613">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="c209a-1614">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="c209a-1614">Support for custom images</span></span>
  - <span data-ttu-id="c209a-1615">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="c209a-1615">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="c209a-1616">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="c209a-1616">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="c209a-1617">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="c209a-1617">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="c209a-1618">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="c209a-1618">National clouds are supported</span></span>
* <span data-ttu-id="c209a-1619">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="c209a-1619">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="c209a-1620">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="c209a-1620">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="c209a-1621">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-1621">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="c209a-1622">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="c209a-1622">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="c209a-1623">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="c209a-1623">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="c209a-1624">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="c209a-1624">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="c209a-1625">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1625">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="c209a-1626">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="c209a-1626">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="c209a-1627">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="c209a-1627">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="c209a-1628">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1628">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="c209a-1629">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-1629">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="c209a-1630">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="c209a-1630">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="c209a-1631">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1631">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="c209a-1632">Facturation</span><span class="sxs-lookup"><span data-stu-id="c209a-1632">Billing</span></span>

* <span data-ttu-id="c209a-1633">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="c209a-1633">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-1634">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-1634">Consumption</span></span>

* <span data-ttu-id="c209a-1635">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="c209a-1635">Added `marketplace` commands</span></span>
* <span data-ttu-id="c209a-1636">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c209a-1636">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="c209a-1637">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="c209a-1637">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="c209a-1638">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="c209a-1638">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="c209a-1639">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c209a-1639">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="c209a-1640">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="c209a-1640">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1641">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1641">Container</span></span>

* <span data-ttu-id="c209a-1642">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="c209a-1642">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="c209a-1643">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="c209a-1643">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1644">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1644">Extension</span></span>

* <span data-ttu-id="c209a-1645">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="c209a-1645">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1646">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1646">Interactive</span></span>

* <span data-ttu-id="c209a-1647">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="c209a-1647">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="c209a-1648">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-1648">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="c209a-1649">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="c209a-1649">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1650">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1650">Network</span></span>

* <span data-ttu-id="c209a-1651">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="c209a-1651">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="c209a-1652">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c209a-1652">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="c209a-1653">#4910</span><span class="sxs-lookup"><span data-stu-id="c209a-1653">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="c209a-1654">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c209a-1654">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="c209a-1655">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c209a-1655">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="c209a-1656">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1656">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="c209a-1657">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1657">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="c209a-1658">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="c209a-1658">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-1659">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1659">Profile</span></span>

* <span data-ttu-id="c209a-1660">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1660">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="c209a-1661">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="c209a-1661">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-1662">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-1662">RDBMS</span></span>

* <span data-ttu-id="c209a-1663">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="c209a-1663">Added `georestore` command</span></span>
* <span data-ttu-id="c209a-1664">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1664">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1665">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1665">Resource</span></span>

* <span data-ttu-id="c209a-1666">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1666">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="c209a-1667">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1667">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1668">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1668">SQL</span></span>

* <span data-ttu-id="c209a-1669">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="c209a-1669">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1670">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1670">Storage</span></span>

* <span data-ttu-id="c209a-1671">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="c209a-1671">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1672">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1672">VM</span></span>

* <span data-ttu-id="c209a-1673">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1673">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="c209a-1674">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="c209a-1674">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="c209a-1676">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1676">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="c209a-1677">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="c209a-1677">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="c209a-1678">#5718</span><span class="sxs-lookup"><span data-stu-id="c209a-1678">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="c209a-1679">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="c209a-1679">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="c209a-1680">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1680">March 27, 2018</span></span>

<span data-ttu-id="c209a-1681">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="c209a-1681">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1682">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1682">Core</span></span>

* <span data-ttu-id="c209a-1683">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="c209a-1683">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1684">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1684">ACS</span></span>

* <span data-ttu-id="c209a-1685">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c209a-1685">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1686">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1686">Appservice</span></span>

* <span data-ttu-id="c209a-1687">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1687">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="c209a-1688">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1688">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c209a-1689">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c209a-1689">Backup</span></span>

* <span data-ttu-id="c209a-1690">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="c209a-1690">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="c209a-1691">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-1691">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="c209a-1692">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c209a-1692">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="c209a-1693">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1693">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1694">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1694">Container</span></span>

* <span data-ttu-id="c209a-1695">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="c209a-1695">Added `container exec` command.</span></span> <span data-ttu-id="c209a-1696">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="c209a-1696">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="c209a-1697">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1697">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1698">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1698">Extension</span></span>

* <span data-ttu-id="c209a-1699">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-1699">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="c209a-1700">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="c209a-1700">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="c209a-1701">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1701">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1702">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1702">Interactive</span></span>

* <span data-ttu-id="c209a-1703">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-1703">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="c209a-1704">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="c209a-1704">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="c209a-1705">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="c209a-1705">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="c209a-1706">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="c209a-1706">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="c209a-1707">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-1707">Lab</span></span>

* <span data-ttu-id="c209a-1708">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="c209a-1708">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-1709">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-1709">Monitor</span></span>

* <span data-ttu-id="c209a-1710">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c209a-1710">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="c209a-1711">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="c209a-1711">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="c209a-1712">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c209a-1712">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1713">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1713">Network</span></span>

* <span data-ttu-id="c209a-1714">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c209a-1714">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-1715">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1715">Profile</span></span>

* <span data-ttu-id="c209a-1716">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="c209a-1716">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-1717">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-1717">RDBMS</span></span>

* <span data-ttu-id="c209a-1718">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="c209a-1718">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1719">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1719">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="c209a-1721">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1721">Role</span></span>

* <span data-ttu-id="c209a-1722">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1722">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="c209a-1723">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="c209a-1723">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="c209a-1724">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1724">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="c209a-1725">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1725">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="c209a-1726">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="c209a-1726">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1727">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1727">Storage</span></span>

* <span data-ttu-id="c209a-1728">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="c209a-1728">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="c209a-1729">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="c209a-1729">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1730">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1730">VM</span></span>

* <span data-ttu-id="c209a-1731">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="c209a-1731">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="c209a-1732">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1732">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="c209a-1733">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c209a-1733">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="c209a-1734">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="c209a-1734">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="c209a-1735">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1735">March 13, 2018</span></span>

<span data-ttu-id="c209a-1736">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="c209a-1736">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1737">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1737">ACR</span></span>

* <span data-ttu-id="c209a-1738">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-1738">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="c209a-1739">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="c209a-1739">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="c209a-1740">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="c209a-1740">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1741">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1741">ACS</span></span>

* <span data-ttu-id="c209a-1742">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="c209a-1742">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="c209a-1743">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="c209a-1743">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="c209a-1744">Advisor</span><span class="sxs-lookup"><span data-stu-id="c209a-1744">Advisor</span></span>

* <span data-ttu-id="c209a-1745">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1745">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="c209a-1746">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1746">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="c209a-1747">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="c209a-1747">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="c209a-1748">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="c209a-1748">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="c209a-1749">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1749">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1750">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1750">Appservice</span></span>

* <span data-ttu-id="c209a-1751">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c209a-1751">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="c209a-1752">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1752">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c209a-1753">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c209a-1753">Eventhubs</span></span>

* <span data-ttu-id="c209a-1754">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-1754">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1755">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1755">Extension</span></span>

* <span data-ttu-id="c209a-1756">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1756">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1757">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1757">Interactive</span></span>

* <span data-ttu-id="c209a-1758">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="c209a-1758">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="c209a-1759">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="c209a-1759">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="c209a-1760">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="c209a-1760">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="c209a-1761">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="c209a-1761">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-1762">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-1762">Monitor</span></span>

* <span data-ttu-id="c209a-1763">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="c209a-1763">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="c209a-1764">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="c209a-1764">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="c209a-1765">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="c209a-1765">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="c209a-1766">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-1766">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1767">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1767">Network</span></span>

* <span data-ttu-id="c209a-1768">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1768">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="c209a-1769">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c209a-1769">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="c209a-1770">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="c209a-1770">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="c209a-1771">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="c209a-1771">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-1772">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1772">Profile</span></span>

* <span data-ttu-id="c209a-1773">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="c209a-1773">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="c209a-1774">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="c209a-1774">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-1775">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-1775">RDBMS</span></span>

* <span data-ttu-id="c209a-1776">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-1776">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="c209a-1777">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c209a-1777">Service Bus</span></span>

* <span data-ttu-id="c209a-1778">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-1778">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1779">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1779">Storage</span></span>

* <span data-ttu-id="c209a-1780">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="c209a-1780">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="c209a-1781">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="c209a-1781">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1782">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1782">VM</span></span>

* <span data-ttu-id="c209a-1783">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="c209a-1783">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="c209a-1784">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="c209a-1784">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="c209a-1785">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="c209a-1785">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="c209a-1786">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="c209a-1786">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="c209a-1787">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1787">February 27, 2018</span></span>

<span data-ttu-id="c209a-1788">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="c209a-1788">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1789">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1789">Core</span></span>

* <span data-ttu-id="c209a-1790">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="c209a-1790">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="c209a-1791">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="c209a-1791">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="c209a-1792">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="c209a-1792">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1793">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1793">ACS</span></span>

* <span data-ttu-id="c209a-1794">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1794">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="c209a-1795">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="c209a-1795">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="c209a-1796">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c209a-1796">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="c209a-1797">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="c209a-1797">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1798">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1798">Appservice</span></span>

* <span data-ttu-id="c209a-1799">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="c209a-1799">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="c209a-1800">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="c209a-1800">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c209a-1801">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1801">Cognitive Services</span></span>

* <span data-ttu-id="c209a-1802">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-1802">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-1803">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-1803">Consumption</span></span>

* <span data-ttu-id="c209a-1804">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="c209a-1804">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="c209a-1805">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="c209a-1805">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1806">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1806">Container</span></span>

* <span data-ttu-id="c209a-1807">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="c209a-1807">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1808">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1808">Network</span></span>

* <span data-ttu-id="c209a-1809">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="c209a-1809">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1810">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1810">Resource</span></span>

* <span data-ttu-id="c209a-1811">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="c209a-1811">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1812">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1812">Role</span></span>

* <span data-ttu-id="c209a-1813">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="c209a-1813">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1814">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1814">SQL</span></span>

* <span data-ttu-id="c209a-1815">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="c209a-1815">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1816">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1816">Storage</span></span>

* <span data-ttu-id="c209a-1817">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1817">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1818">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1818">VM</span></span>

* <span data-ttu-id="c209a-1819">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="c209a-1819">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="c209a-1820">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1820">February 13, 2018</span></span>

<span data-ttu-id="c209a-1821">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="c209a-1821">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1822">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1822">Core</span></span>

* <span data-ttu-id="c209a-1823">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="c209a-1823">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1824">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1824">ACS</span></span>

* <span data-ttu-id="c209a-1825">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="c209a-1825">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="c209a-1826">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1826">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="c209a-1827">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c209a-1827">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="c209a-1828">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-1828">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="c209a-1829">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="c209a-1829">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="c209a-1830">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="c209a-1830">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="c209a-1831">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c209a-1831">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="c209a-1832">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="c209a-1832">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1833">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1833">Appservice</span></span>

* <span data-ttu-id="c209a-1834">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="c209a-1834">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="c209a-1835">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="c209a-1835">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-1836">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-1836">CDN</span></span>

* <span data-ttu-id="c209a-1837">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1837">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1838">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1838">Container</span></span>

* <span data-ttu-id="c209a-1839">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="c209a-1839">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="c209a-1840">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1840">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-1841">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-1841">CosmosDB</span></span>

* <span data-ttu-id="c209a-1842">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c209a-1842">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-1843">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-1843">Extension</span></span>

* <span data-ttu-id="c209a-1844">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1844">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="c209a-1845">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1845">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="c209a-1846">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c209a-1846">Feedback</span></span>

* <span data-ttu-id="c209a-1847">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c209a-1847">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1848">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1848">Interactive</span></span>

* <span data-ttu-id="c209a-1849">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c209a-1849">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="c209a-1850">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="c209a-1850">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1851">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1851">IoT</span></span>

* <span data-ttu-id="c209a-1852">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c209a-1852">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c209a-1853">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c209a-1853">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c209a-1854">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1854">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="c209a-1855">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="c209a-1855">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-1856">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-1856">Monitor</span></span>

* <span data-ttu-id="c209a-1857">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1857">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1858">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1858">Network</span></span>

* <span data-ttu-id="c209a-1859">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c209a-1859">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="c209a-1860">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1860">Profile</span></span>

* <span data-ttu-id="c209a-1861">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c209a-1861">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1862">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1862">Resource</span></span>

* <span data-ttu-id="c209a-1863">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="c209a-1863">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1864">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1864">Role</span></span>

* <span data-ttu-id="c209a-1865">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1865">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-1866">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-1866">SQL</span></span>

* <span data-ttu-id="c209a-1867">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="c209a-1867">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="c209a-1868">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="c209a-1868">Added `sql db rename`</span></span>
* <span data-ttu-id="c209a-1869">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="c209a-1869">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1870">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1870">Storage</span></span>

* <span data-ttu-id="c209a-1871">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="c209a-1871">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1872">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1872">VM</span></span>

* <span data-ttu-id="c209a-1873">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="c209a-1873">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="c209a-1874">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="c209a-1874">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="c209a-1875">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="c209a-1875">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="c209a-1876">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1876">January 31, 2018</span></span>

<span data-ttu-id="c209a-1877">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="c209a-1877">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="c209a-1878">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-1878">Core</span></span>

* <span data-ttu-id="c209a-1879">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="c209a-1879">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="c209a-1880">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-1880">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="c209a-1881">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="c209a-1881">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="c209a-1882">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="c209a-1882">Use `--verbose` to see</span></span>
* <span data-ttu-id="c209a-1883">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="c209a-1883">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1884">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1884">ACS</span></span>

* <span data-ttu-id="c209a-1885">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="c209a-1885">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="c209a-1886">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="c209a-1886">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1887">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1887">Appservice</span></span>

* <span data-ttu-id="c209a-1888">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="c209a-1888">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="c209a-1889">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="c209a-1889">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-1890">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-1890">CDN</span></span>

* <span data-ttu-id="c209a-1891">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1891">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-1892">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-1892">CosmosDB</span></span>

* <span data-ttu-id="c209a-1893">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="c209a-1893">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1894">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1894">Interactive</span></span>

* <span data-ttu-id="c209a-1895">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="c209a-1895">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1896">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1896">Network</span></span>

* <span data-ttu-id="c209a-1897">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1897">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="c209a-1898">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1898">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="c209a-1899">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1899">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="c209a-1900">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1900">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="c209a-1901">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="c209a-1901">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="c209a-1902">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="c209a-1902">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="c209a-1903">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="c209a-1903">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="c209a-1904">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="c209a-1904">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="c209a-1905">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c209a-1905">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="c209a-1906">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="c209a-1906">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-1907">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1907">Profile</span></span>

* <span data-ttu-id="c209a-1908">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c209a-1908">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-1909">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-1909">Resource</span></span>

* <span data-ttu-id="c209a-1910">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="c209a-1910">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1911">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1911">Storage</span></span>

* <span data-ttu-id="c209a-1912">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="c209a-1912">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="c209a-1913">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="c209a-1913">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="c209a-1914">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-1914">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="c209a-1915">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1915">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="c209a-1916">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="c209a-1916">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1917">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1917">VM</span></span>

* <span data-ttu-id="c209a-1918">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="c209a-1918">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="c209a-1919">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="c209a-1919">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="c209a-1920">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="c209a-1920">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="c209a-1921">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1921">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="c209a-1922">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c209a-1922">January 17, 2018</span></span>

<span data-ttu-id="c209a-1923">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="c209a-1923">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-1924">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-1924">ACR</span></span>

* <span data-ttu-id="c209a-1925">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-1925">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="c209a-1926">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="c209a-1926">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-1927">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-1927">ACS</span></span>

* <span data-ttu-id="c209a-1928">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c209a-1928">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="c209a-1929">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="c209a-1929">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-1930">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-1930">Appservice</span></span>

* <span data-ttu-id="c209a-1931">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="c209a-1931">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="c209a-1932">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="c209a-1932">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="c209a-1933">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="c209a-1933">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="c209a-1934">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c209a-1934">Backup</span></span>

* <span data-ttu-id="c209a-1935">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="c209a-1935">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="c209a-1936">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="c209a-1936">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="c209a-1937">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-1937">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="c209a-1938">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="c209a-1938">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="c209a-1939">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-1939">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-1940">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-1940">Batch</span></span>

* <span data-ttu-id="c209a-1941">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="c209a-1941">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="c209a-1942">Cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-1942">Cloud</span></span>

* <span data-ttu-id="c209a-1943">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-1943">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-1944">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-1944">Consumption</span></span>

* <span data-ttu-id="c209a-1945">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="c209a-1945">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="c209a-1946">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c209a-1946">Event Grid</span></span>

* <span data-ttu-id="c209a-1947">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c209a-1947">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c209a-1948">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c209a-1948">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c209a-1949">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="c209a-1949">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="c209a-1950">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="c209a-1950">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="c209a-1951">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1951">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="c209a-1952">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1952">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="c209a-1953">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="c209a-1953">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="c209a-1954">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="c209a-1954">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-1955">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-1955">Interactive</span></span>

* <span data-ttu-id="c209a-1956">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="c209a-1956">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="c209a-1957">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="c209a-1957">Fixed errors on startup</span></span>
* <span data-ttu-id="c209a-1958">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="c209a-1958">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-1959">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1959">IoT</span></span>

* <span data-ttu-id="c209a-1960">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="c209a-1960">Added support for device provisioning service</span></span>
* <span data-ttu-id="c209a-1961">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1961">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="c209a-1962">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-1962">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-1963">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-1963">Monitor</span></span>

* <span data-ttu-id="c209a-1964">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="c209a-1964">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="c209a-1965">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1965">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="c209a-1966">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="c209a-1966">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1967">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1967">Network</span></span>

* <span data-ttu-id="c209a-1968">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="c209a-1968">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="c209a-1969">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1969">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-1970">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-1970">Profile</span></span>

* <span data-ttu-id="c209a-1971">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1971">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="c209a-1972">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-1972">Role</span></span>

* <span data-ttu-id="c209a-1973">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="c209a-1973">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c209a-1974">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c209a-1974">Service Fabric</span></span>

* <span data-ttu-id="c209a-1975">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="c209a-1975">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="c209a-1976">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-1976">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1977">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1977">VM</span></span>

* <span data-ttu-id="c209a-1978">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="c209a-1978">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="c209a-1979">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="c209a-1979">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="c209a-1980">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="c209a-1980">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="c209a-1981">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="c209a-1981">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="c209a-1982">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="c209a-1982">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="c209a-1983">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1983">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c209a-1984">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-1984">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="c209a-1985">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="c209a-1985">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="c209a-1986">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-1986">December 19, 2017</span></span>

<span data-ttu-id="c209a-1987">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="c209a-1987">Version 2.0.23</span></span>

* <span data-ttu-id="c209a-1988">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c209a-1988">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="c209a-1989">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1989">Container</span></span>

* <span data-ttu-id="c209a-1990">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-1990">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="c209a-1991">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-1991">Network</span></span>

* <span data-ttu-id="c209a-1992">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1992">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="c209a-1993">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-1993">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-1994">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-1994">Storage</span></span>

* <span data-ttu-id="c209a-1995">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="c209a-1995">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-1996">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-1996">VM</span></span>

* <span data-ttu-id="c209a-1997">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="c209a-1997">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="c209a-1998">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-1998">December 5, 2017</span></span>

<span data-ttu-id="c209a-1999">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="c209a-1999">Version 2.0.22</span></span>

* <span data-ttu-id="c209a-2000">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="c209a-2000">Removed `az component` commands.</span></span> <span data-ttu-id="c209a-2001">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="c209a-2001">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="c209a-2002">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2002">Core</span></span>
* <span data-ttu-id="c209a-2003">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="c209a-2003">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="c209a-2004">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="c209a-2004">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2005">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2005">ACS</span></span>

* <span data-ttu-id="c209a-2006">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c209a-2006">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="c209a-2007">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2007">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="c209a-2008">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="c209a-2008">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="c209a-2009">Advisor</span><span class="sxs-lookup"><span data-stu-id="c209a-2009">Advisor</span></span>

* <span data-ttu-id="c209a-2010">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-2010">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2011">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2011">Appservice</span></span>

* <span data-ttu-id="c209a-2012">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="c209a-2012">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="c209a-2013">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="c209a-2013">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="c209a-2014">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="c209a-2014">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="c209a-2015">Consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-2015">Consumption</span></span>

* <span data-ttu-id="c209a-2016">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="c209a-2016">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="c209a-2017">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-2017">Container</span></span>

* <span data-ttu-id="c209a-2018">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-2018">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-2019">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-2019">Monitor</span></span>

* <span data-ttu-id="c209a-2020">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="c209a-2020">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2021">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2021">Resource</span></span>

* <span data-ttu-id="c209a-2022">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2022">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="c209a-2023">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-2023">Role</span></span>

* <span data-ttu-id="c209a-2024">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="c209a-2024">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="c209a-2025">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="c209a-2025">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="c209a-2026">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c209a-2026">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2027">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2027">SQL</span></span>

* <span data-ttu-id="c209a-2028">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="c209a-2028">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="c209a-2029">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2029">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2030">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2030">VM</span></span>

* <span data-ttu-id="c209a-2031">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="c209a-2031">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="c209a-2032">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2032">November 14, 2017</span></span>

<span data-ttu-id="c209a-2033">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="c209a-2033">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-2034">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-2034">ACR</span></span>

* <span data-ttu-id="c209a-2035">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="c209a-2035">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="c209a-2036">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2036">ACS</span></span>

* <span data-ttu-id="c209a-2037">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="c209a-2037">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="c209a-2038">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2038">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="c209a-2039">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="c209a-2039">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="c209a-2040">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-2040">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="c209a-2041">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c209a-2041">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2042">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2042">Appservice</span></span>

* <span data-ttu-id="c209a-2043">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="c209a-2043">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="c209a-2044">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c209a-2044">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="c209a-2045">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c209a-2045">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="c209a-2046">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="c209a-2046">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="c209a-2047">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="c209a-2047">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="c209a-2048">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="c209a-2048">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-2049">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-2049">Batch</span></span>

* <span data-ttu-id="c209a-2050">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="c209a-2050">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-2051">Batchai</span><span class="sxs-lookup"><span data-stu-id="c209a-2051">Batchai</span></span>

* <span data-ttu-id="c209a-2052">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2052">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="c209a-2053">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2053">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="c209a-2054">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="c209a-2054">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="c209a-2055">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2055">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="c209a-2056">Cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-2056">Cloud</span></span>

* <span data-ttu-id="c209a-2057">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="c209a-2057">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="c209a-2058">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-2058">Container</span></span>

* <span data-ttu-id="c209a-2059">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="c209a-2059">Added support to open multiple ports</span></span>
* <span data-ttu-id="c209a-2060">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c209a-2060">Added container group restart policy</span></span>
* <span data-ttu-id="c209a-2061">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="c209a-2061">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="c209a-2062">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="c209a-2062">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c209a-2063">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c209a-2063">Data Lake Analytics</span></span>

* <span data-ttu-id="c209a-2064">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c209a-2064">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c209a-2065">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2065">Data Lake Store</span></span>

* <span data-ttu-id="c209a-2066">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c209a-2066">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-2067">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-2067">Extension</span></span>

* <span data-ttu-id="c209a-2068">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="c209a-2068">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="c209a-2069">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="c209a-2069">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-2070">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-2070">IoT</span></span>

* <span data-ttu-id="c209a-2071">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="c209a-2071">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-2072">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-2072">Monitor</span></span>

* <span data-ttu-id="c209a-2073">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="c209a-2073">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2074">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2074">Network</span></span>

* <span data-ttu-id="c209a-2075">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="c209a-2075">Added support for CAA DNS records</span></span>
* <span data-ttu-id="c209a-2076">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2076">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="c209a-2077">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c209a-2077">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="c209a-2078">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c209a-2078">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="c209a-2079">Réservations</span><span class="sxs-lookup"><span data-stu-id="c209a-2079">Reservations</span></span>

* <span data-ttu-id="c209a-2080">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-2080">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2081">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2081">Resource</span></span>

* <span data-ttu-id="c209a-2082">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c209a-2082">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2083">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2083">SQL</span></span>

* <span data-ttu-id="c209a-2084">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2084">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2085">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2085">Storage</span></span>

* <span data-ttu-id="c209a-2086">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-2086">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="c209a-2087">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="c209a-2087">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="c209a-2088">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="c209a-2088">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="c209a-2089">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="c209a-2089">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="c209a-2090">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2090">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="c209a-2091">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="c209a-2091">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="c209a-2092">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2092">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2093">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2093">VM</span></span>

* <span data-ttu-id="c209a-2094">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="c209a-2094">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="c209a-2095">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="c209a-2095">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="c209a-2096">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="c209a-2096">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="c209a-2097">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="c209a-2097">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="c209a-2098">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c209a-2098">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c209a-2099">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2099">October 24, 2017</span></span>

<span data-ttu-id="c209a-2100">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c209a-2100">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c209a-2101">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2101">Core</span></span>

* <span data-ttu-id="c209a-2102">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c209a-2102">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-2103">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-2103">ACR</span></span>

* <span data-ttu-id="c209a-2104">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c209a-2104">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c209a-2105">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="c209a-2105">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c209a-2106">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="c209a-2106">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2107">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2107">ACS</span></span>

* <span data-ttu-id="c209a-2108">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="c209a-2108">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c209a-2109">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c209a-2109">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2110">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2110">Appservice</span></span>

* <span data-ttu-id="c209a-2111">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="c209a-2111">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c209a-2112">Composant</span><span class="sxs-lookup"><span data-stu-id="c209a-2112">Component</span></span>

* <span data-ttu-id="c209a-2113">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="c209a-2113">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-2114">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-2114">Monitor</span></span>

* <span data-ttu-id="c209a-2115">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="c209a-2115">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2116">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2116">Resource</span></span>

* <span data-ttu-id="c209a-2117">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c209a-2117">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c209a-2118">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="c209a-2118">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2119">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2119">VM</span></span>

* <span data-ttu-id="c209a-2120">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2120">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c209a-2121">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2121">October 9, 2017</span></span>

<span data-ttu-id="c209a-2122">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c209a-2122">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c209a-2123">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2123">Core</span></span>

* <span data-ttu-id="c209a-2124">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c209a-2124">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2125">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2125">Appservice</span></span>

* <span data-ttu-id="c209a-2126">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2126">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-2127">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-2127">Batch</span></span>

* <span data-ttu-id="c209a-2128">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c209a-2128">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c209a-2129">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="c209a-2129">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c209a-2130">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-2130">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c209a-2131">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="c209a-2131">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c209a-2132">Batchai</span><span class="sxs-lookup"><span data-stu-id="c209a-2132">Batchai</span></span>

* <span data-ttu-id="c209a-2133">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="c209a-2133">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-2134">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-2134">Keyvault</span></span>

* <span data-ttu-id="c209a-2135">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c209a-2135">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c209a-2136">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c209a-2136">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c209a-2137">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2137">Network</span></span>

* <span data-ttu-id="c209a-2138">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="c209a-2138">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c209a-2139">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c209a-2139">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2140">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2140">Resource</span></span>

* <span data-ttu-id="c209a-2141">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="c209a-2141">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c209a-2142">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-2142">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c209a-2143">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="c209a-2143">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c209a-2144">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c209a-2144">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2145">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2145">Sql</span></span>

* <span data-ttu-id="c209a-2146">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="c209a-2146">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c209a-2147">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="c209a-2147">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c209a-2148">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="c209a-2148">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2149">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2149">Storage</span></span>

* <span data-ttu-id="c209a-2150">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="c209a-2150">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2151">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2151">Vm</span></span>

* <span data-ttu-id="c209a-2152">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="c209a-2152">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c209a-2153">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2153">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c209a-2154">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c209a-2154">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c209a-2155">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2155">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c209a-2156">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2156">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c209a-2157">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2157">September 22, 2017</span></span>

<span data-ttu-id="c209a-2158">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c209a-2158">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2159">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2159">Resource</span></span>

* <span data-ttu-id="c209a-2160">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="c209a-2160">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c209a-2161">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="c209a-2161">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c209a-2162">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2162">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c209a-2163">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c209a-2163">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2164">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2164">Network</span></span>

* <span data-ttu-id="c209a-2165">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c209a-2165">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c209a-2166">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="c209a-2166">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c209a-2167">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="c209a-2167">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c209a-2168">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2168">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c209a-2169">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2169">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c209a-2170">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2170">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c209a-2171">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2171">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2172">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2172">Storage</span></span>

* <span data-ttu-id="c209a-2173">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c209a-2173">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c209a-2174">Événement</span><span class="sxs-lookup"><span data-stu-id="c209a-2174">Eventgrid</span></span>

* <span data-ttu-id="c209a-2175">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="c209a-2175">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2176">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2176">SQL</span></span>

* <span data-ttu-id="c209a-2177">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="c209a-2177">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c209a-2178">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="c209a-2178">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c209a-2179">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2179">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-2180">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-2180">Keyvault</span></span>

* <span data-ttu-id="c209a-2181">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="c209a-2181">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2182">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2182">VM</span></span>

* <span data-ttu-id="c209a-2183">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2183">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c209a-2184">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="c209a-2184">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c209a-2185">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2185">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c209a-2186">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c209a-2186">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c209a-2187">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c209a-2187">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c209a-2188">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c209a-2188">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2189">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2189">ACS</span></span>

* <span data-ttu-id="c209a-2190">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-2190">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2191">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2191">Appservice</span></span>

* <span data-ttu-id="c209a-2192">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2192">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c209a-2193">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c209a-2193">Backup</span></span>

* <span data-ttu-id="c209a-2194">Préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-2194">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c209a-2195">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2195">September 11, 2017</span></span>

<span data-ttu-id="c209a-2196">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c209a-2196">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c209a-2197">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2197">Core</span></span>

* <span data-ttu-id="c209a-2198">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="c209a-2198">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c209a-2199">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="c209a-2199">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2200">Acs</span><span class="sxs-lookup"><span data-stu-id="c209a-2200">Acs</span></span>

* <span data-ttu-id="c209a-2201">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c209a-2201">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c209a-2202">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="c209a-2202">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2203">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2203">Appservice</span></span>

* <span data-ttu-id="c209a-2204">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="c209a-2204">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-2205">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-2205">CDN</span></span>

* <span data-ttu-id="c209a-2206">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2206">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="c209a-2207">Extension</span><span class="sxs-lookup"><span data-stu-id="c209a-2207">Extension</span></span>

* <span data-ttu-id="c209a-2208">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-2208">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-2209">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-2209">Keyvault</span></span>

* <span data-ttu-id="c209a-2210">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="c209a-2210">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2211">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2211">Network</span></span>

* <span data-ttu-id="c209a-2212">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c209a-2212">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c209a-2213">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2213">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c209a-2214">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2214">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c209a-2215">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2215">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c209a-2216">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2216">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2217">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2217">Resource</span></span>

* <span data-ttu-id="c209a-2218">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2218">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c209a-2219">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2219">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c209a-2220">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="c209a-2220">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c209a-2221">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="c209a-2221">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2222">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2222">SQL</span></span>

* <span data-ttu-id="c209a-2223">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-2223">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2224">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2224">VM</span></span>

* <span data-ttu-id="c209a-2225">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="c209a-2225">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c209a-2226">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="c209a-2226">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c209a-2227">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2227">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c209a-2228">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="c209a-2228">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c209a-2229">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="c209a-2229">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c209a-2230">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2230">August 31, 2017</span></span>

<span data-ttu-id="c209a-2231">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c209a-2231">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-2232">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-2232">Keyvault</span></span>

* <span data-ttu-id="c209a-2233">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="c209a-2233">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c209a-2234">Sf</span><span class="sxs-lookup"><span data-stu-id="c209a-2234">Sf</span></span>

* <span data-ttu-id="c209a-2235">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c209a-2235">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2236">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2236">Storage</span></span>

* <span data-ttu-id="c209a-2237">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="c209a-2237">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c209a-2238">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="c209a-2238">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c209a-2239">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2239">August 28, 2017</span></span>

<span data-ttu-id="c209a-2240">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c209a-2240">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c209a-2241">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c209a-2241">CLI</span></span>

* <span data-ttu-id="c209a-2242">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="c209a-2242">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2243">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2243">ACS</span></span>

* <span data-ttu-id="c209a-2244">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c209a-2244">Corrected preview regions</span></span>
* <span data-ttu-id="c209a-2245">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-2245">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="c209a-2246">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2246">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2247">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2247">Appservice</span></span>

* <span data-ttu-id="c209a-2248">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2248">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c209a-2249">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-2249">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c209a-2250">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2250">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c209a-2251">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="c209a-2251">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c209a-2252">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-2252">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-2253">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-2253">IoT</span></span>

* <span data-ttu-id="c209a-2254">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="c209a-2254">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2255">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2255">Network</span></span>

* <span data-ttu-id="c209a-2256">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c209a-2256">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c209a-2257">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2257">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c209a-2258">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c209a-2258">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c209a-2259">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2259">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c209a-2260">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2260">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-2261">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-2261">Profile</span></span>

* <span data-ttu-id="c209a-2262">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2262">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c209a-2263">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c209a-2263">Service Fabric</span></span>

* <span data-ttu-id="c209a-2264">Préversion</span><span class="sxs-lookup"><span data-stu-id="c209a-2264">Preview release</span></span>
* <span data-ttu-id="c209a-2265">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="c209a-2265">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c209a-2266">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="c209a-2266">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c209a-2267">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="c209a-2267">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2268">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2268">Storage</span></span>

* <span data-ttu-id="c209a-2269">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="c209a-2269">Enabled setting blob tier</span></span>
* <span data-ttu-id="c209a-2270">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="c209a-2270">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c209a-2271">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c209a-2271">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="c209a-2272">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="c209a-2272">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c209a-2273">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2273">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c209a-2274">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="c209a-2274">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2275">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2275">VM</span></span>

* <span data-ttu-id="c209a-2276">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c209a-2276">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c209a-2277">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c209a-2277">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="c209a-2278">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2278">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="c209a-2279">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="c209a-2279">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c209a-2280">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="c209a-2280">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c209a-2281">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2281">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c209a-2282">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2282">August 15, 2017</span></span>

<span data-ttu-id="c209a-2283">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c209a-2283">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2284">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2284">ACS</span></span>

* <span data-ttu-id="c209a-2285">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="c209a-2285">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2286">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2286">Appservice</span></span>

* <span data-ttu-id="c209a-2287">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="c209a-2287">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c209a-2288">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c209a-2288">Event Grid</span></span>

* <span data-ttu-id="c209a-2289">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c209a-2289">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c209a-2290">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2290">August 11, 2017</span></span>

<span data-ttu-id="c209a-2291">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c209a-2291">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2292">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2292">ACS</span></span>

* <span data-ttu-id="c209a-2293">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c209a-2293">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-2294">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-2294">Batch</span></span>

* <span data-ttu-id="c209a-2295">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c209a-2295">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c209a-2296">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="c209a-2296">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c209a-2297">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="c209a-2297">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c209a-2298">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="c209a-2298">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c209a-2299">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="c209a-2299">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c209a-2300">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="c209a-2300">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c209a-2301">Composant</span><span class="sxs-lookup"><span data-stu-id="c209a-2301">Component</span></span>

* <span data-ttu-id="c209a-2302">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="c209a-2302">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c209a-2303">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-2303">Container</span></span>

* <span data-ttu-id="c209a-2304">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="c209a-2304">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c209a-2305">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2305">Data Lake Store</span></span>

* <span data-ttu-id="c209a-2306">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="c209a-2306">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c209a-2307">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c209a-2307">Event Grid</span></span>

* <span data-ttu-id="c209a-2308">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c209a-2308">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2309">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2309">Network</span></span>

* <span data-ttu-id="c209a-2310">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="c209a-2310">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c209a-2311">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c209a-2311">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c209a-2312">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="c209a-2312">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c209a-2313">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c209a-2313">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-2314">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-2314">Profile</span></span>

* <span data-ttu-id="c209a-2315">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="c209a-2315">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2316">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2316">Storage</span></span>

* <span data-ttu-id="c209a-2317">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c209a-2317">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2318">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2318">VM</span></span>

* <span data-ttu-id="c209a-2319">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="c209a-2319">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c209a-2320">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="c209a-2320">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c209a-2321">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="c209a-2321">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c209a-2322">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="c209a-2322">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c209a-2323">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="c209a-2323">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c209a-2324">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2324">July 28, 2017</span></span>

<span data-ttu-id="c209a-2325">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c209a-2325">Version 2.0.12</span></span>

* <span data-ttu-id="c209a-2326">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="c209a-2326">Added container commands</span></span>
* <span data-ttu-id="c209a-2327">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="c209a-2327">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c209a-2328">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2328">Core</span></span>

* <span data-ttu-id="c209a-2329">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="c209a-2329">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c209a-2330">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="c209a-2330">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c209a-2331">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c209a-2331">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c209a-2332">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c209a-2332">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c209a-2333">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="c209a-2333">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c209a-2334">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="c209a-2334">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c209a-2335">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="c209a-2335">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c209a-2336">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c209a-2336">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c209a-2337">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="c209a-2337">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c209a-2338">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c209a-2338">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c209a-2339">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="c209a-2339">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c209a-2340">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="c209a-2340">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c209a-2341">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-2341">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c209a-2342">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c209a-2342">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c209a-2343">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c209a-2343">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c209a-2344">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c209a-2344">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c209a-2345">ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-2345">ACR</span></span>

* <span data-ttu-id="c209a-2346">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c209a-2346">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c209a-2347">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c209a-2347">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c209a-2348">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="c209a-2348">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c209a-2349">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="c209a-2349">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c209a-2350">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="c209a-2350">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c209a-2351">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="c209a-2351">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2352">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2352">ACS</span></span>

* <span data-ttu-id="c209a-2353">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c209a-2353">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2354">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2354">Appservice</span></span>

* <span data-ttu-id="c209a-2355">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="c209a-2355">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c209a-2356">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="c209a-2356">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c209a-2357">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c209a-2357">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c209a-2358">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="c209a-2358">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c209a-2359">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="c209a-2359">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c209a-2360">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c209a-2360">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c209a-2361">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="c209a-2361">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c209a-2362">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="c209a-2362">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c209a-2363">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="c209a-2363">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c209a-2364">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c209a-2364">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c209a-2365">Batch</span><span class="sxs-lookup"><span data-stu-id="c209a-2365">Batch</span></span>

* <span data-ttu-id="c209a-2366">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="c209a-2366">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c209a-2367">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c209a-2367">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c209a-2368">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c209a-2368">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c209a-2369">CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-2369">CDN</span></span>

* <span data-ttu-id="c209a-2370">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c209a-2370">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="c209a-2371">Cloud</span><span class="sxs-lookup"><span data-stu-id="c209a-2371">Cloud</span></span>

* <span data-ttu-id="c209a-2372">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="c209a-2372">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c209a-2373">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c209a-2373">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c209a-2374">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="c209a-2374">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c209a-2375">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="c209a-2375">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c209a-2376">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c209a-2376">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-2377">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-2377">CosmosDB</span></span>

* <span data-ttu-id="c209a-2378">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="c209a-2378">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c209a-2379">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="c209a-2379">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c209a-2380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c209a-2380">Data Lake Analytics</span></span>

* <span data-ttu-id="c209a-2381">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c209a-2381">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c209a-2382">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2382">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c209a-2383">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c209a-2383">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c209a-2384">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2384">Data Lake Store</span></span>

* <span data-ttu-id="c209a-2385">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2385">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c209a-2386">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="c209a-2386">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c209a-2387">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c209a-2387">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c209a-2388">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2388">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c209a-2389">Interactive</span><span class="sxs-lookup"><span data-stu-id="c209a-2389">Interactive</span></span>

* <span data-ttu-id="c209a-2390">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="c209a-2390">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c209a-2391">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="c209a-2391">Increased test coverage</span></span>
* <span data-ttu-id="c209a-2392">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="c209a-2392">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c209a-2393">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c209a-2393">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c209a-2394">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="c209a-2394">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c209a-2395">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="c209a-2395">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c209a-2396">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="c209a-2396">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c209a-2397">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="c209a-2397">Added `--progress` flag</span></span>
* <span data-ttu-id="c209a-2398">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="c209a-2398">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c209a-2399">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="c209a-2399">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c209a-2400">IoT</span><span class="sxs-lookup"><span data-stu-id="c209a-2400">IoT</span></span>

* <span data-ttu-id="c209a-2401">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="c209a-2401">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c209a-2402">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c209a-2402">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c209a-2403">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c209a-2403">Key vault</span></span>

* <span data-ttu-id="c209a-2404">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="c209a-2404">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c209a-2405">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c209a-2405">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c209a-2406">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c209a-2406">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c209a-2407">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c209a-2407">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c209a-2408">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c209a-2408">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c209a-2409">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="c209a-2409">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c209a-2410">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c209a-2410">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c209a-2411">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c209a-2411">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c209a-2412">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2412">Lab</span></span>

* <span data-ttu-id="c209a-2413">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c209a-2413">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c209a-2414">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2414">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-2415">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-2415">Monitor</span></span>

* <span data-ttu-id="c209a-2416">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="c209a-2416">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c209a-2417">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c209a-2417">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c209a-2418">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c209a-2418">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c209a-2419">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c209a-2419">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c209a-2420">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c209a-2420">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c209a-2421">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c209a-2421">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c209a-2422">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="c209a-2422">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c209a-2423">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="c209a-2423">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c209a-2424">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c209a-2424">`location` no longer required</span></span>
  * <span data-ttu-id="c209a-2425">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="c209a-2425">Add name and ID support for target</span></span>
  * <span data-ttu-id="c209a-2426">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-2426">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c209a-2427">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c209a-2427">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c209a-2428">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="c209a-2428">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c209a-2429">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="c209a-2429">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c209a-2430">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c209a-2430">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c209a-2431">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2431">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2432">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2432">Network</span></span>

* <span data-ttu-id="c209a-2433">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c209a-2433">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c209a-2434">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2434">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c209a-2435">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="c209a-2435">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c209a-2436">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="c209a-2436">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c209a-2437">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2437">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c209a-2438">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c209a-2438">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c209a-2439">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2439">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c209a-2440">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c209a-2440">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c209a-2441">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c209a-2441">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c209a-2442">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c209a-2442">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c209a-2443">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2443">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c209a-2444">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c209a-2444">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c209a-2445">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c209a-2445">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c209a-2446">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2446">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c209a-2447">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2447">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c209a-2448">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2448">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c209a-2449">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="c209a-2449">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c209a-2450">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c209a-2450">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c209a-2451">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2451">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c209a-2452">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2452">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c209a-2453">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2453">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c209a-2454">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-2454">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c209a-2455">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c209a-2455">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c209a-2456">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c209a-2456">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c209a-2457">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c209a-2457">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c209a-2458">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c209a-2458">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c209a-2459">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c209a-2459">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-2460">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-2460">Profile</span></span>

* <span data-ttu-id="c209a-2461">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="c209a-2461">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c209a-2462">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c209a-2462">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c209a-2463">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="c209a-2463">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c209a-2464">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="c209a-2464">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c209a-2465">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="c209a-2465">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c209a-2466">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c209a-2466">RDBMS</span></span>

* <span data-ttu-id="c209a-2467">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="c209a-2467">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c209a-2468">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c209a-2468">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c209a-2469">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="c209a-2469">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c209a-2470">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c209a-2470">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2471">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2471">Resource</span></span>

* <span data-ttu-id="c209a-2472">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2472">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c209a-2473">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c209a-2473">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c209a-2474">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c209a-2474">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c209a-2475">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="c209a-2475">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c209a-2476">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="c209a-2476">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c209a-2477">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c209a-2477">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c209a-2478">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="c209a-2478">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c209a-2479">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c209a-2479">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c209a-2480">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-2480">Role</span></span>

* <span data-ttu-id="c209a-2481">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c209a-2481">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c209a-2482">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="c209a-2482">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c209a-2483">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="c209a-2483">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c209a-2484">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c209a-2484">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c209a-2485">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c209a-2485">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c209a-2486">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c209a-2486">Service Fabric</span></span>
* <span data-ttu-id="c209a-2487">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="c209a-2487">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c209a-2488">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c209a-2488">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c209a-2489">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c209a-2489">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2490">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2490">SQL</span></span>

* <span data-ttu-id="c209a-2491">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="c209a-2491">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c209a-2492">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c209a-2492">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c209a-2493">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c209a-2493">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2494">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2494">Storage</span></span>

* <span data-ttu-id="c209a-2495">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c209a-2495">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c209a-2496">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="c209a-2496">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c209a-2497">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="c209a-2497">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c209a-2498">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c209a-2498">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="c209a-2499">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="c209a-2499">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="c209a-2500">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c209a-2500">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2501">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2501">VM</span></span>

* <span data-ttu-id="c209a-2502">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2502">Support configuring nsg</span></span>
* <span data-ttu-id="c209a-2503">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="c209a-2503">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c209a-2504">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="c209a-2504">Support managed service identities</span></span>
* <span data-ttu-id="c209a-2505">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="c209a-2505">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="c209a-2506">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="c209a-2506">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c209a-2507">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2507">May 10, 2017</span></span>

<span data-ttu-id="c209a-2508">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c209a-2508">Version 2.0.6</span></span>

* <span data-ttu-id="c209a-2509">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c209a-2509">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c209a-2510">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c209a-2510">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c209a-2511">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2511">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="c209a-2512">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c209a-2512">Include Cognitive Services module</span></span>
* <span data-ttu-id="c209a-2513">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c209a-2513">Include Service Fabric module</span></span>
* <span data-ttu-id="c209a-2514">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="c209a-2514">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="c209a-2515">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="c209a-2515">Add support for CDN commands</span></span>
* <span data-ttu-id="c209a-2516">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="c209a-2516">Remove Container module</span></span>
* <span data-ttu-id="c209a-2517">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c209a-2517">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c209a-2518">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c209a-2518">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c209a-2519">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2519">Core</span></span>

* <span data-ttu-id="c209a-2520">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="c209a-2520">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="c209a-2521">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c209a-2521">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c209a-2522">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c209a-2522">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c209a-2523">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c209a-2523">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c209a-2524">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c209a-2524">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c209a-2525">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c209a-2525">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c209a-2526">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c209a-2526">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c209a-2527">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c209a-2527">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c209a-2528">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c209a-2528">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c209a-2529">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="c209a-2529">core: Improved performance</span></span>
* <span data-ttu-id="c209a-2530">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c209a-2530">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c209a-2531">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="c209a-2531">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2532">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2532">ACS</span></span>

* <span data-ttu-id="c209a-2533">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c209a-2533">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c209a-2534">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="c209a-2534">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c209a-2535">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="c209a-2535">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c209a-2536">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c209a-2536">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2537">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2537">AppService</span></span>

* <span data-ttu-id="c209a-2538">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c209a-2538">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c209a-2539">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="c209a-2539">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c209a-2540">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="c209a-2540">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c209a-2541">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="c209a-2541">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c209a-2542">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="c209a-2542">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c209a-2543">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c209a-2543">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c209a-2544">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="c209a-2544">support slot swap with preview</span></span>
* <span data-ttu-id="c209a-2545">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c209a-2545">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c209a-2546">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c209a-2546">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c209a-2547">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c209a-2547">CosmosDB</span></span>

* <span data-ttu-id="c209a-2548">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c209a-2548">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="c209a-2549">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="c209a-2549">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c209a-2550">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="c209a-2550">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c209a-2551">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c209a-2551">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c209a-2552">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c209a-2552">Data Lake Analytics</span></span>

* <span data-ttu-id="c209a-2553">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="c209a-2553">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="c209a-2554">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="c209a-2554">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c209a-2555">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c209a-2555">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c209a-2556">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="c209a-2556">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c209a-2557">Table</span><span class="sxs-lookup"><span data-stu-id="c209a-2557">Table</span></span>
  * <span data-ttu-id="c209a-2558">Fonction table</span><span class="sxs-lookup"><span data-stu-id="c209a-2558">Table valued function</span></span>
  * <span data-ttu-id="c209a-2559">Affichage</span><span class="sxs-lookup"><span data-stu-id="c209a-2559">View</span></span>
  * <span data-ttu-id="c209a-2560">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="c209a-2560">Table Statistics.</span></span> <span data-ttu-id="c209a-2561">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="c209a-2561">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c209a-2562">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2562">Data Lake Store</span></span>

* <span data-ttu-id="c209a-2563">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="c209a-2563">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="c209a-2564">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c209a-2564">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c209a-2565">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="c209a-2565">missed help for access show.</span></span> <span data-ttu-id="c209a-2566">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="c209a-2566">adding it.</span></span> <span data-ttu-id="c209a-2567">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c209a-2567">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c209a-2568">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c209a-2568">Find</span></span>

* <span data-ttu-id="c209a-2569">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="c209a-2569">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c209a-2570">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c209a-2570">KeyVault</span></span>

* <span data-ttu-id="c209a-2571">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="c209a-2571">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c209a-2572">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c209a-2572">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="c209a-2573">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="c209a-2573">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c209a-2574">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="c209a-2574">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="c209a-2575">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c209a-2575">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c209a-2576">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2576">Lab</span></span>

* <span data-ttu-id="c209a-2577">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2577">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="c209a-2578">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2578">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="c209a-2579">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2579">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="c209a-2580">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2580">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="c209a-2581">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="c209a-2581">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="c209a-2582">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c209a-2582">Monitor</span></span>

* <span data-ttu-id="c209a-2583">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c209a-2583">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c209a-2584">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c209a-2584">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c209a-2585">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2585">Network</span></span>

* <span data-ttu-id="c209a-2586">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="c209a-2586">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="c209a-2587">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2587">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="c209a-2588">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c209a-2588">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="c209a-2589">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c209a-2589">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="c209a-2590">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="c209a-2590">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="c209a-2591">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c209a-2591">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="c209a-2592">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c209a-2592">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="c209a-2593">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c209a-2593">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="c209a-2594">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="c209a-2594">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="c209a-2595">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="c209a-2595">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c209a-2596">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="c209a-2596">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="c209a-2597">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2597">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="c209a-2598">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-2598">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="c209a-2599">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="c209a-2599">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="c209a-2600">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c209a-2600">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="c209a-2601">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="c209a-2601">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="c209a-2602">Profil</span><span class="sxs-lookup"><span data-stu-id="c209a-2602">Profile</span></span>

* <span data-ttu-id="c209a-2603">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c209a-2603">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c209a-2604">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c209a-2604">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c209a-2605">Redis</span><span class="sxs-lookup"><span data-stu-id="c209a-2605">Redis</span></span>

* <span data-ttu-id="c209a-2606">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="c209a-2606">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c209a-2607">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="c209a-2607">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="c209a-2608">Ressource</span><span class="sxs-lookup"><span data-stu-id="c209a-2608">Resource</span></span>

* <span data-ttu-id="c209a-2609">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c209a-2609">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c209a-2610">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c209a-2610">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c209a-2611">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c209a-2611">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c209a-2612">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="c209a-2612">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c209a-2613">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c209a-2613">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c209a-2614">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="c209a-2614">Add docs for az lock update.</span></span> <span data-ttu-id="c209a-2615">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c209a-2615">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c209a-2616">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c209a-2616">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c209a-2617">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c209a-2617">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c209a-2618">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c209a-2618">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c209a-2619">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c209a-2619">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c209a-2620">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c209a-2620">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c209a-2621">Role</span><span class="sxs-lookup"><span data-stu-id="c209a-2621">Role</span></span>

* <span data-ttu-id="c209a-2622">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c209a-2622">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c209a-2623">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c209a-2623">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c209a-2624">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c209a-2624">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c209a-2625">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="c209a-2625">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c209a-2626">SQL</span><span class="sxs-lookup"><span data-stu-id="c209a-2626">SQL</span></span>

* <span data-ttu-id="c209a-2627">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="c209a-2627">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="c209a-2628">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c209a-2628">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c209a-2629">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2629">Storage</span></span>

* <span data-ttu-id="c209a-2630">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="c209a-2630">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="c209a-2631">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c209a-2631">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c209a-2632">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="c209a-2632">Add support for large block blob upload</span></span>
* <span data-ttu-id="c209a-2633">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="c209a-2633">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2634">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2634">VM</span></span>

* <span data-ttu-id="c209a-2635">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="c209a-2635">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c209a-2636">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="c209a-2636">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c209a-2637">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c209a-2637">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c209a-2638">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c209a-2638">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c209a-2639">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="c209a-2639">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c209a-2640">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="c209a-2640">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c209a-2641">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c209a-2641">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c209a-2642">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2642">April 3, 2017</span></span>

<span data-ttu-id="c209a-2643">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c209a-2643">Version 2.0.2</span></span>

<span data-ttu-id="c209a-2644">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="c209a-2644">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="c209a-2645">Core</span><span class="sxs-lookup"><span data-stu-id="c209a-2645">Core</span></span>

* <span data-ttu-id="c209a-2646">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-2646">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="c209a-2647">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c209a-2647">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c209a-2648">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c209a-2648">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c209a-2649">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c209a-2649">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c209a-2650">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c209a-2650">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c209a-2651">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="c209a-2651">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c209a-2652">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c209a-2652">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c209a-2653">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="c209a-2653">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c209a-2654">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="c209a-2654">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="c209a-2655">ACS</span><span class="sxs-lookup"><span data-stu-id="c209a-2655">ACS</span></span>

* <span data-ttu-id="c209a-2656">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c209a-2656">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c209a-2657">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="c209a-2657">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c209a-2658">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c209a-2658">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c209a-2659">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="c209a-2659">Add support for windows clusters.</span></span> <span data-ttu-id="c209a-2660">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c209a-2660">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c209a-2661">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="c209a-2661">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c209a-2662">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c209a-2662">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="c209a-2663">AppService</span><span class="sxs-lookup"><span data-stu-id="c209a-2663">AppService</span></span>

* <span data-ttu-id="c209a-2664">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c209a-2664">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c209a-2665">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c209a-2665">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c209a-2666">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c209a-2666">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c209a-2667">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c209a-2667">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="c209a-2668">DataLake</span><span class="sxs-lookup"><span data-stu-id="c209a-2668">DataLake</span></span>

* <span data-ttu-id="c209a-2669">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c209a-2669">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="c209a-2670">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c209a-2670">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="c209a-2671">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c209a-2671">DocuemntDB</span></span>

* <span data-ttu-id="c209a-2672">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c209a-2672">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c209a-2673">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c209a-2673">VM</span></span>

* <span data-ttu-id="c209a-2674">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c209a-2674">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c209a-2675">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c209a-2675">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c209a-2676">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c209a-2676">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c209a-2677">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c209a-2677">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c209a-2678">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c209a-2678">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c209a-2679">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="c209a-2679">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="c209a-2680">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c209a-2680">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c209a-2681">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="c209a-2681">February 27, 2017</span></span>

<span data-ttu-id="c209a-2682">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c209a-2682">Version 2.0.0</span></span>

<span data-ttu-id="c209a-2683">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="c209a-2683">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="c209a-2684">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c209a-2684">Container Service (acs)</span></span>
- <span data-ttu-id="c209a-2685">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="c209a-2685">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c209a-2686">Réseau</span><span class="sxs-lookup"><span data-stu-id="c209a-2686">Networking</span></span>
- <span data-ttu-id="c209a-2687">Stockage</span><span class="sxs-lookup"><span data-stu-id="c209a-2687">Storage</span></span>

<span data-ttu-id="c209a-2688">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c209a-2688">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="c209a-2689">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c209a-2689">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="c209a-2690">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="c209a-2690">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="c209a-2691">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="c209a-2691">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="c209a-2692">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c209a-2692">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="c209a-2693">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="c209a-2693">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c209a-2694">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c209a-2694">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c209a-2695">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c209a-2695">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="c209a-2696">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c209a-2696">Provide feedback from the command line with the `az feedback` command</span></span>

