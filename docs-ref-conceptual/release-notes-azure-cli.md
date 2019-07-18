---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/16/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8cb0e2f43a3f40fdf15a00ebc7bdb931bf8f41f0
ms.sourcegitcommit: 49e1dea60942fce02d9c3ce249ac633a83f303e7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2019
ms.locfileid: "68246918"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="9b557-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9b557-103">Azure CLI release notes</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="9b557-104">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-104">July 16, 2019</span></span>

<span data-ttu-id="9b557-105">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="9b557-105">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-106">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-106">Appservice</span></span>

* <span data-ttu-id="9b557-107">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="9b557-107">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="9b557-108">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="9b557-108">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="9b557-109">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="9b557-109">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="9b557-110">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-110">Core</span></span>

* <span data-ttu-id="9b557-111">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="9b557-111">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-112">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-112">Batch</span></span>

* <span data-ttu-id="9b557-113">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="9b557-113">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="9b557-114">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="9b557-114">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="9b557-115">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="9b557-115">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="9b557-116">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-116">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9b557-117">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9b557-117">Eventhubs</span></span>

* <span data-ttu-id="9b557-118">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="9b557-118">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-119">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-119">RDBMS</span></span>

* <span data-ttu-id="9b557-120">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="9b557-120">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="9b557-121">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="9b557-121">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="9b557-122">Relais</span><span class="sxs-lookup"><span data-stu-id="9b557-122">Relay</span></span>

* <span data-ttu-id="9b557-123">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="9b557-123">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="9b557-124">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="9b557-124">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9b557-125">Servicebus</span><span class="sxs-lookup"><span data-stu-id="9b557-125">Servicebus</span></span>

* <span data-ttu-id="9b557-126">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="9b557-126">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-127">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-127">Storage</span></span>

* <span data-ttu-id="9b557-128">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-128">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="9b557-129">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="9b557-129">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="9b557-130">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-130">July 2, 2019</span></span>

<span data-ttu-id="9b557-131">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="9b557-131">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="9b557-132">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-132">Core</span></span>

* <span data-ttu-id="9b557-133">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="9b557-133">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="9b557-134">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="9b557-134">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="9b557-135">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="9b557-135">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-136">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-136">ACR</span></span>

* <span data-ttu-id="9b557-137">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="9b557-137">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-138">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-138">Appservice</span></span>

* <span data-ttu-id="9b557-139">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-139">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="9b557-140">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="9b557-140">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="9b557-141">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="9b557-141">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="9b557-142">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="9b557-142">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9b557-143">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9b557-143">Cosmos DB</span></span>

* <span data-ttu-id="9b557-144">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="9b557-144">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="9b557-145">DLS</span><span class="sxs-lookup"><span data-stu-id="9b557-145">DLS</span></span>

* <span data-ttu-id="9b557-146">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="9b557-146">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="9b557-147">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9b557-147">Feedback</span></span>

* <span data-ttu-id="9b557-148">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="9b557-148">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-149">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-149">HDInsight</span></span>

* <span data-ttu-id="9b557-150">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="9b557-150">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="9b557-151">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="9b557-151">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="9b557-152">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="9b557-152">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="9b557-153">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="9b557-153">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="9b557-154">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="9b557-154">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="9b557-155">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-155">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="9b557-156">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="9b557-156">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="9b557-157">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="9b557-157">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="9b557-158">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="9b557-158">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="9b557-159">Services gérés</span><span class="sxs-lookup"><span data-stu-id="9b557-159">Managed Services</span></span>

* <span data-ttu-id="9b557-160">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-160">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-161">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-161">Profile</span></span>
* <span data-ttu-id="9b557-162">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="9b557-162">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="9b557-163">RBAC</span><span class="sxs-lookup"><span data-stu-id="9b557-163">RBAC</span></span>

* <span data-ttu-id="9b557-164">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9b557-164">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="9b557-165">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="9b557-165">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="9b557-166">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="9b557-166">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="9b557-167">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="9b557-167">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-168">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-168">RDBMS</span></span>

* <span data-ttu-id="9b557-169">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="9b557-169">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-170">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-170">SQL</span></span>

* <span data-ttu-id="9b557-171">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-171">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-172">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-172">Storage</span></span>

* <span data-ttu-id="9b557-173">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9b557-173">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="9b557-174">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9b557-174">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="9b557-175">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-175">VM</span></span>

* <span data-ttu-id="9b557-176">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-176">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="9b557-177">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="9b557-177">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="9b557-178">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="9b557-178">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="9b557-179">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="9b557-179">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="9b557-180">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-180">June 18, 2019</span></span>

<span data-ttu-id="9b557-181">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="9b557-181">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="9b557-182">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-182">Core</span></span>

<span data-ttu-id="9b557-183">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="9b557-183">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="9b557-184">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="9b557-184">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="9b557-185">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="9b557-185">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="9b557-186">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="9b557-186">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="9b557-187">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="9b557-187">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="9b557-188">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="9b557-188">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="9b557-189">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="9b557-189">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-190">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-190">ACR</span></span>
* <span data-ttu-id="9b557-191">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="9b557-191">Added 'acr check-health' command</span></span>
* <span data-ttu-id="9b557-192">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="9b557-192">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-193">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-193">ACS</span></span>
* <span data-ttu-id="9b557-194">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="9b557-194">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-195">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-195">AMS</span></span>
* <span data-ttu-id="9b557-196">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="9b557-196">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-197">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-197">AppService</span></span>
* <span data-ttu-id="9b557-198">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="9b557-198">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="9b557-199">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9b557-199">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="9b557-200">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="9b557-200">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="9b557-201">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-201">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="9b557-202">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="9b557-202">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="9b557-203">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="9b557-203">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-204">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-204">Batch</span></span>
* <span data-ttu-id="9b557-205">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="9b557-205">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-206">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-206">BatchAI</span></span>
* <span data-ttu-id="9b557-207">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="9b557-207">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-208">BotService</span><span class="sxs-lookup"><span data-stu-id="9b557-208">BotService</span></span>
* <span data-ttu-id="9b557-209">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="9b557-209">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-210">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-210">CosmosDB</span></span>
* <span data-ttu-id="9b557-211">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="9b557-211">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="9b557-212">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="9b557-212">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="9b557-213">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="9b557-213">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="9b557-214">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="9b557-214">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9b557-215">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9b557-215">EventGrid</span></span>
* <span data-ttu-id="9b557-216">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="9b557-216">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="9b557-217">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="9b557-217">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="9b557-218">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="9b557-218">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="9b557-219">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="9b557-219">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="9b557-220">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-220">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-221">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-221">HDInsight</span></span>
* <span data-ttu-id="9b557-222">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9b557-222">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-223">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-223">IoT</span></span>
* <span data-ttu-id="9b557-224">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="9b557-224">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="9b557-225">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="9b557-225">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="9b557-226">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-226">Network</span></span>
* <span data-ttu-id="9b557-227">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="9b557-227">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="9b557-228">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="9b557-228">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="9b557-229">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="9b557-229">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="9b557-230">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="9b557-230">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-231">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-231">Resource</span></span>
* <span data-ttu-id="9b557-232">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="9b557-232">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="9b557-233">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="9b557-233">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9b557-234">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9b557-234">ServiceBus</span></span>
* <span data-ttu-id="9b557-235">Correction d’une erreur liée à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="9b557-235">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-236">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-236">SQL</span></span>
* <span data-ttu-id="9b557-237">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="9b557-237">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="9b557-238">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="9b557-238">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="9b557-239">SQLVm</span><span class="sxs-lookup"><span data-stu-id="9b557-239">SQLVm</span></span>
* <span data-ttu-id="9b557-240">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="9b557-240">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="9b557-241">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-241">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-242">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-242">Storage</span></span>
* <span data-ttu-id="9b557-243">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9b557-243">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="9b557-244">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-244">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-245">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-245">VM</span></span>
* <span data-ttu-id="9b557-246">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-246">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="9b557-247">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-247">June 4, 2019</span></span>

<span data-ttu-id="9b557-248">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="9b557-248">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="9b557-249">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-249">Core</span></span>
* <span data-ttu-id="9b557-250">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="9b557-250">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-251">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-251">ACR</span></span>
* <span data-ttu-id="9b557-252">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="9b557-252">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-253">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-253">ACS</span></span>
* <span data-ttu-id="9b557-254">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-254">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="9b557-255">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="9b557-255">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-256">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-256">Batch</span></span>
* <span data-ttu-id="9b557-257">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="9b557-257">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-258">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-258">IoT</span></span>
* <span data-ttu-id="9b557-259">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="9b557-259">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="9b557-260">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-260">Network</span></span>
* <span data-ttu-id="9b557-261">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="9b557-261">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="9b557-262">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-262">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="9b557-263">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-263">Resource</span></span>
* <span data-ttu-id="9b557-264">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="9b557-264">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="9b557-265">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-265">Role</span></span>
* <span data-ttu-id="9b557-266">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="9b557-266">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="9b557-267">Calcul</span><span class="sxs-lookup"><span data-stu-id="9b557-267">Compute</span></span>
* <span data-ttu-id="9b557-268">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="9b557-268">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="9b557-269">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-269">May 21, 2019</span></span>

<span data-ttu-id="9b557-270">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="9b557-270">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="9b557-271">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-271">Core</span></span>
* <span data-ttu-id="9b557-272">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="9b557-272">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="9b557-273">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="9b557-273">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="9b557-274">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="9b557-274">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-275">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-275">ACR</span></span>
* <span data-ttu-id="9b557-276">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="9b557-276">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-277">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-277">ACS</span></span>
* <span data-ttu-id="9b557-278">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="9b557-278">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-279">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-279">AppService</span></span>
* <span data-ttu-id="9b557-280">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="9b557-280">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="9b557-281">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="9b557-281">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="9b557-282">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="9b557-282">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="9b557-283">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="9b557-283">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="9b557-284">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9b557-284">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="9b557-285">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="9b557-285">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="9b557-286">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9b557-286">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-287">BotService</span><span class="sxs-lookup"><span data-stu-id="9b557-287">BotService</span></span>
* <span data-ttu-id="9b557-288">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-288">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="9b557-289">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-289">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-290">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-290">Consumption</span></span>
* <span data-ttu-id="9b557-291">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-291">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-292">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-292">IoT</span></span>
* <span data-ttu-id="9b557-293">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="9b557-293">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="9b557-294">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-294">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="9b557-296">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="9b557-296">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="9b557-297">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="9b557-297">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-298">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-298">RDBMS</span></span>
* <span data-ttu-id="9b557-299">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="9b557-299">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="9b557-300">RBAC</span><span class="sxs-lookup"><span data-stu-id="9b557-300">RBAC</span></span>
* <span data-ttu-id="9b557-301">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="9b557-301">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-302">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-302">Storage</span></span>
* <span data-ttu-id="9b557-303">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-303">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="9b557-304">Calcul</span><span class="sxs-lookup"><span data-stu-id="9b557-304">Compute</span></span>
* <span data-ttu-id="9b557-305">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-305">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="9b557-306">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="9b557-306">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="9b557-307">__Remarque__: il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="9b557-307">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="9b557-308">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="9b557-308">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="9b557-309">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-309">May 6, 2019</span></span>

<span data-ttu-id="9b557-310">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="9b557-310">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-311">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-311">ACS</span></span>
* <span data-ttu-id="9b557-312">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="9b557-312">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="9b557-313">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="9b557-313">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="9b557-314">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="9b557-314">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="9b557-315">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="9b557-315">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-316">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-316">Appservice</span></span>
* <span data-ttu-id="9b557-317">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="9b557-317">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="9b557-318">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="9b557-318">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="9b557-319">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9b557-319">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="9b557-320">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="9b557-320">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="9b557-321">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9b557-321">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="9b557-322">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="9b557-322">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="9b557-323">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="9b557-323">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="9b557-324">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="9b557-324">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="9b557-325">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-325">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="9b557-326">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="9b557-326">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-327">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-327">Batch</span></span>
* <span data-ttu-id="9b557-328">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="9b557-328">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-329">Botservice</span><span class="sxs-lookup"><span data-stu-id="9b557-329">Botservice</span></span>
* <span data-ttu-id="9b557-330">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="9b557-330">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="9b557-331">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="9b557-331">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="9b557-332">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="9b557-332">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="9b557-333">__REMARQUE :__  `bot prepare-publish` utilise toujours l’ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-333">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="9b557-334">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="9b557-334">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="9b557-335">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-335">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="9b557-336">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="9b557-336">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="9b557-337">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="9b557-337">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="9b557-338">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="9b557-338">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="9b557-339">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="9b557-339">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="9b557-340">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="9b557-340">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="9b557-341">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="9b557-341">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="9b557-342">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="9b557-342">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="9b557-343">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="9b557-343">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="9b557-344">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-344">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="9b557-345">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="9b557-345">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="9b557-346">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9b557-346">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9b557-347">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="9b557-347">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="9b557-348">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9b557-348">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="9b557-349">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9b557-349">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9b557-350">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="9b557-350">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="9b557-351">Configuration</span><span class="sxs-lookup"><span data-stu-id="9b557-351">Configure</span></span>
* <span data-ttu-id="9b557-352">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="9b557-352">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9b557-353">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9b557-353">Eventhubs</span></span>
* <span data-ttu-id="9b557-354">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-354">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9b557-355">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-355">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-356">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-356">Network</span></span>
* <span data-ttu-id="9b557-357">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-357">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="9b557-358">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9b557-358">Policy Insights</span></span>
* <span data-ttu-id="9b557-359">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-359">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="9b557-360">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-360">Role</span></span>
* <span data-ttu-id="9b557-361">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-361">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="9b557-362">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9b557-362">Service Bus</span></span>
* <span data-ttu-id="9b557-363">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-363">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9b557-364">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-364">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="9b557-365">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="9b557-365">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-366">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-366">SQL</span></span>
* <span data-ttu-id="9b557-367">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="9b557-367">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-368">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-368">VM</span></span>
* <span data-ttu-id="9b557-369">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="9b557-369">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="9b557-370">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="9b557-370">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="9b557-371">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-371">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="9b557-372">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="9b557-372">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="9b557-373">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="9b557-373">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="9b557-374">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="9b557-374">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="9b557-375">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-375">April 23, 2019</span></span>

<span data-ttu-id="9b557-376">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="9b557-376">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-377">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-377">ACS</span></span>
* <span data-ttu-id="9b557-378">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="9b557-378">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="9b557-379">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="9b557-379">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-380">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-380">AMS</span></span>
* <span data-ttu-id="9b557-381">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="9b557-381">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-382">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-382">AppService</span></span>
* <span data-ttu-id="9b557-383">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="9b557-383">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="9b557-384">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="9b557-384">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="9b557-385">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="9b557-385">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="9b557-386">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="9b557-386">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="9b557-387">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="9b557-387">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="9b557-388">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-388">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="9b557-389">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="9b557-389">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="9b557-390">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="9b557-390">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="9b557-391">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="9b557-391">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9b557-392">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="9b557-392">Deployment Manager</span></span>
* <span data-ttu-id="9b557-393">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="9b557-393">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="9b557-394">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-394">Lab</span></span>
* <span data-ttu-id="9b557-395">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="9b557-395">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="9b557-396">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-396">Network</span></span>
* <span data-ttu-id="9b557-397">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="9b557-397">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-398">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-398">Resource</span></span>
* <span data-ttu-id="9b557-399">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="9b557-399">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="9b557-400">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="9b557-400">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="9b557-401">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-401">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="9b557-402">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-402">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-403">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-403">SQL</span></span>
* <span data-ttu-id="9b557-404">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="9b557-404">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="9b557-405">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="9b557-405">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="9b557-406">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-406">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="9b557-407">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-407">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-408">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-408">Storage</span></span>
* <span data-ttu-id="9b557-409">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9b557-409">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-410">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-410">VM</span></span>
* <span data-ttu-id="9b557-411">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="9b557-411">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="9b557-412">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="9b557-412">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="9b557-413">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="9b557-413">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="9b557-414">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-414">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="9b557-415">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-415">Core</span></span>
* <span data-ttu-id="9b557-416">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="9b557-416">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-417">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-417">ACR</span></span>
* <span data-ttu-id="9b557-418">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="9b557-418">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-419">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-419">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="9b557-422">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9b557-422">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="9b557-423">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="9b557-423">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-424">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-424">AppService</span></span>
* <span data-ttu-id="9b557-425">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9b557-425">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="9b557-426">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9b557-426">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="9b557-427">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9b557-427">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="9b557-428">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9b557-428">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="9b557-429">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-429">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="9b557-430">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="9b557-430">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="9b557-431">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="9b557-431">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-432">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-432">CDN</span></span>
* <span data-ttu-id="9b557-433">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="9b557-433">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="9b557-434">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9b557-434">Feedback</span></span>
* <span data-ttu-id="9b557-435">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="9b557-435">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="9b557-436">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="9b557-436">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="9b557-437">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="9b557-437">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-438">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-438">Monitor</span></span>
* <span data-ttu-id="9b557-439">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-439">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="9b557-440">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-440">Network</span></span>
* <span data-ttu-id="9b557-441">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="9b557-441">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="9b557-442">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-442">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="9b557-443">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="9b557-443">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="9b557-444">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="9b557-444">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="9b557-445">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="9b557-445">PrivateDNS</span></span>
* <span data-ttu-id="9b557-446">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="9b557-446">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-447">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-447">Resource</span></span>
* <span data-ttu-id="9b557-448">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9b557-448">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="9b557-449">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-449">Role</span></span>
* <span data-ttu-id="9b557-450">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-450">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="9b557-451">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-451">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-452">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-452">SQL</span></span>
* <span data-ttu-id="9b557-453">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="9b557-453">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-454">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-454">Storage</span></span>
* <span data-ttu-id="9b557-455">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-455">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="9b557-456">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="9b557-456">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="9b557-457">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="9b557-457">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="9b557-458">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="9b557-458">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="9b557-459">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-459">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="9b557-460">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-460">Core</span></span>
* <span data-ttu-id="9b557-461">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="9b557-461">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="9b557-462">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="9b557-462">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="9b557-463">Cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-463">Cloud</span></span>
* <span data-ttu-id="9b557-464">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="9b557-464">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-465">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-465">ACR</span></span>
* <span data-ttu-id="9b557-466">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="9b557-466">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="9b557-467">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="9b557-467">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="9b557-468">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="9b557-468">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="9b557-469">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="9b557-469">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-470">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-470">AppService</span></span>
* <span data-ttu-id="9b557-471">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="9b557-471">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="9b557-472">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="9b557-472">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="9b557-473">Service BOT</span><span class="sxs-lookup"><span data-stu-id="9b557-473">BOT Service</span></span>
* <span data-ttu-id="9b557-474">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="9b557-474">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="9b557-475">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="9b557-475">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="9b557-476">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="9b557-476">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="9b557-477">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9b557-477">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-478">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-478">CDN</span></span>
* <span data-ttu-id="9b557-479">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="9b557-479">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="9b557-480">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="9b557-480">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="9b557-481">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="9b557-481">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9b557-482">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="9b557-482">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-483">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9b557-483">Cosmosdb</span></span>
* <span data-ttu-id="9b557-484">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="9b557-484">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="9b557-485">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9b557-485">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-486">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-486">Interactive</span></span>
* <span data-ttu-id="9b557-487">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="9b557-487">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-488">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-488">Monitor</span></span>
* <span data-ttu-id="9b557-489">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-489">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-490">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-490">Network</span></span>
* <span data-ttu-id="9b557-491">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="9b557-491">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-492">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-492">Profile</span></span>
* <span data-ttu-id="9b557-493">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="9b557-493">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="9b557-494">Postgres</span><span class="sxs-lookup"><span data-stu-id="9b557-494">Postgres</span></span> 
* <span data-ttu-id="9b557-495">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="9b557-495">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="9b557-496">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="9b557-496">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-497">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-497">Resource</span></span>
* <span data-ttu-id="9b557-498">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-498">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="9b557-499">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="9b557-499">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="9b557-500">Graph</span><span class="sxs-lookup"><span data-stu-id="9b557-500">Graph</span></span>
* <span data-ttu-id="9b557-501">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="9b557-501">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="9b557-502">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="9b557-502">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="9b557-503">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="9b557-503">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="9b557-504">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-504">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="9b557-505">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="9b557-505">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-506">storage</span><span class="sxs-lookup"><span data-stu-id="9b557-506">storage</span></span>
* <span data-ttu-id="9b557-507">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="9b557-507">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="9b557-508">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="9b557-508">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="9b557-509">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="9b557-509">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="9b557-510">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="9b557-510">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-511">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-511">VM</span></span>
* <span data-ttu-id="9b557-512">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="9b557-512">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="9b557-513">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-513">March 12, 2019</span></span>

<span data-ttu-id="9b557-514">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="9b557-514">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="9b557-515">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-515">Core</span></span>

* <span data-ttu-id="9b557-516">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="9b557-516">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-517">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-517">ACR</span></span>

* <span data-ttu-id="9b557-518">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="9b557-518">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-519">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-519">ACS</span></span>

* <span data-ttu-id="9b557-520">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="9b557-520">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="9b557-521">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-521">AppService</span></span>

* <span data-ttu-id="9b557-522">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="9b557-522">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="9b557-523">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9b557-523">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="9b557-524">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-524">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="9b557-525">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="9b557-525">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-526">Botservice</span><span class="sxs-lookup"><span data-stu-id="9b557-526">Botservice</span></span>

* <span data-ttu-id="9b557-527">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9b557-527">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9b557-528">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9b557-528">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9b557-529">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="9b557-529">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="9b557-530">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="9b557-530">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="9b557-531">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-531">Container</span></span>

* <span data-ttu-id="9b557-532">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="9b557-532">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="9b557-533">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9b557-533">EventHub</span></span>

* <span data-ttu-id="9b557-534">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="9b557-534">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="9b557-535">Rechercher</span><span class="sxs-lookup"><span data-stu-id="9b557-535">Find</span></span>

* <span data-ttu-id="9b557-536">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="9b557-536">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-537">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-537">HDInsight</span></span>

* <span data-ttu-id="9b557-538">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="9b557-538">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="9b557-539">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-539">Network</span></span>

* <span data-ttu-id="9b557-540">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="9b557-540">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-541">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9b557-541">Rdbms</span></span>

* <span data-ttu-id="9b557-542">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="9b557-542">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="9b557-543">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-543">Role</span></span>

* <span data-ttu-id="9b557-544">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="9b557-544">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="9b557-545">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="9b557-545">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9b557-546">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9b557-546">Service Fabric</span></span>

* <span data-ttu-id="9b557-547">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="9b557-547">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="9b557-548">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-548">February 26, 2019</span></span>

<span data-ttu-id="9b557-549">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="9b557-549">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="9b557-550">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-550">Core</span></span>

* <span data-ttu-id="9b557-551">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="9b557-551">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-552">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-552">ACR</span></span>

* <span data-ttu-id="9b557-553">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="9b557-553">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="9b557-554">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="9b557-554">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-555">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-555">ACS</span></span>

* <span data-ttu-id="9b557-556">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="9b557-556">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-557">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-557">AppService</span></span>

* <span data-ttu-id="9b557-558">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="9b557-558">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-559">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-559">Batch</span></span>
* <span data-ttu-id="9b557-560">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="9b557-560">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="9b557-561">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="9b557-561">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="9b557-562">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="9b557-562">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="9b557-563">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="9b557-563">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="9b557-564">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="9b557-564">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="9b557-565">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="9b557-565">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-566">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-566">CosmosDB</span></span>

* <span data-ttu-id="9b557-567">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9b557-567">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="9b557-568">Kusto</span><span class="sxs-lookup"><span data-stu-id="9b557-568">Kusto</span></span>

* <span data-ttu-id="9b557-569">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="9b557-569">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="9b557-570">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-570">Network</span></span>

* <span data-ttu-id="9b557-571">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-571">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="9b557-572">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="9b557-572">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="9b557-573">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="9b557-573">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="9b557-574">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-574">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="9b557-575">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-575">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="9b557-576">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-576">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="9b557-577">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="9b557-577">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-578">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-578">Resource</span></span>

* <span data-ttu-id="9b557-579">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-579">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="9b557-580">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="9b557-580">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="9b557-581">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="9b557-581">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="9b557-582">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9b557-582">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="9b557-583">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-583">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="9b557-584">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-584">Role</span></span>

* <span data-ttu-id="9b557-585">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-585">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-586">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-586">VM</span></span>

* <span data-ttu-id="9b557-587">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="9b557-587">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="9b557-588">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-588">February 12, 2019</span></span>

<span data-ttu-id="9b557-589">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="9b557-589">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="9b557-590">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-590">Core</span></span>

* <span data-ttu-id="9b557-591">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="9b557-591">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="9b557-592">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="9b557-592">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-593">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-593">ACR</span></span>
* <span data-ttu-id="9b557-594">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="9b557-594">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="9b557-595">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-595">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-596">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-596">ACS</span></span>
* <span data-ttu-id="9b557-597">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="9b557-597">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="9b557-598">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="9b557-598">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="9b557-599">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9b557-599">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-600">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-600">AMS</span></span>
* <span data-ttu-id="9b557-601">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-601">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="9b557-602">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-602">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-603">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-603">Appservice</span></span>
* <span data-ttu-id="9b557-604">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-604">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="9b557-605">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="9b557-605">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="9b557-606">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="9b557-606">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="9b557-607">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="9b557-607">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="9b557-608">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="9b557-608">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-609">Botservice</span><span class="sxs-lookup"><span data-stu-id="9b557-609">Botservice</span></span>
* <span data-ttu-id="9b557-610">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="9b557-610">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="9b557-611">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="9b557-611">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="9b557-612">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="9b557-612">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="9b557-613">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="9b557-613">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="9b557-614">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="9b557-614">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="9b557-615">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="9b557-615">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="9b557-616">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="9b557-616">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="9b557-617">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="9b557-617">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="9b557-618">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="9b557-618">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="9b557-619">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="9b557-619">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="9b557-620">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9b557-620">Key Vault</span></span>
* <span data-ttu-id="9b557-621">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="9b557-621">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-622">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-622">Monitor</span></span>
* <span data-ttu-id="9b557-623">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="9b557-623">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-624">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-624">Network</span></span>
* <span data-ttu-id="9b557-625">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="9b557-625">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="9b557-626">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9b557-626">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="9b557-627">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="9b557-627">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="9b557-628">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-628">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9b557-629">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9b557-629">Policy Insights</span></span>
* <span data-ttu-id="9b557-630">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="9b557-630">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-631">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-631">RDBMS</span></span>
* <span data-ttu-id="9b557-632">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-632">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="9b557-633">Redis</span><span class="sxs-lookup"><span data-stu-id="9b557-633">Redis</span></span>
* <span data-ttu-id="9b557-634">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="9b557-634">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="9b557-635">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="9b557-635">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="9b557-636">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="9b557-636">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="9b557-637">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="9b557-637">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="9b557-638">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="9b557-638">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="9b557-639">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="9b557-639">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="9b557-640">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="9b557-640">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="9b557-641">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-641">Role</span></span>
* <span data-ttu-id="9b557-642">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="9b557-642">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="9b557-643">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-643">SQL VM</span></span>
* <span data-ttu-id="9b557-644">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="9b557-644">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-645">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-645">VM</span></span>
* <span data-ttu-id="9b557-646">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="9b557-646">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="9b557-647">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-647">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="9b557-648">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="9b557-648">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="9b557-649">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="9b557-649">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="9b557-650">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-650">January 31, 2019</span></span>

<span data-ttu-id="9b557-651">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="9b557-651">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="9b557-652">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-652">Core</span></span>

* <span data-ttu-id="9b557-653">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="9b557-653">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="9b557-654">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-654">January 28, 2019</span></span>

<span data-ttu-id="9b557-655">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="9b557-655">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-656">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-656">ACR</span></span>
* <span data-ttu-id="9b557-657">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="9b557-657">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-658">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-658">ACS</span></span>
* <span data-ttu-id="9b557-659">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="9b557-659">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9b557-660">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="9b557-660">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="9b557-661">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="9b557-661">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-662">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-662">AMS</span></span>
* <span data-ttu-id="9b557-663">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="9b557-663">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="9b557-664">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="9b557-664">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-665">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-665">Appservice</span></span>
* <span data-ttu-id="9b557-666">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="9b557-666">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="9b557-667">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="9b557-667">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="9b557-668">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="9b557-668">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="9b557-669">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-669">Container</span></span>
* <span data-ttu-id="9b557-670">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="9b557-670">Added `container start` command</span></span>
* <span data-ttu-id="9b557-671">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-671">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9b557-672">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9b557-672">EventGrid</span></span>
* <span data-ttu-id="9b557-673">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-673">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="9b557-674">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="9b557-674">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="9b557-675">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="9b557-675">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="9b557-676">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="9b557-676">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="9b557-677">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="9b557-677">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-678">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-678">HDInsight</span></span>
* <span data-ttu-id="9b557-679">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-679">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="9b557-680">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="9b557-680">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="9b557-681">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9b557-681">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="9b557-682">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9b557-682">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="9b557-683">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="9b557-683">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="9b557-684">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="9b557-684">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-685">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-685">IoT</span></span>
* <span data-ttu-id="9b557-686">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="9b557-686">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="9b557-687">Kusto</span><span class="sxs-lookup"><span data-stu-id="9b557-687">Kusto</span></span>
* <span data-ttu-id="9b557-688">Préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-688">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-689">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-689">Monitor</span></span>
* <span data-ttu-id="9b557-690">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-690">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-691">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-691">Profile</span></span>
* <span data-ttu-id="9b557-692">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="9b557-692">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-693">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-693">Network</span></span>
* <span data-ttu-id="9b557-694">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="9b557-694">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="9b557-695">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="9b557-695">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-696">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-696">Resource</span></span>
* <span data-ttu-id="9b557-697">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="9b557-697">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="9b557-698">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-698">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="9b557-699">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-699">SQL Virtual Machine</span></span>
* <span data-ttu-id="9b557-700">Préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-700">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-701">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-701">Storage</span></span>
* <span data-ttu-id="9b557-702">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="9b557-702">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="9b557-703">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="9b557-703">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-704">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-704">VM</span></span>
* <span data-ttu-id="9b557-705">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="9b557-705">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="9b557-706">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9b557-706">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="9b557-707">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9b557-707">January 15, 2019</span></span>

<span data-ttu-id="9b557-708">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="9b557-708">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-709">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-709">ACR</span></span>
* <span data-ttu-id="9b557-710">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="9b557-710">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="9b557-711">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="9b557-711">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="9b557-712">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="9b557-712">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="9b557-713">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-713">ACS</span></span>
* <span data-ttu-id="9b557-714">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="9b557-714">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-715">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-715">Appservice</span></span>
* <span data-ttu-id="9b557-716">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="9b557-716">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="9b557-717">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-717">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="9b557-718">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="9b557-718">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="9b557-719">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="9b557-719">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-720">Botservice</span><span class="sxs-lookup"><span data-stu-id="9b557-720">Botservice</span></span>
* <span data-ttu-id="9b557-721">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="9b557-721">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="9b557-722">Configuration</span><span class="sxs-lookup"><span data-stu-id="9b557-722">Configure</span></span>
* <span data-ttu-id="9b557-723">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="9b557-723">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-724">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-724">CosmosDB</span></span>
* <span data-ttu-id="9b557-725">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="9b557-725">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-726">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-726">HDInsight</span></span>
* <span data-ttu-id="9b557-727">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="9b557-727">Added commands for managing applications</span></span>
* <span data-ttu-id="9b557-728">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="9b557-728">Added commands for managing script actions</span></span>
* <span data-ttu-id="9b557-729">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="9b557-729">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="9b557-730">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="9b557-730">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="9b557-731">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9b557-731">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-732">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-732">Network</span></span>
* <span data-ttu-id="9b557-733">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-733">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="9b557-734">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="9b557-734">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="9b557-735">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-735">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="9b557-736">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-736">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="9b557-737">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-737">Role</span></span>
* <span data-ttu-id="9b557-738">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9b557-738">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="9b557-739">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="9b557-739">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="9b557-740">Sécurité</span><span class="sxs-lookup"><span data-stu-id="9b557-740">Security</span></span>
* <span data-ttu-id="9b557-741">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-741">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-742">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-742">Storage</span></span>
* <span data-ttu-id="9b557-743">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="9b557-743">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="9b557-744">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="9b557-744">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="9b557-745">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9b557-745">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="9b557-746">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9b557-746">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="9b557-747">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="9b557-747">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-748">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-748">VM</span></span>
* <span data-ttu-id="9b557-749">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="9b557-749">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="9b557-750">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-750">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9b557-751">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="9b557-751">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="9b557-752">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="9b557-752">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="9b557-753">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-753">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="9b557-754">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="9b557-754">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="9b557-755">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-755">December 20, 2018</span></span>

<span data-ttu-id="9b557-756">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="9b557-756">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="9b557-757">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-757">Appservice</span></span>
* <span data-ttu-id="9b557-758">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9b557-758">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="9b557-759">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="9b557-759">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="9b557-760">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-760">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9b557-761">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9b557-761">IoTCentral</span></span>
* <span data-ttu-id="9b557-762">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="9b557-762">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="9b557-763">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-763">Role</span></span>
* <span data-ttu-id="9b557-764">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="9b557-764">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-765">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-765">SQL</span></span>
* <span data-ttu-id="9b557-766">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="9b557-766">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-767">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-767">VM</span></span>
* <span data-ttu-id="9b557-768">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="9b557-768">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="9b557-769">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-769">December 18, 2018</span></span>

<span data-ttu-id="9b557-770">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="9b557-770">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="9b557-771">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-771">ACR</span></span>
* <span data-ttu-id="9b557-772">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="9b557-772">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="9b557-773">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="9b557-773">Condensed the table layout for task list</span></span>
* <span data-ttu-id="9b557-774">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9b557-774">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-775">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-775">ACS</span></span>
* <span data-ttu-id="9b557-776">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="9b557-776">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9b557-777">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-777">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="9b557-778">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="9b557-778">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="9b557-779">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="9b557-779">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="9b557-780">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-780">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="9b557-781">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="9b557-781">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-782">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-782">Appservice</span></span>
* <span data-ttu-id="9b557-783">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="9b557-783">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="9b557-784">Botservice</span><span class="sxs-lookup"><span data-stu-id="9b557-784">Botservice</span></span>
* <span data-ttu-id="9b557-785">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="9b557-785">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="9b557-786">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="9b557-786">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="9b557-787">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="9b557-787">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="9b557-788">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="9b557-788">Reduced Kudu network calls</span></span>
* <span data-ttu-id="9b557-789">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="9b557-789">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-790">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-790">Consumption</span></span>
* <span data-ttu-id="9b557-791">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="9b557-791">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-792">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-792">CosmosDB</span></span>
* <span data-ttu-id="9b557-793">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="9b557-793">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="9b557-794">Cartes</span><span class="sxs-lookup"><span data-stu-id="9b557-794">Maps</span></span>
* <span data-ttu-id="9b557-795">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-795">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-796">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-796">Network</span></span>
* <span data-ttu-id="9b557-797">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="9b557-797">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="9b557-798">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9b557-798">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-799">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-799">Resource</span></span>
* <span data-ttu-id="9b557-800">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-800">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="9b557-801">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-801">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-802">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-802">Storage</span></span>
*  <span data-ttu-id="9b557-803">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="9b557-803">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-804">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-804">VM</span></span>
* <span data-ttu-id="9b557-805">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="9b557-805">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="9b557-806">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-806">December 4, 2018</span></span>

<span data-ttu-id="9b557-807">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="9b557-807">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="9b557-808">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-808">Core</span></span>
* <span data-ttu-id="9b557-809">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="9b557-809">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="9b557-810">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="9b557-810">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-811">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-811">Appservice</span></span>
* <span data-ttu-id="9b557-812">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="9b557-812">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="9b557-813">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="9b557-813">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="9b557-814">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-814">Network</span></span>
* <span data-ttu-id="9b557-815">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="9b557-815">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="9b557-816">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-816">Role</span></span>
* <span data-ttu-id="9b557-817">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="9b557-817">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="9b557-818">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-818">VM</span></span>
* <span data-ttu-id="9b557-819">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="9b557-819">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="9b557-820">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="9b557-820">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="9b557-821">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="9b557-821">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="9b557-822">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="9b557-822">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="9b557-823">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-823">November 20, 2018</span></span>

<span data-ttu-id="9b557-824">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="9b557-824">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="9b557-825">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-825">Core</span></span>
* <span data-ttu-id="9b557-826">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="9b557-826">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-827">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-827">ACR</span></span>
* <span data-ttu-id="9b557-828">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="9b557-828">Added context token to task step</span></span>
* <span data-ttu-id="9b557-829">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="9b557-829">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="9b557-830">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9b557-830">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-831">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-831">Appservice</span></span>
* <span data-ttu-id="9b557-832">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="9b557-832">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="9b557-833">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="9b557-833">Updated the default `node_version`.</span></span> <span data-ttu-id="9b557-834">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="9b557-834">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="9b557-835">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-835">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="9b557-836">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="9b557-836">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9b557-837">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9b557-837">IotCentral</span></span>
* <span data-ttu-id="9b557-838">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="9b557-838">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-839">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-839">KeyVault</span></span>
* <span data-ttu-id="9b557-840">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="9b557-840">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="9b557-841">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-841">Network</span></span>
* <span data-ttu-id="9b557-842">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="9b557-842">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="9b557-843">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="9b557-843">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="9b557-844">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9b557-844">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="9b557-845">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="9b557-845">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-846">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9b557-846">Rdbms</span></span>
* <span data-ttu-id="9b557-847">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="9b557-847">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="9b557-848">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="9b557-848">Rbac</span></span>
* <span data-ttu-id="9b557-849">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9b557-849">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="9b557-850">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="9b557-850">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="9b557-851">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-851">Storage</span></span>
* <span data-ttu-id="9b557-852">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-852">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="9b557-853">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="9b557-853">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="9b557-854">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="9b557-854">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="9b557-855">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="9b557-855">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-856">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-856">VM</span></span>
* <span data-ttu-id="9b557-857">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="9b557-857">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="9b557-858">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="9b557-858">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="9b557-859">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="9b557-859">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="9b557-860">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="9b557-860">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="9b557-861">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="9b557-861">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="9b557-862">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-862">Added `snapshot wait` command</span></span>
* <span data-ttu-id="9b557-863">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-863">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="9b557-864">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-864">November 6, 2018</span></span>

<span data-ttu-id="9b557-865">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="9b557-865">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="9b557-866">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-866">Core</span></span>
* <span data-ttu-id="9b557-867">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="9b557-867">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-868">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-868">ACR</span></span>
* <span data-ttu-id="9b557-869">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="9b557-869">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="9b557-870">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="9b557-870">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-871">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-871">ACS</span></span>
* <span data-ttu-id="9b557-872">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-872">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="9b557-873">Advisor</span><span class="sxs-lookup"><span data-stu-id="9b557-873">Advisor</span></span>
* <span data-ttu-id="9b557-874">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="9b557-874">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-875">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-875">AMS</span></span>
* <span data-ttu-id="9b557-876">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="9b557-876">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="9b557-877">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="9b557-877">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="9b557-878">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9b557-878">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="9b557-879">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="9b557-879">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="9b557-880">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="9b557-880">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="9b557-881">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="9b557-881">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="9b557-882">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="9b557-882">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="9b557-883">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="9b557-883">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="9b557-884">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9b557-884">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="9b557-885">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9b557-885">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="9b557-886">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="9b557-886">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="9b557-887">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="9b557-887">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="9b557-888">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="9b557-888">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="9b557-889">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="9b557-889">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="9b557-890">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="9b557-890">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="9b557-891">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="9b557-891">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="9b557-892">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="9b557-892">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-893">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-893">AppService</span></span>
* <span data-ttu-id="9b557-894">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="9b557-894">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="9b557-895">Configuration</span><span class="sxs-lookup"><span data-stu-id="9b557-895">Configure</span></span>
* <span data-ttu-id="9b557-896">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="9b557-896">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="9b557-897">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-897">Container</span></span>
* <span data-ttu-id="9b557-898">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="9b557-898">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="9b557-899">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9b557-899">EventHub</span></span>
* <span data-ttu-id="9b557-900">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-900">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-901">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-901">Interactive</span></span>
* <span data-ttu-id="9b557-902">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="9b557-902">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-903">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-903">Monitor</span></span>
* <span data-ttu-id="9b557-904">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-904">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-905">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-905">Network</span></span>
* <span data-ttu-id="9b557-906">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="9b557-906">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="9b557-907">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="9b557-907">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="9b557-908">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9b557-908">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="9b557-909">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-909">Profile</span></span>
* <span data-ttu-id="9b557-910">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="9b557-910">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-911">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-911">RDBMS</span></span>
* <span data-ttu-id="9b557-912">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="9b557-912">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-913">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-913">Resource</span></span>
* <span data-ttu-id="9b557-914">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="9b557-914">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="9b557-915">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-915">Role</span></span>
* <span data-ttu-id="9b557-916">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="9b557-916">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="9b557-917">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="9b557-917">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="9b557-918">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="9b557-918">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-919">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-919">Storage</span></span>
* <span data-ttu-id="9b557-920">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="9b557-920">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-921">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-921">VM</span></span>
* <span data-ttu-id="9b557-922">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="9b557-922">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="9b557-923">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="9b557-923">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="9b557-924">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="9b557-924">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="9b557-925">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="9b557-925">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="9b557-926">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="9b557-926">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="9b557-927">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="9b557-927">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="9b557-928">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-928">October 23, 2018</span></span>

<span data-ttu-id="9b557-929">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="9b557-929">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="9b557-930">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-930">Core</span></span>
* <span data-ttu-id="9b557-931">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="9b557-931">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="9b557-932">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="9b557-932">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-933">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-933">ACR</span></span>
* <span data-ttu-id="9b557-934">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="9b557-934">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-935">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-935">CDN</span></span>
* <span data-ttu-id="9b557-936">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="9b557-936">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9b557-937">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="9b557-937">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="9b557-938">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-938">Container</span></span>
* <span data-ttu-id="9b557-939">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="9b557-939">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="9b557-940">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-940">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="9b557-941">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="9b557-941">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="9b557-942">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-942">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="9b557-943">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="9b557-943">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="9b557-944">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="9b557-944">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="9b557-945">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="9b557-945">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-946">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-946">CosmosDB</span></span>
* <span data-ttu-id="9b557-947">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="9b557-947">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-948">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-948">Interactive</span></span>
* <span data-ttu-id="9b557-949">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="9b557-949">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="9b557-950">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9b557-950">IoT Central</span></span>
* <span data-ttu-id="9b557-951">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="9b557-951">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="9b557-952">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="9b557-952">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-953">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-953">Monitor</span></span>
* <span data-ttu-id="9b557-954">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="9b557-954">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="9b557-955">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-955">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="9b557-956">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="9b557-956">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9b557-957">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="9b557-957">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="9b557-958">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="9b557-958">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="9b557-959">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="9b557-959">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="9b557-960">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="9b557-960">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="9b557-961">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="9b557-961">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9b557-962">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="9b557-962">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="9b557-963">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9b557-963">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-964">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-964">Network</span></span>
* <span data-ttu-id="9b557-965">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-965">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="9b557-966">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-966">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="9b557-967">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9b557-967">ServiceBus</span></span>
* <span data-ttu-id="9b557-968">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="9b557-968">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-969">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-969">SQL</span></span>
* <span data-ttu-id="9b557-970">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="9b557-970">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-971">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-971">Storage</span></span>
* <span data-ttu-id="9b557-972">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="9b557-972">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="9b557-973">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="9b557-973">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-974">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-974">VM</span></span>
* <span data-ttu-id="9b557-975">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-975">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="9b557-976">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-976">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="9b557-977">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="9b557-977">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="9b557-978">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-978">October 16, 2018</span></span>

<span data-ttu-id="9b557-979">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="9b557-979">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-980">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-980">VM</span></span>
* <span data-ttu-id="9b557-981">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9b557-981">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="9b557-982">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-982">October 9, 2018</span></span>

<span data-ttu-id="9b557-983">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="9b557-983">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="9b557-984">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-984">Core</span></span>
* <span data-ttu-id="9b557-985">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="9b557-985">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-986">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-986">ACR</span></span>
* <span data-ttu-id="9b557-987">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="9b557-987">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-988">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-988">ACS</span></span>
* <span data-ttu-id="9b557-989">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="9b557-989">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="9b557-990">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="9b557-990">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="9b557-991">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="9b557-991">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="9b557-992">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="9b557-992">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="9b557-993">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-993">Container</span></span>
* <span data-ttu-id="9b557-994">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="9b557-994">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="9b557-995">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-995">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="9b557-996">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9b557-996">Event Hub</span></span>
* <span data-ttu-id="9b557-997">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="9b557-997">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="9b557-998">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="9b557-998">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="9b557-999">Extensions</span><span class="sxs-lookup"><span data-stu-id="9b557-999">Extensions</span></span>
* <span data-ttu-id="9b557-1000">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="9b557-1000">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9b557-1001">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9b557-1001">HDInsight</span></span>
* <span data-ttu-id="9b557-1002">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1002">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1003">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1003">IoT</span></span>
* <span data-ttu-id="9b557-1004">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="9b557-1004">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-1005">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-1005">KeyVault</span></span>
* <span data-ttu-id="9b557-1006">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="9b557-1006">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1007">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1007">Network</span></span>
* <span data-ttu-id="9b557-1008">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="9b557-1008">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="9b557-1009">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="9b557-1009">See #6052</span></span>
* <span data-ttu-id="9b557-1010">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1010">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="9b557-1011">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="9b557-1011">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="9b557-1012">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9b557-1012">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="9b557-1013">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9b557-1013">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="9b557-1014">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="9b557-1014">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="9b557-1015">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1015">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1016">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1016">Role</span></span>
* <span data-ttu-id="9b557-1017">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="9b557-1017">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="9b557-1018">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="9b557-1018">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="9b557-1019">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="9b557-1019">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="9b557-1020">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="9b557-1020">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="9b557-1021">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9b557-1021">Service Bus</span></span>
* <span data-ttu-id="9b557-1022">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="9b557-1022">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1023">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1023">VM</span></span>
* <span data-ttu-id="9b557-1024">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="9b557-1024">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="9b557-1025">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1025">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="9b557-1026">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="9b557-1026">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="9b557-1027">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="9b557-1027">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="9b557-1028">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1028">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="9b557-1029">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="9b557-1029">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="9b557-1030">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1030">September 21, 2018</span></span>

<span data-ttu-id="9b557-1031">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="9b557-1031">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1032">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1032">ACR</span></span>
* <span data-ttu-id="9b557-1033">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1033">Added ACR Task commands</span></span>
* <span data-ttu-id="9b557-1034">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="9b557-1034">Added quick run command</span></span>
* <span data-ttu-id="9b557-1035">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9b557-1035">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="9b557-1036">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1036">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="9b557-1037">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="9b557-1037">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="9b557-1038">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="9b557-1038">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1039">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1039">ACS</span></span>
* <span data-ttu-id="9b557-1040">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-1040">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="9b557-1041">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="9b557-1041">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1042">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1042">AppService</span></span>

* <span data-ttu-id="9b557-1043">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="9b557-1043">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="9b557-1044">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="9b557-1044">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="9b557-1045">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="9b557-1045">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="9b557-1046">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="9b557-1046">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1047">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1047">Batch</span></span>
* <span data-ttu-id="9b557-1048">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="9b557-1048">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="9b557-1049">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="9b557-1049">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="9b557-1050">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1050">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="9b557-1051">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="9b557-1051">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9b557-1052">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1052">Batch AI</span></span> 
* <span data-ttu-id="9b557-1053">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1053">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9b557-1054">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1054">Cognitive Services</span></span>
* <span data-ttu-id="9b557-1055">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="9b557-1055">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="9b557-1056">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="9b557-1056">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="9b557-1057">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="9b557-1057">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="9b557-1058">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1058">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="9b557-1059">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9b557-1059">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="9b557-1060">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="9b557-1060">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1061">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1061">Container</span></span>
* <span data-ttu-id="9b557-1062">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="9b557-1062">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="9b557-1063">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1063">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="9b557-1064">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9b557-1064">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="9b557-1065">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1065">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="9b557-1066">DataLake</span><span class="sxs-lookup"><span data-stu-id="9b557-1066">Datalake</span></span>
* <span data-ttu-id="9b557-1067">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9b557-1067">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="9b557-1068">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="9b557-1068">Interactive Shell</span></span>
* <span data-ttu-id="9b557-1069">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-1069">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="9b557-1070">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="9b557-1070">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1071">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1071">IoT</span></span>
* <span data-ttu-id="9b557-1072">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1072">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="9b557-1073">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9b557-1073">Key Vault</span></span>
* <span data-ttu-id="9b557-1074">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="9b557-1074">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1075">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1075">Network</span></span>
* <span data-ttu-id="9b557-1076">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1076">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="9b557-1077">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="9b557-1077">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="9b557-1078">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="9b557-1078">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="9b557-1079">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1079">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="9b557-1080">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1080">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="9b557-1081">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1081">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="9b557-1082">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1082">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="9b557-1083">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="9b557-1083">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="9b557-1084">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="9b557-1084">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="9b557-1085">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="9b557-1085">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="9b557-1086">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="9b557-1086">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="9b557-1087">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="9b557-1087">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="9b557-1088">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="9b557-1088">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="9b557-1089">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="9b557-1089">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="9b557-1090">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="9b557-1090">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="9b557-1091">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="9b557-1091">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="9b557-1092">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1092">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="9b557-1093">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="9b557-1093">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-1094">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-1094">RDBMS</span></span>
* <span data-ttu-id="9b557-1095">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="9b557-1095">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="9b557-1096">Réservation</span><span class="sxs-lookup"><span data-stu-id="9b557-1096">Reservation</span></span>
* <span data-ttu-id="9b557-1097">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="9b557-1097">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="9b557-1098">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="9b557-1098">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="9b557-1099">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="9b557-1099">Manage App</span></span>
* <span data-ttu-id="9b557-1100">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="9b557-1100">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="9b557-1101">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="9b557-1101">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1102">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1102">Role</span></span>
* <span data-ttu-id="9b557-1103">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="9b557-1103">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="9b557-1104">SignalR</span><span class="sxs-lookup"><span data-stu-id="9b557-1104">SignalR</span></span>
* <span data-ttu-id="9b557-1105">Première version</span><span class="sxs-lookup"><span data-stu-id="9b557-1105">First release</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1106">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1106">Storage</span></span>
* <span data-ttu-id="9b557-1107">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="9b557-1107">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="9b557-1108">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="9b557-1108">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1109">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1109">VM</span></span>
* <span data-ttu-id="9b557-1110">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="9b557-1110">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="9b557-1111">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="9b557-1111">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="9b557-1112">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1112">August 28, 2018</span></span>

<span data-ttu-id="9b557-1113">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="9b557-1113">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1114">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1114">Core</span></span>

* <span data-ttu-id="9b557-1115">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="9b557-1115">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="9b557-1116">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9b557-1116">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1117">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1117">ACR</span></span>

* <span data-ttu-id="9b557-1118">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="9b557-1118">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="9b557-1119">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="9b557-1119">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1120">ACS</span></span>

* <span data-ttu-id="9b557-1121">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="9b557-1121">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="9b557-1122">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="9b557-1122">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1123">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1123">AppService</span></span>

* <span data-ttu-id="9b557-1124">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="9b557-1124">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="9b557-1125">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="9b557-1125">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="9b557-1126">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1126">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="9b557-1127">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9b557-1127">Backup</span></span>

* <span data-ttu-id="9b557-1128">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1128">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="9b557-1129">Service de robot</span><span class="sxs-lookup"><span data-stu-id="9b557-1129">Bot Service</span></span>

* <span data-ttu-id="9b557-1130">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="9b557-1130">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9b557-1131">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1131">Cognitive Services</span></span>

* <span data-ttu-id="9b557-1132">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="9b557-1132">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1133">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1133">IoT</span></span>

* <span data-ttu-id="9b557-1134">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="9b557-1134">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1135">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1135">Monitor</span></span>

* <span data-ttu-id="9b557-1136">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="9b557-1136">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="9b557-1137">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="9b557-1137">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1138">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1138">Network</span></span>

* <span data-ttu-id="9b557-1139">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1139">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1140">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1140">Resource</span></span>

* <span data-ttu-id="9b557-1141">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1141">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1142">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1142">Storage</span></span>

* <span data-ttu-id="9b557-1143">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1143">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1144">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1144">VM</span></span>

* <span data-ttu-id="9b557-1145">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1145">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="9b557-1146">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1146">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="9b557-1147">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1147">Auguest 14, 2018</span></span>

<span data-ttu-id="9b557-1148">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="9b557-1148">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1149">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1149">Core</span></span>

* <span data-ttu-id="9b557-1150">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="9b557-1150">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="9b557-1151">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="9b557-1151">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="9b557-1152">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="9b557-1152">Telemetry</span></span>

* <span data-ttu-id="9b557-1153">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9b557-1153">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1154">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1154">ACR</span></span>

* <span data-ttu-id="9b557-1155">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="9b557-1155">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="9b557-1156">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="9b557-1156">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1157">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1157">ACS</span></span>

* <span data-ttu-id="9b557-1158">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-1158">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="9b557-1159">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-1159">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="9b557-1160">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="9b557-1160">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="9b557-1161">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="9b557-1161">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="9b557-1162">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="9b557-1162">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="9b557-1163">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1163">AppService</span></span>

* <span data-ttu-id="9b557-1164">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="9b557-1164">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="9b557-1165">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="9b557-1165">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-1166">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1166">BatchAI</span></span>

* <span data-ttu-id="9b557-1167">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="9b557-1167">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="9b557-1168">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1168">Container</span></span>

* <span data-ttu-id="9b557-1169">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1169">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="9b557-1170">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1170">IoT</span></span>

* <span data-ttu-id="9b557-1171">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="9b557-1171">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="9b557-1172">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="9b557-1172">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="9b557-1173">Iot Central</span><span class="sxs-lookup"><span data-stu-id="9b557-1173">Iot Central</span></span>

* <span data-ttu-id="9b557-1174">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="9b557-1174">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-1175">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-1175">KeyVault</span></span>


* <span data-ttu-id="9b557-1176">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="9b557-1176">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="9b557-1177">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1177">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="9b557-1178">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="9b557-1178">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="9b557-1179">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="9b557-1179">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="9b557-1180">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="9b557-1180">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="9b557-1181">Relais</span><span class="sxs-lookup"><span data-stu-id="9b557-1181">Relay</span></span>

* <span data-ttu-id="9b557-1182">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1182">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1183">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1183">Sql</span></span>

* <span data-ttu-id="9b557-1184">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="9b557-1184">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1185">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1185">Storage</span></span>

* <span data-ttu-id="9b557-1186">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="9b557-1186">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="9b557-1187">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="9b557-1187">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="9b557-1188">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="9b557-1188">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="9b557-1189">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="9b557-1189">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="9b557-1190">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1190">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1191">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1191">VM</span></span>

* <span data-ttu-id="9b557-1192">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="9b557-1192">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="9b557-1193">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1193">July 31, 2018</span></span>

<span data-ttu-id="9b557-1194">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="9b557-1194">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1195">ACR</span></span>

* <span data-ttu-id="9b557-1196">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1196">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="9b557-1197">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="9b557-1197">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1198">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1198">ACS</span></span>

* <span data-ttu-id="9b557-1199">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="9b557-1199">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1200">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1200">Batch</span></span>

* <span data-ttu-id="9b557-1201">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9b557-1201">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1202">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1202">Container</span></span>

* <span data-ttu-id="9b557-1203">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="9b557-1203">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1204">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1204">Network</span></span>

* <span data-ttu-id="9b557-1205">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9b557-1205">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="9b557-1206">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1206">Resource</span></span>

* <span data-ttu-id="9b557-1207">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-1207">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="9b557-1208">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-1208">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1209">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1209">Role</span></span>

* <span data-ttu-id="9b557-1210">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="9b557-1210">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="9b557-1211">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-1211">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="9b557-1212">Recherche</span><span class="sxs-lookup"><span data-stu-id="9b557-1212">Search</span></span>

* <span data-ttu-id="9b557-1213">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="9b557-1213">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="9b557-1214">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9b557-1214">Service Bus</span></span>

* <span data-ttu-id="9b557-1215">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="9b557-1215">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="9b557-1216">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1216">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="9b557-1217">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="9b557-1217">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="9b557-1218">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="9b557-1218">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1219">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1219">Storage</span></span>

* <span data-ttu-id="9b557-1220">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="9b557-1220">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="9b557-1221">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1221">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1222">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1222">VM</span></span>

* <span data-ttu-id="9b557-1223">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1223">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="9b557-1224">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="9b557-1224">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="9b557-1225">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="9b557-1225">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="9b557-1226">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="9b557-1226">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="9b557-1227">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1227">July 18, 2018</span></span>

<span data-ttu-id="9b557-1228">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="9b557-1228">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1229">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1229">Core</span></span>

* <span data-ttu-id="9b557-1230">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-1230">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="9b557-1231">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="9b557-1231">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="9b557-1232">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9b557-1232">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1233">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1233">ACR</span></span>

* <span data-ttu-id="9b557-1234">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="9b557-1234">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="9b557-1235">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="9b557-1235">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="9b557-1236">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="9b557-1236">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="9b557-1237">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="9b557-1237">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1238">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1238">ACS</span></span>

* <span data-ttu-id="9b557-1239">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="9b557-1239">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1240">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1240">AppService</span></span>

* <span data-ttu-id="9b557-1241">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="9b557-1241">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1242">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1242">Batch</span></span>

* <span data-ttu-id="9b557-1243">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9b557-1243">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="9b557-1244">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-1244">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9b557-1245">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1245">Batch AI</span></span>

* <span data-ttu-id="9b557-1246">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="9b557-1246">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1247">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1247">Container</span></span>

* <span data-ttu-id="9b557-1248">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="9b557-1248">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="9b557-1249">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="9b557-1249">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1250">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1250">Network</span></span>

* <span data-ttu-id="9b557-1251">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1251">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="9b557-1252">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-1252">Added `network nic wait`</span></span>
* <span data-ttu-id="9b557-1253">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1253">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="9b557-1254">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1254">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="9b557-1255">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1255">Resource</span></span>

* <span data-ttu-id="9b557-1256">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-1256">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="9b557-1257">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-1257">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="9b557-1258">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-1258">Added `deployment wait` command</span></span>
* <span data-ttu-id="9b557-1259">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="9b557-1259">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1260">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1260">SQL</span></span>

* <span data-ttu-id="9b557-1261">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1261">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="9b557-1262">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="9b557-1262">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="9b557-1263">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="9b557-1263">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1264">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1264">Storage</span></span>

* <span data-ttu-id="9b557-1265">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="9b557-1265">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1266">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1266">VM</span></span>

* <span data-ttu-id="9b557-1267">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1267">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="9b557-1268">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1268">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="9b557-1269">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="9b557-1269">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9b557-1270">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1270">July 3, 2018</span></span>

<span data-ttu-id="9b557-1271">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="9b557-1271">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="9b557-1272">AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-1272">AKS</span></span>

* <span data-ttu-id="9b557-1273">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1273">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9b557-1274">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1274">July 3, 2018</span></span>

<span data-ttu-id="9b557-1275">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="9b557-1275">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1276">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1276">Core</span></span>

* <span data-ttu-id="9b557-1277">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1277">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1278">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1278">ACR</span></span>

* <span data-ttu-id="9b557-1279">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="9b557-1279">Added polling build status</span></span>
* <span data-ttu-id="9b557-1280">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-1280">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="9b557-1281">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9b557-1281">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1282">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1282">ACS</span></span>

* <span data-ttu-id="9b557-1283">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1283">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="9b557-1284">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1284">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="9b557-1285">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1285">Updated options for `aks browse` command.</span></span> <span data-ttu-id="9b557-1286">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="9b557-1286">Added `--listen-port` support</span></span>
* <span data-ttu-id="9b557-1287">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1287">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="9b557-1288">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="9b557-1288">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="9b557-1289">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="9b557-1289">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1290">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1290">AppService</span></span>

* <span data-ttu-id="9b557-1291">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="9b557-1291">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="9b557-1292">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="9b557-1292">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="9b557-1293">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9b557-1293">Backup</span></span>

* <span data-ttu-id="9b557-1294">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="9b557-1294">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-1295">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1295">BatchAI</span></span>

* <span data-ttu-id="9b557-1296">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1296">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="9b557-1297">Cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-1297">Cloud</span></span>

* <span data-ttu-id="9b557-1298">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-1298">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1299">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1299">Container</span></span>

* <span data-ttu-id="9b557-1300">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="9b557-1300">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="9b557-1301">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="9b557-1301">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="9b557-1302">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="9b557-1302">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1303">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1303">Extension</span></span>

* <span data-ttu-id="9b557-1304">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="9b557-1304">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1305">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1305">Network</span></span>

* <span data-ttu-id="9b557-1306">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="9b557-1306">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-1307">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9b557-1307">Rdbms</span></span>

* <span data-ttu-id="9b557-1308">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-1308">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1309">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1309">Resource</span></span>

* <span data-ttu-id="9b557-1310">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="9b557-1310">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1311">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1311">VM</span></span>

* <span data-ttu-id="9b557-1312">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="9b557-1312">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="9b557-1313">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1313">June 25, 2018</span></span>

<span data-ttu-id="9b557-1314">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="9b557-1314">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="9b557-1315">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-1315">CLI</span></span>

* <span data-ttu-id="9b557-1316">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1316">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="9b557-1317">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1317">June 19, 2018</span></span>

<span data-ttu-id="9b557-1318">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="9b557-1318">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1319">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1319">Core</span></span>

* <span data-ttu-id="9b557-1320">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1320">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1321">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1321">ACR</span></span>

* <span data-ttu-id="9b557-1322">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="9b557-1322">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="9b557-1323">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1323">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1324">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1324">ACS</span></span>

* <span data-ttu-id="9b557-1325">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1325">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="9b557-1326">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1326">Added `--update` support</span></span>
* <span data-ttu-id="9b557-1327">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="9b557-1327">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="9b557-1328">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="9b557-1328">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="9b557-1329">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="9b557-1329">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="9b557-1330">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9b557-1330">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="9b557-1331">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9b557-1331">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="9b557-1332">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9b557-1332">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1333">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1333">AppService</span></span>

* <span data-ttu-id="9b557-1334">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="9b557-1334">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="9b557-1335">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="9b557-1335">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1336">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1336">Batch</span></span>

* <span data-ttu-id="9b557-1337">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="9b557-1337">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9b557-1338">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1338">Batch AI</span></span>

* <span data-ttu-id="9b557-1339">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="9b557-1339">Added support for workspaces.</span></span> <span data-ttu-id="9b557-1340">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="9b557-1340">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="9b557-1341">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="9b557-1341">Added support for experiments.</span></span> <span data-ttu-id="9b557-1342">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="9b557-1342">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="9b557-1343">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="9b557-1343">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="9b557-1344">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1344">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="9b557-1345">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="9b557-1345">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="9b557-1346">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="9b557-1346">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="9b557-1347">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="9b557-1347">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="9b557-1348">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="9b557-1348">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="9b557-1349">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1349">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="9b557-1350">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="9b557-1350">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="9b557-1351">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1351">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="9b557-1352">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="9b557-1352">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="9b557-1353">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="9b557-1353">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="9b557-1354">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="9b557-1354">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="9b557-1355">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1355">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="9b557-1356">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="9b557-1356">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="9b557-1357">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="9b557-1357">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="9b557-1358">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9b557-1358">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9b557-1359">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9b557-1359">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9b557-1360">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="9b557-1360">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="9b557-1361">Cartes</span><span class="sxs-lookup"><span data-stu-id="9b557-1361">Maps</span></span>

* <span data-ttu-id="9b557-1362">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="9b557-1362">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1363">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1363">Network</span></span>

* <span data-ttu-id="9b557-1364">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="9b557-1364">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="9b557-1365">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="9b557-1365">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="9b557-1366">#6502</span><span class="sxs-lookup"><span data-stu-id="9b557-1366">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="9b557-1367">Réservations</span><span class="sxs-lookup"><span data-stu-id="9b557-1367">Reservations</span></span>

* <span data-ttu-id="9b557-1368">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1368">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="9b557-1369">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1369">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="9b557-1370">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="9b557-1370">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="9b557-1371">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="9b557-1371">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="9b557-1372">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="9b557-1372">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="9b557-1373">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1373">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1374">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1374">Role</span></span>

* <span data-ttu-id="9b557-1375">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1375">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1376">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1376">SQL</span></span>

* <span data-ttu-id="9b557-1377">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1377">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1378">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1378">Storage</span></span>

* <span data-ttu-id="9b557-1379">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="9b557-1379">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1380">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1380">VM</span></span>

* <span data-ttu-id="9b557-1381">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1381">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="9b557-1382">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="9b557-1382">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="9b557-1383">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="9b557-1383">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9b557-1384">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1384">June 13, 2018</span></span>

<span data-ttu-id="9b557-1385">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="9b557-1385">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1386">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1386">Core</span></span>

* <span data-ttu-id="9b557-1387">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1387">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9b557-1388">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1388">June 13, 2018</span></span>

<span data-ttu-id="9b557-1389">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="9b557-1389">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="9b557-1390">AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-1390">AKS</span></span>

* <span data-ttu-id="9b557-1391">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1391">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="9b557-1392">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="9b557-1392">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="9b557-1393">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1393">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="9b557-1394">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1394">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="9b557-1395">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1395">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1396">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1396">AppService</span></span>

* <span data-ttu-id="9b557-1397">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="9b557-1397">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9b557-1398">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1398">June 5, 2018</span></span>

<span data-ttu-id="9b557-1399">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="9b557-1399">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1400">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1400">Interactive</span></span>

* <span data-ttu-id="9b557-1401">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="9b557-1401">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9b557-1402">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1402">June 5, 2018</span></span>

<span data-ttu-id="9b557-1403">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="9b557-1403">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1404">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1404">Core</span></span>

* <span data-ttu-id="9b557-1405">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="9b557-1405">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="9b557-1406">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9b557-1406">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1407">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1407">ACR</span></span>

* <span data-ttu-id="9b557-1408">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="9b557-1408">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="9b557-1409">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="9b557-1409">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="9b557-1410">AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-1410">AKS</span></span>

* <span data-ttu-id="9b557-1411">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="9b557-1411">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1412">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1412">Batch</span></span>

* <span data-ttu-id="9b557-1413">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="9b557-1413">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1414">IOT</span><span class="sxs-lookup"><span data-stu-id="9b557-1414">IOT</span></span>

* <span data-ttu-id="9b557-1415">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="9b557-1415">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1416">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1416">Network</span></span>

* <span data-ttu-id="9b557-1417">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="9b557-1417">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9b557-1418">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9b557-1418">Policy Insights</span></span>

* <span data-ttu-id="9b557-1419">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1419">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="9b557-1420">ARM</span><span class="sxs-lookup"><span data-stu-id="9b557-1420">ARM</span></span>

* <span data-ttu-id="9b557-1421">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1421">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1422">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1422">SQL</span></span>

* <span data-ttu-id="9b557-1423">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="9b557-1423">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="9b557-1424">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="9b557-1424">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="9b557-1425">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1425">Storage</span></span>

* <span data-ttu-id="9b557-1426">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="9b557-1426">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1427">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1427">VM</span></span>

* <span data-ttu-id="9b557-1428">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="9b557-1428">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="9b557-1429">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1429">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="9b557-1430">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1430">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="9b557-1431">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1431">May 22, 2018</span></span>

<span data-ttu-id="9b557-1432">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="9b557-1432">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1433">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1433">Core</span></span>

* <span data-ttu-id="9b557-1434">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="9b557-1434">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1435">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1435">ACS</span></span>

* <span data-ttu-id="9b557-1436">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="9b557-1436">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="9b557-1437">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="9b557-1437">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1438">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1438">AppService</span></span>

* <span data-ttu-id="9b557-1439">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="9b557-1439">Improved generic update commands</span></span>
* <span data-ttu-id="9b557-1440">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="9b557-1440">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1441">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1441">Container</span></span>

* <span data-ttu-id="9b557-1442">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="9b557-1442">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="9b557-1443">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1443">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1444">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1444">Extension</span></span>

* <span data-ttu-id="9b557-1445">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="9b557-1445">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1446">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1446">Interactive</span></span>

* <span data-ttu-id="9b557-1447">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1447">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="9b557-1448">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="9b557-1448">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-1449">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-1449">KeyVault</span></span>

* <span data-ttu-id="9b557-1450">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="9b557-1450">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1451">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1451">Network</span></span>

* <span data-ttu-id="9b557-1452">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="9b557-1452">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="9b557-1453">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="9b557-1453">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1454">SQL</span></span>

* <span data-ttu-id="9b557-1455">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="9b557-1455">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="9b557-1456">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="9b557-1456">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="9b557-1457">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="9b557-1457">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="9b557-1458">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="9b557-1458">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="9b557-1459">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="9b557-1459">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="9b557-1460">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1460">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="9b557-1461">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="9b557-1461">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="9b557-1462">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1462">`edition`.</span></span> <span data-ttu-id="9b557-1463">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="9b557-1463">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="9b557-1464">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1464">`elasticPoolName`.</span></span> <span data-ttu-id="9b557-1465">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="9b557-1465">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="9b557-1466">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="9b557-1466">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="9b557-1467">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1467">`edition`.</span></span> <span data-ttu-id="9b557-1468">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="9b557-1468">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="9b557-1469">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1469">`dtu`.</span></span> <span data-ttu-id="9b557-1470">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="9b557-1470">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="9b557-1471">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1471">`databaseDtuMin`.</span></span> <span data-ttu-id="9b557-1472">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="9b557-1472">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="9b557-1473">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1473">`databaseDtuMax`.</span></span> <span data-ttu-id="9b557-1474">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="9b557-1474">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="9b557-1475">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="9b557-1475">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="9b557-1476">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="9b557-1476">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1477">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1477">Storage</span></span>

* <span data-ttu-id="9b557-1478">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-1478">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="9b557-1479">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="9b557-1479">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1480">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1480">VM</span></span>

* <span data-ttu-id="9b557-1481">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1481">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="9b557-1482">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="9b557-1482">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="9b557-1483">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="9b557-1483">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="9b557-1484">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="9b557-1484">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="9b557-1485">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1485">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="9b557-1486">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1486">May 7, 2018</span></span>

<span data-ttu-id="9b557-1487">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="9b557-1487">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1488">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1488">Core</span></span>

* <span data-ttu-id="9b557-1489">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="9b557-1489">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="9b557-1490">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="9b557-1490">Added limited support for positional arguments</span></span>
* <span data-ttu-id="9b557-1491">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1491">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="9b557-1492">#5591</span><span class="sxs-lookup"><span data-stu-id="9b557-1492">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="9b557-1493">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1493">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="9b557-1494">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="9b557-1494">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="9b557-1495">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1495">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="9b557-1496">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="9b557-1496">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="9b557-1497">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-1497">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1498">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1498">ACR</span></span>

* <span data-ttu-id="9b557-1499">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1499">Added ACR Build commands</span></span>
* <span data-ttu-id="9b557-1500">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="9b557-1500">Improved resource not found error messages</span></span>
* <span data-ttu-id="9b557-1501">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1501">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="9b557-1502">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="9b557-1502">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="9b557-1503">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="9b557-1503">Improved repository commands error messages</span></span>
* <span data-ttu-id="9b557-1504">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="9b557-1504">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1505">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1505">ACS</span></span>

* <span data-ttu-id="9b557-1506">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-1506">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="9b557-1507">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="9b557-1507">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="9b557-1508">AMS</span><span class="sxs-lookup"><span data-stu-id="9b557-1508">AMS</span></span>

* <span data-ttu-id="9b557-1509">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1509">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1510">Appservice</span></span>

* <span data-ttu-id="9b557-1511">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="9b557-1511">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="9b557-1512">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1512">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="9b557-1513">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="9b557-1513">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="9b557-1514">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1514">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9b557-1515">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1515">Batch AI</span></span>

* <span data-ttu-id="9b557-1516">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="9b557-1516">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9b557-1517">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1517">Cognitive Services</span></span>

* <span data-ttu-id="9b557-1518">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="9b557-1518">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-1519">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-1519">Consumption</span></span>

* <span data-ttu-id="9b557-1520">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="9b557-1520">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1521">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1521">Container</span></span>

* <span data-ttu-id="9b557-1522">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="9b557-1522">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9b557-1523">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9b557-1523">Cosmos DB</span></span>

* <span data-ttu-id="9b557-1524">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9b557-1524">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="9b557-1525">DMS</span><span class="sxs-lookup"><span data-stu-id="9b557-1525">DMS</span></span>

* <span data-ttu-id="9b557-1526">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="9b557-1526">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1527">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1527">Extension</span></span>

* <span data-ttu-id="9b557-1528">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="9b557-1528">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1529">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1529">Interactive</span></span>

* <span data-ttu-id="9b557-1530">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="9b557-1530">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="9b557-1531">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="9b557-1531">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="9b557-1532">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="9b557-1532">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="9b557-1533">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1533">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="9b557-1534">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-1534">Lab</span></span>

* <span data-ttu-id="9b557-1535">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="9b557-1535">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1536">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1536">Network</span></span>

* <span data-ttu-id="9b557-1537">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="9b557-1537">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="9b557-1538">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1538">Profile</span></span>

* <span data-ttu-id="9b557-1539">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1539">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="9b557-1540">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="9b557-1540">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="9b557-1541">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="9b557-1541">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="9b557-1542">Redis</span><span class="sxs-lookup"><span data-stu-id="9b557-1542">Redis</span></span>

* <span data-ttu-id="9b557-1543">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1543">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="9b557-1544">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="9b557-1544">Deprecated `redis list-all`.</span></span> <span data-ttu-id="9b557-1545">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1545">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="9b557-1546">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="9b557-1546">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="9b557-1547">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1547">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1548">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1548">Role</span></span>

* <span data-ttu-id="9b557-1549">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9b557-1549">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1550">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1550">Storage</span></span>

* <span data-ttu-id="9b557-1551">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="9b557-1551">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="9b557-1552">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="9b557-1552">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="9b557-1553">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="9b557-1553">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="9b557-1554">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="9b557-1554">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="9b557-1555">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1555">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1556">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1556">VM</span></span>

* <span data-ttu-id="9b557-1557">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="9b557-1557">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="9b557-1558">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="9b557-1558">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="9b557-1559">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="9b557-1559">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="9b557-1560">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="9b557-1560">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="9b557-1561">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="9b557-1561">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="9b557-1562">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="9b557-1562">Added write accelerator support</span></span>
* <span data-ttu-id="9b557-1563">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9b557-1563">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="9b557-1564">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1564">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="9b557-1565">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="9b557-1565">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="9b557-1566">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1566">April 10, 2018</span></span>

<span data-ttu-id="9b557-1567">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="9b557-1567">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1568">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1568">ACR</span></span>

* <span data-ttu-id="9b557-1569">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="9b557-1569">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1570">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1570">ACS</span></span>

* <span data-ttu-id="9b557-1571">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="9b557-1571">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1572">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1572">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="9b557-1574">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="9b557-1574">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-1575">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1575">BatchAI</span></span>

* <span data-ttu-id="9b557-1576">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="9b557-1576">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="9b557-1577">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="9b557-1577">Job level mounting</span></span>
  - <span data-ttu-id="9b557-1578">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="9b557-1578">Environment variables with secret values</span></span>
  - <span data-ttu-id="9b557-1579">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="9b557-1579">Performance counters settings</span></span>
  - <span data-ttu-id="9b557-1580">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="9b557-1580">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="9b557-1581">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="9b557-1581">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="9b557-1582">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="9b557-1582">Usage and limits reporting</span></span>
  - <span data-ttu-id="9b557-1583">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="9b557-1583">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="9b557-1584">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="9b557-1584">Support for custom images</span></span>
  - <span data-ttu-id="9b557-1585">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="9b557-1585">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="9b557-1586">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="9b557-1586">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="9b557-1587">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="9b557-1587">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="9b557-1588">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="9b557-1588">National clouds are supported</span></span>
* <span data-ttu-id="9b557-1589">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="9b557-1589">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="9b557-1590">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="9b557-1590">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="9b557-1591">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-1591">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="9b557-1592">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="9b557-1592">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="9b557-1593">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="9b557-1593">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="9b557-1594">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="9b557-1594">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="9b557-1595">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1595">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="9b557-1596">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="9b557-1596">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="9b557-1597">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="9b557-1597">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="9b557-1598">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1598">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="9b557-1599">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-1599">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="9b557-1600">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="9b557-1600">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="9b557-1601">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1601">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="9b557-1602">Facturation</span><span class="sxs-lookup"><span data-stu-id="9b557-1602">Billing</span></span>

* <span data-ttu-id="9b557-1603">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="9b557-1603">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-1604">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-1604">Consumption</span></span>

* <span data-ttu-id="9b557-1605">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="9b557-1605">Added `marketplace` commands</span></span>
* <span data-ttu-id="9b557-1606">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9b557-1606">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="9b557-1607">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="9b557-1607">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="9b557-1608">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="9b557-1608">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="9b557-1609">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9b557-1609">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="9b557-1610">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="9b557-1610">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1611">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1611">Container</span></span>

* <span data-ttu-id="9b557-1612">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="9b557-1612">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="9b557-1613">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="9b557-1613">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1614">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1614">Extension</span></span>

* <span data-ttu-id="9b557-1615">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="9b557-1615">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1616">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1616">Interactive</span></span>

* <span data-ttu-id="9b557-1617">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="9b557-1617">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="9b557-1618">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-1618">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="9b557-1619">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="9b557-1619">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1620">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1620">Network</span></span>

* <span data-ttu-id="9b557-1621">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="9b557-1621">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="9b557-1622">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1622">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="9b557-1623">#4910</span><span class="sxs-lookup"><span data-stu-id="9b557-1623">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="9b557-1624">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="9b557-1624">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="9b557-1625">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="9b557-1625">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="9b557-1626">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1626">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="9b557-1627">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1627">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="9b557-1628">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="9b557-1628">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-1629">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1629">Profile</span></span>

* <span data-ttu-id="9b557-1630">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1630">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="9b557-1631">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="9b557-1631">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-1632">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-1632">RDBMS</span></span>

* <span data-ttu-id="9b557-1633">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="9b557-1633">Added `georestore` command</span></span>
* <span data-ttu-id="9b557-1634">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1634">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1635">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1635">Resource</span></span>

* <span data-ttu-id="9b557-1636">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1636">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="9b557-1637">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1637">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1638">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1638">SQL</span></span>

* <span data-ttu-id="9b557-1639">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="9b557-1639">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1640">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1640">Storage</span></span>

* <span data-ttu-id="9b557-1641">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="9b557-1641">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1642">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1642">VM</span></span>

* <span data-ttu-id="9b557-1643">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1643">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="9b557-1644">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="9b557-1644">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="9b557-1646">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1646">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="9b557-1647">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="9b557-1647">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="9b557-1648">#5718</span><span class="sxs-lookup"><span data-stu-id="9b557-1648">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="9b557-1649">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="9b557-1649">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="9b557-1650">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1650">March 27, 2018</span></span>

<span data-ttu-id="9b557-1651">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="9b557-1651">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1652">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1652">Core</span></span>

* <span data-ttu-id="9b557-1653">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="9b557-1653">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1654">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1654">ACS</span></span>

* <span data-ttu-id="9b557-1655">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9b557-1655">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1656">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1656">Appservice</span></span>

* <span data-ttu-id="9b557-1657">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1657">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="9b557-1658">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1658">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9b557-1659">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9b557-1659">Backup</span></span>

* <span data-ttu-id="9b557-1660">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="9b557-1660">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="9b557-1661">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-1661">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="9b557-1662">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9b557-1662">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="9b557-1663">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1663">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1664">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1664">Container</span></span>

* <span data-ttu-id="9b557-1665">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="9b557-1665">Added `container exec` command.</span></span> <span data-ttu-id="9b557-1666">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="9b557-1666">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="9b557-1667">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1667">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1668">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1668">Extension</span></span>

* <span data-ttu-id="9b557-1669">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-1669">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="9b557-1670">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="9b557-1670">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="9b557-1671">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1671">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1672">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1672">Interactive</span></span>

* <span data-ttu-id="9b557-1673">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-1673">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="9b557-1674">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="9b557-1674">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="9b557-1675">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="9b557-1675">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="9b557-1676">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="9b557-1676">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="9b557-1677">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-1677">Lab</span></span>

* <span data-ttu-id="9b557-1678">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="9b557-1678">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1679">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1679">Monitor</span></span>

* <span data-ttu-id="9b557-1680">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="9b557-1680">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="9b557-1681">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="9b557-1681">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="9b557-1682">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="9b557-1682">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1683">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1683">Network</span></span>

* <span data-ttu-id="9b557-1684">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="9b557-1684">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-1685">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1685">Profile</span></span>

* <span data-ttu-id="9b557-1686">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="9b557-1686">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-1687">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-1687">RDBMS</span></span>

* <span data-ttu-id="9b557-1688">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="9b557-1688">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1689">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1689">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="9b557-1691">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1691">Role</span></span>

* <span data-ttu-id="9b557-1692">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1692">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="9b557-1693">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="9b557-1693">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="9b557-1694">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1694">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="9b557-1695">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1695">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="9b557-1696">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="9b557-1696">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1697">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1697">Storage</span></span>

* <span data-ttu-id="9b557-1698">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="9b557-1698">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="9b557-1699">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="9b557-1699">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1700">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1700">VM</span></span>

* <span data-ttu-id="9b557-1701">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="9b557-1701">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="9b557-1702">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1702">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="9b557-1703">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="9b557-1703">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="9b557-1704">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="9b557-1704">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="9b557-1705">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1705">March 13, 2018</span></span>

<span data-ttu-id="9b557-1706">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="9b557-1706">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1707">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1707">ACR</span></span>

* <span data-ttu-id="9b557-1708">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-1708">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="9b557-1709">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="9b557-1709">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="9b557-1710">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="9b557-1710">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1711">ACS</span></span>

* <span data-ttu-id="9b557-1712">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="9b557-1712">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="9b557-1713">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="9b557-1713">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="9b557-1714">Advisor</span><span class="sxs-lookup"><span data-stu-id="9b557-1714">Advisor</span></span>

* <span data-ttu-id="9b557-1715">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1715">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="9b557-1716">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1716">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="9b557-1717">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="9b557-1717">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="9b557-1718">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1718">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="9b557-1719">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1719">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1720">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1720">Appservice</span></span>

* <span data-ttu-id="9b557-1721">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9b557-1721">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="9b557-1722">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1722">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9b557-1723">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9b557-1723">Eventhubs</span></span>

* <span data-ttu-id="9b557-1724">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1724">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1725">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1725">Extension</span></span>

* <span data-ttu-id="9b557-1726">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1726">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1727">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1727">Interactive</span></span>

* <span data-ttu-id="9b557-1728">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="9b557-1728">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="9b557-1729">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="9b557-1729">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="9b557-1730">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="9b557-1730">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="9b557-1731">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="9b557-1731">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1732">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1732">Monitor</span></span>

* <span data-ttu-id="9b557-1733">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="9b557-1733">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="9b557-1734">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="9b557-1734">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="9b557-1735">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="9b557-1735">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="9b557-1736">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-1736">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1737">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1737">Network</span></span>

* <span data-ttu-id="9b557-1738">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1738">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="9b557-1739">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9b557-1739">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="9b557-1740">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="9b557-1740">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="9b557-1741">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="9b557-1741">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-1742">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1742">Profile</span></span>

* <span data-ttu-id="9b557-1743">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="9b557-1743">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="9b557-1744">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="9b557-1744">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-1745">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-1745">RDBMS</span></span>

* <span data-ttu-id="9b557-1746">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-1746">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="9b557-1747">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9b557-1747">Service Bus</span></span>

* <span data-ttu-id="9b557-1748">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1748">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1749">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1749">Storage</span></span>

* <span data-ttu-id="9b557-1750">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="9b557-1750">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="9b557-1751">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="9b557-1751">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1752">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1752">VM</span></span>

* <span data-ttu-id="9b557-1753">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="9b557-1753">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="9b557-1754">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="9b557-1754">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="9b557-1755">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="9b557-1755">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="9b557-1756">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="9b557-1756">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="9b557-1757">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1757">February 27, 2018</span></span>

<span data-ttu-id="9b557-1758">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="9b557-1758">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1759">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1759">Core</span></span>

* <span data-ttu-id="9b557-1760">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="9b557-1760">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="9b557-1761">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="9b557-1761">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="9b557-1762">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="9b557-1762">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1763">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1763">ACS</span></span>

* <span data-ttu-id="9b557-1764">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1764">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="9b557-1765">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="9b557-1765">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="9b557-1766">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9b557-1766">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="9b557-1767">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="9b557-1767">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1768">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1768">Appservice</span></span>

* <span data-ttu-id="9b557-1769">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="9b557-1769">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="9b557-1770">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="9b557-1770">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9b557-1771">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1771">Cognitive Services</span></span>

* <span data-ttu-id="9b557-1772">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-1772">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-1773">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-1773">Consumption</span></span>

* <span data-ttu-id="9b557-1774">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="9b557-1774">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="9b557-1775">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="9b557-1775">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1776">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1776">Container</span></span>

* <span data-ttu-id="9b557-1777">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="9b557-1777">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1778">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1778">Network</span></span>

* <span data-ttu-id="9b557-1779">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="9b557-1779">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1780">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1780">Resource</span></span>

* <span data-ttu-id="9b557-1781">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="9b557-1781">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1782">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1782">Role</span></span>

* <span data-ttu-id="9b557-1783">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="9b557-1783">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1784">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1784">SQL</span></span>

* <span data-ttu-id="9b557-1785">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="9b557-1785">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1786">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1786">Storage</span></span>

* <span data-ttu-id="9b557-1787">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1787">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1788">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1788">VM</span></span>

* <span data-ttu-id="9b557-1789">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="9b557-1789">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="9b557-1790">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1790">February 13, 2018</span></span>

<span data-ttu-id="9b557-1791">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="9b557-1791">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1792">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1792">Core</span></span>

* <span data-ttu-id="9b557-1793">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="9b557-1793">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1794">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1794">ACS</span></span>

* <span data-ttu-id="9b557-1795">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="9b557-1795">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="9b557-1796">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1796">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="9b557-1797">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9b557-1797">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="9b557-1798">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-1798">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="9b557-1799">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="9b557-1799">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="9b557-1800">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="9b557-1800">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="9b557-1801">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9b557-1801">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="9b557-1802">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="9b557-1802">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1803">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1803">Appservice</span></span>

* <span data-ttu-id="9b557-1804">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="9b557-1804">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="9b557-1805">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="9b557-1805">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-1806">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-1806">CDN</span></span>

* <span data-ttu-id="9b557-1807">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1807">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1808">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1808">Container</span></span>

* <span data-ttu-id="9b557-1809">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="9b557-1809">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="9b557-1810">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1810">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-1811">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-1811">CosmosDB</span></span>

* <span data-ttu-id="9b557-1812">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="9b557-1812">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-1813">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-1813">Extension</span></span>

* <span data-ttu-id="9b557-1814">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1814">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="9b557-1815">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1815">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="9b557-1816">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9b557-1816">Feedback</span></span>

* <span data-ttu-id="9b557-1817">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9b557-1817">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1818">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1818">Interactive</span></span>

* <span data-ttu-id="9b557-1819">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9b557-1819">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="9b557-1820">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="9b557-1820">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1821">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1821">IoT</span></span>

* <span data-ttu-id="9b557-1822">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9b557-1822">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9b557-1823">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9b557-1823">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9b557-1824">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1824">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="9b557-1825">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="9b557-1825">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1826">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1826">Monitor</span></span>

* <span data-ttu-id="9b557-1827">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1827">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1828">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1828">Network</span></span>

* <span data-ttu-id="9b557-1829">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9b557-1829">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="9b557-1830">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1830">Profile</span></span>

* <span data-ttu-id="9b557-1831">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="9b557-1831">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1832">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1832">Resource</span></span>

* <span data-ttu-id="9b557-1833">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1833">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1834">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1834">Role</span></span>

* <span data-ttu-id="9b557-1835">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1835">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1836">SQL</span></span>

* <span data-ttu-id="9b557-1837">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="9b557-1837">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="9b557-1838">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="9b557-1838">Added `sql db rename`</span></span>
* <span data-ttu-id="9b557-1839">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="9b557-1839">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1840">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1840">Storage</span></span>

* <span data-ttu-id="9b557-1841">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="9b557-1841">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1842">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1842">VM</span></span>

* <span data-ttu-id="9b557-1843">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="9b557-1843">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="9b557-1844">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="9b557-1844">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="9b557-1845">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="9b557-1845">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="9b557-1846">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1846">January 31, 2018</span></span>

<span data-ttu-id="9b557-1847">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="9b557-1847">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1848">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1848">Core</span></span>

* <span data-ttu-id="9b557-1849">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="9b557-1849">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="9b557-1850">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-1850">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="9b557-1851">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="9b557-1851">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="9b557-1852">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="9b557-1852">Use `--verbose` to see</span></span>
* <span data-ttu-id="9b557-1853">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="9b557-1853">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1854">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1854">ACS</span></span>

* <span data-ttu-id="9b557-1855">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="9b557-1855">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="9b557-1856">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="9b557-1856">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1857">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1857">Appservice</span></span>

* <span data-ttu-id="9b557-1858">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="9b557-1858">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="9b557-1859">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="9b557-1859">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-1860">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-1860">CDN</span></span>

* <span data-ttu-id="9b557-1861">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1861">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-1862">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-1862">CosmosDB</span></span>

* <span data-ttu-id="9b557-1863">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="9b557-1863">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1864">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1864">Interactive</span></span>

* <span data-ttu-id="9b557-1865">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="9b557-1865">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1866">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1866">Network</span></span>

* <span data-ttu-id="9b557-1867">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1867">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="9b557-1868">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1868">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="9b557-1869">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1869">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="9b557-1870">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1870">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="9b557-1871">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="9b557-1871">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="9b557-1872">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="9b557-1872">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="9b557-1873">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="9b557-1873">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="9b557-1874">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="9b557-1874">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="9b557-1875">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9b557-1875">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="9b557-1876">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="9b557-1876">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-1877">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1877">Profile</span></span>

* <span data-ttu-id="9b557-1878">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="9b557-1878">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1879">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1879">Resource</span></span>

* <span data-ttu-id="9b557-1880">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="9b557-1880">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1881">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1881">Storage</span></span>

* <span data-ttu-id="9b557-1882">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="9b557-1882">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="9b557-1883">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="9b557-1883">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="9b557-1884">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-1884">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="9b557-1885">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1885">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="9b557-1886">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="9b557-1886">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1887">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1887">VM</span></span>

* <span data-ttu-id="9b557-1888">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="9b557-1888">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="9b557-1889">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="9b557-1889">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="9b557-1890">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="9b557-1890">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="9b557-1891">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1891">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="9b557-1892">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="9b557-1892">January 17, 2018</span></span>

<span data-ttu-id="9b557-1893">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="9b557-1893">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-1894">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-1894">ACR</span></span>

* <span data-ttu-id="9b557-1895">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-1895">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="9b557-1896">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="9b557-1896">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1897">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1897">ACS</span></span>

* <span data-ttu-id="9b557-1898">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9b557-1898">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="9b557-1899">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="9b557-1899">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1900">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1900">Appservice</span></span>

* <span data-ttu-id="9b557-1901">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="9b557-1901">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="9b557-1902">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="9b557-1902">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="9b557-1903">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="9b557-1903">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="9b557-1904">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9b557-1904">Backup</span></span>

* <span data-ttu-id="9b557-1905">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="9b557-1905">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="9b557-1906">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="9b557-1906">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="9b557-1907">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-1907">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="9b557-1908">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="9b557-1908">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="9b557-1909">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1909">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-1910">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-1910">Batch</span></span>

* <span data-ttu-id="9b557-1911">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="9b557-1911">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="9b557-1912">Cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-1912">Cloud</span></span>

* <span data-ttu-id="9b557-1913">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-1913">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-1914">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-1914">Consumption</span></span>

* <span data-ttu-id="9b557-1915">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="9b557-1915">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="9b557-1916">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9b557-1916">Event Grid</span></span>

* <span data-ttu-id="9b557-1917">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9b557-1917">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9b557-1918">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9b557-1918">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9b557-1919">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="9b557-1919">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="9b557-1920">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="9b557-1920">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="9b557-1921">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1921">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="9b557-1922">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1922">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="9b557-1923">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="9b557-1923">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="9b557-1924">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="9b557-1924">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-1925">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-1925">Interactive</span></span>

* <span data-ttu-id="9b557-1926">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="9b557-1926">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="9b557-1927">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="9b557-1927">Fixed errors on startup</span></span>
* <span data-ttu-id="9b557-1928">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="9b557-1928">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-1929">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1929">IoT</span></span>

* <span data-ttu-id="9b557-1930">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="9b557-1930">Added support for device provisioning service</span></span>
* <span data-ttu-id="9b557-1931">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1931">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="9b557-1932">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-1932">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1933">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1933">Monitor</span></span>

* <span data-ttu-id="9b557-1934">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="9b557-1934">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="9b557-1935">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1935">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="9b557-1936">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="9b557-1936">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1937">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1937">Network</span></span>

* <span data-ttu-id="9b557-1938">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1938">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="9b557-1939">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1939">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-1940">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-1940">Profile</span></span>

* <span data-ttu-id="9b557-1941">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1941">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1942">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1942">Role</span></span>

* <span data-ttu-id="9b557-1943">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="9b557-1943">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9b557-1944">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9b557-1944">Service Fabric</span></span>

* <span data-ttu-id="9b557-1945">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="9b557-1945">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="9b557-1946">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-1946">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1947">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1947">VM</span></span>

* <span data-ttu-id="9b557-1948">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="9b557-1948">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="9b557-1949">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="9b557-1949">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="9b557-1950">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="9b557-1950">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="9b557-1951">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="9b557-1951">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="9b557-1952">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="9b557-1952">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="9b557-1953">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1953">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9b557-1954">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1954">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="9b557-1955">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="9b557-1955">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="9b557-1956">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-1956">December 19, 2017</span></span>

<span data-ttu-id="9b557-1957">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="9b557-1957">Version 2.0.23</span></span>

* <span data-ttu-id="9b557-1958">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9b557-1958">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1959">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1959">Container</span></span>

* <span data-ttu-id="9b557-1960">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1960">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="9b557-1961">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-1961">Network</span></span>

* <span data-ttu-id="9b557-1962">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1962">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="9b557-1963">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-1963">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-1964">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-1964">Storage</span></span>

* <span data-ttu-id="9b557-1965">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="9b557-1965">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-1966">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-1966">VM</span></span>

* <span data-ttu-id="9b557-1967">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="9b557-1967">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="9b557-1968">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-1968">December 5, 2017</span></span>

<span data-ttu-id="9b557-1969">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="9b557-1969">Version 2.0.22</span></span>

* <span data-ttu-id="9b557-1970">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="9b557-1970">Removed `az component` commands.</span></span> <span data-ttu-id="9b557-1971">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="9b557-1971">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="9b557-1972">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-1972">Core</span></span>
* <span data-ttu-id="9b557-1973">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="9b557-1973">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="9b557-1974">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="9b557-1974">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-1975">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-1975">ACS</span></span>

* <span data-ttu-id="9b557-1976">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9b557-1976">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="9b557-1977">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="9b557-1977">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="9b557-1978">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="9b557-1978">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="9b557-1979">Advisor</span><span class="sxs-lookup"><span data-stu-id="9b557-1979">Advisor</span></span>

* <span data-ttu-id="9b557-1980">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-1980">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-1981">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-1981">Appservice</span></span>

* <span data-ttu-id="9b557-1982">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="9b557-1982">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="9b557-1983">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="9b557-1983">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="9b557-1984">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="9b557-1984">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="9b557-1985">Consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-1985">Consumption</span></span>

* <span data-ttu-id="9b557-1986">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="9b557-1986">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="9b557-1987">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-1987">Container</span></span>

* <span data-ttu-id="9b557-1988">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-1988">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-1989">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-1989">Monitor</span></span>

* <span data-ttu-id="9b557-1990">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="9b557-1990">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-1991">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-1991">Resource</span></span>

* <span data-ttu-id="9b557-1992">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="9b557-1992">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="9b557-1993">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-1993">Role</span></span>

* <span data-ttu-id="9b557-1994">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="9b557-1994">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="9b557-1995">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="9b557-1995">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="9b557-1996">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9b557-1996">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-1997">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-1997">SQL</span></span>

* <span data-ttu-id="9b557-1998">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="9b557-1998">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="9b557-1999">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="9b557-1999">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2000">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2000">VM</span></span>

* <span data-ttu-id="9b557-2001">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="9b557-2001">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="9b557-2002">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2002">November 14, 2017</span></span>

<span data-ttu-id="9b557-2003">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="9b557-2003">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-2004">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-2004">ACR</span></span>

* <span data-ttu-id="9b557-2005">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="9b557-2005">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="9b557-2006">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2006">ACS</span></span>

* <span data-ttu-id="9b557-2007">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="9b557-2007">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="9b557-2008">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2008">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="9b557-2009">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="9b557-2009">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="9b557-2010">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-2010">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="9b557-2011">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9b557-2011">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2012">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2012">Appservice</span></span>

* <span data-ttu-id="9b557-2013">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="9b557-2013">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="9b557-2014">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9b557-2014">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="9b557-2015">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9b557-2015">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="9b557-2016">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="9b557-2016">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="9b557-2017">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="9b557-2017">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="9b557-2018">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="9b557-2018">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-2019">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-2019">Batch</span></span>

* <span data-ttu-id="9b557-2020">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="9b557-2020">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-2021">Batchai</span><span class="sxs-lookup"><span data-stu-id="9b557-2021">Batchai</span></span>

* <span data-ttu-id="9b557-2022">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2022">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="9b557-2023">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2023">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="9b557-2024">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="9b557-2024">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="9b557-2025">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2025">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="9b557-2026">Cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-2026">Cloud</span></span>

* <span data-ttu-id="9b557-2027">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="9b557-2027">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="9b557-2028">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-2028">Container</span></span>

* <span data-ttu-id="9b557-2029">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="9b557-2029">Added support to open multiple ports</span></span>
* <span data-ttu-id="9b557-2030">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9b557-2030">Added container group restart policy</span></span>
* <span data-ttu-id="9b557-2031">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="9b557-2031">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="9b557-2032">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="9b557-2032">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9b557-2033">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9b557-2033">Data Lake Analytics</span></span>

* <span data-ttu-id="9b557-2034">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="9b557-2034">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9b557-2035">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2035">Data Lake Store</span></span>

* <span data-ttu-id="9b557-2036">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="9b557-2036">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-2037">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-2037">Extension</span></span>

* <span data-ttu-id="9b557-2038">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="9b557-2038">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="9b557-2039">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="9b557-2039">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-2040">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-2040">IoT</span></span>

* <span data-ttu-id="9b557-2041">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="9b557-2041">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-2042">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-2042">Monitor</span></span>

* <span data-ttu-id="9b557-2043">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="9b557-2043">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2044">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2044">Network</span></span>

* <span data-ttu-id="9b557-2045">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="9b557-2045">Added support for CAA DNS records</span></span>
* <span data-ttu-id="9b557-2046">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2046">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="9b557-2047">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9b557-2047">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="9b557-2048">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9b557-2048">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="9b557-2049">Réservations</span><span class="sxs-lookup"><span data-stu-id="9b557-2049">Reservations</span></span>

* <span data-ttu-id="9b557-2050">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-2050">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2051">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2051">Resource</span></span>

* <span data-ttu-id="9b557-2052">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="9b557-2052">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2053">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2053">SQL</span></span>

* <span data-ttu-id="9b557-2054">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2054">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2055">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2055">Storage</span></span>

* <span data-ttu-id="9b557-2056">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-2056">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="9b557-2057">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="9b557-2057">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="9b557-2058">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="9b557-2058">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="9b557-2059">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="9b557-2059">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="9b557-2060">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2060">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="9b557-2061">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="9b557-2061">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="9b557-2062">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2062">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2063">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2063">VM</span></span>

* <span data-ttu-id="9b557-2064">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="9b557-2064">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="9b557-2065">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="9b557-2065">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="9b557-2066">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="9b557-2066">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="9b557-2067">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="9b557-2067">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="9b557-2068">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9b557-2068">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="9b557-2069">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2069">October 24, 2017</span></span>

<span data-ttu-id="9b557-2070">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="9b557-2070">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="9b557-2071">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2071">Core</span></span>

* <span data-ttu-id="9b557-2072">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="9b557-2072">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-2073">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-2073">ACR</span></span>

* <span data-ttu-id="9b557-2074">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="9b557-2074">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="9b557-2075">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="9b557-2075">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="9b557-2076">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="9b557-2076">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2077">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2077">ACS</span></span>

* <span data-ttu-id="9b557-2078">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="9b557-2078">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="9b557-2079">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9b557-2079">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2080">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2080">Appservice</span></span>

* <span data-ttu-id="9b557-2081">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="9b557-2081">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="9b557-2082">Composant</span><span class="sxs-lookup"><span data-stu-id="9b557-2082">Component</span></span>

* <span data-ttu-id="9b557-2083">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="9b557-2083">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-2084">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-2084">Monitor</span></span>

* <span data-ttu-id="9b557-2085">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="9b557-2085">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2086">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2086">Resource</span></span>

* <span data-ttu-id="9b557-2087">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="9b557-2087">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="9b557-2088">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="9b557-2088">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2089">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2089">VM</span></span>

* <span data-ttu-id="9b557-2090">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2090">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="9b557-2091">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2091">October 9, 2017</span></span>

<span data-ttu-id="9b557-2092">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="9b557-2092">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="9b557-2093">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2093">Core</span></span>

* <span data-ttu-id="9b557-2094">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9b557-2094">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2095">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2095">Appservice</span></span>

* <span data-ttu-id="9b557-2096">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2096">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-2097">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-2097">Batch</span></span>

* <span data-ttu-id="9b557-2098">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="9b557-2098">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="9b557-2099">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="9b557-2099">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="9b557-2100">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-2100">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="9b557-2101">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="9b557-2101">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="9b557-2102">Batchai</span><span class="sxs-lookup"><span data-stu-id="9b557-2102">Batchai</span></span>

* <span data-ttu-id="9b557-2103">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="9b557-2103">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-2104">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-2104">Keyvault</span></span>

* <span data-ttu-id="9b557-2105">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9b557-2105">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="9b557-2106">(#4448)</span><span class="sxs-lookup"><span data-stu-id="9b557-2106">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="9b557-2107">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2107">Network</span></span>

* <span data-ttu-id="9b557-2108">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="9b557-2108">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="9b557-2109">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="9b557-2109">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2110">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2110">Resource</span></span>

* <span data-ttu-id="9b557-2111">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="9b557-2111">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="9b557-2112">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-2112">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="9b557-2113">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="9b557-2113">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="9b557-2114">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="9b557-2114">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2115">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2115">Sql</span></span>

* <span data-ttu-id="9b557-2116">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="9b557-2116">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="9b557-2117">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="9b557-2117">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="9b557-2118">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="9b557-2118">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2119">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2119">Storage</span></span>

* <span data-ttu-id="9b557-2120">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="9b557-2120">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2121">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2121">Vm</span></span>

* <span data-ttu-id="9b557-2122">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="9b557-2122">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="9b557-2123">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2123">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="9b557-2124">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9b557-2124">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="9b557-2125">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2125">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="9b557-2126">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2126">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="9b557-2127">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2127">September 22, 2017</span></span>

<span data-ttu-id="9b557-2128">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="9b557-2128">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2129">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2129">Resource</span></span>

* <span data-ttu-id="9b557-2130">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="9b557-2130">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="9b557-2131">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="9b557-2131">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="9b557-2132">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2132">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="9b557-2133">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="9b557-2133">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2134">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2134">Network</span></span>

* <span data-ttu-id="9b557-2135">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="9b557-2135">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="9b557-2136">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="9b557-2136">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="9b557-2137">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="9b557-2137">Added `asg` application security group commands</span></span>
* <span data-ttu-id="9b557-2138">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2138">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="9b557-2139">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2139">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9b557-2140">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2140">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="9b557-2141">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2141">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2142">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2142">Storage</span></span>

* <span data-ttu-id="9b557-2143">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9b557-2143">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9b557-2144">Événement</span><span class="sxs-lookup"><span data-stu-id="9b557-2144">Eventgrid</span></span>

* <span data-ttu-id="9b557-2145">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="9b557-2145">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2146">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2146">SQL</span></span>

* <span data-ttu-id="9b557-2147">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="9b557-2147">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="9b557-2148">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="9b557-2148">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="9b557-2149">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2149">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-2150">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-2150">Keyvault</span></span>

* <span data-ttu-id="9b557-2151">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="9b557-2151">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2152">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2152">VM</span></span>

* <span data-ttu-id="9b557-2153">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2153">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="9b557-2154">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="9b557-2154">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="9b557-2155">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2155">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="9b557-2156">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="9b557-2156">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="9b557-2157">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="9b557-2157">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="9b557-2158">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9b557-2158">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2159">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2159">ACS</span></span>

* <span data-ttu-id="9b557-2160">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-2160">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2161">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2161">Appservice</span></span>

* <span data-ttu-id="9b557-2162">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2162">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9b557-2163">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9b557-2163">Backup</span></span>

* <span data-ttu-id="9b557-2164">Préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-2164">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="9b557-2165">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2165">September 11, 2017</span></span>

<span data-ttu-id="9b557-2166">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="9b557-2166">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="9b557-2167">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2167">Core</span></span>

* <span data-ttu-id="9b557-2168">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="9b557-2168">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="9b557-2169">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="9b557-2169">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2170">Acs</span><span class="sxs-lookup"><span data-stu-id="9b557-2170">Acs</span></span>

* <span data-ttu-id="9b557-2171">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="9b557-2171">Added `acs list-locations` command</span></span>
* <span data-ttu-id="9b557-2172">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="9b557-2172">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2173">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2173">Appservice</span></span>

* <span data-ttu-id="9b557-2174">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="9b557-2174">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-2175">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-2175">CDN</span></span>

* <span data-ttu-id="9b557-2176">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2176">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="9b557-2177">Extension</span><span class="sxs-lookup"><span data-stu-id="9b557-2177">Extension</span></span>

* <span data-ttu-id="9b557-2178">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-2178">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-2179">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-2179">Keyvault</span></span>

* <span data-ttu-id="9b557-2180">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="9b557-2180">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2181">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2181">Network</span></span>

* <span data-ttu-id="9b557-2182">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9b557-2182">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9b557-2183">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2183">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="9b557-2184">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2184">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="9b557-2185">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2185">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9b557-2186">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2186">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2187">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2187">Resource</span></span>

* <span data-ttu-id="9b557-2188">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2188">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="9b557-2189">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2189">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="9b557-2190">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="9b557-2190">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="9b557-2191">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="9b557-2191">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2192">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2192">SQL</span></span>

* <span data-ttu-id="9b557-2193">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-2193">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2194">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2194">VM</span></span>

* <span data-ttu-id="9b557-2195">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="9b557-2195">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="9b557-2196">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="9b557-2196">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="9b557-2197">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2197">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="9b557-2198">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="9b557-2198">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="9b557-2199">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="9b557-2199">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="9b557-2200">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2200">August 31, 2017</span></span>

<span data-ttu-id="9b557-2201">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="9b557-2201">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-2202">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-2202">Keyvault</span></span>

* <span data-ttu-id="9b557-2203">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="9b557-2203">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="9b557-2204">Sf</span><span class="sxs-lookup"><span data-stu-id="9b557-2204">Sf</span></span>

* <span data-ttu-id="9b557-2205">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="9b557-2205">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2206">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2206">Storage</span></span>

* <span data-ttu-id="9b557-2207">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="9b557-2207">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="9b557-2208">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="9b557-2208">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="9b557-2209">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2209">August 28, 2017</span></span>

<span data-ttu-id="9b557-2210">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="9b557-2210">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="9b557-2211">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9b557-2211">CLI</span></span>

* <span data-ttu-id="9b557-2212">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="9b557-2212">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2213">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2213">ACS</span></span>

* <span data-ttu-id="9b557-2214">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="9b557-2214">Corrected preview regions</span></span>
* <span data-ttu-id="9b557-2215">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-2215">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="9b557-2216">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2216">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2217">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2217">Appservice</span></span>

* <span data-ttu-id="9b557-2218">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2218">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="9b557-2219">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-2219">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="9b557-2220">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="9b557-2220">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="9b557-2221">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="9b557-2221">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="9b557-2222">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-2222">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-2223">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-2223">IoT</span></span>

* <span data-ttu-id="9b557-2224">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="9b557-2224">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2225">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2225">Network</span></span>

* <span data-ttu-id="9b557-2226">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9b557-2226">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9b557-2227">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2227">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="9b557-2228">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9b557-2228">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9b557-2229">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2229">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9b557-2230">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2230">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-2231">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-2231">Profile</span></span>

* <span data-ttu-id="9b557-2232">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2232">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9b557-2233">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9b557-2233">Service Fabric</span></span>

* <span data-ttu-id="9b557-2234">Préversion</span><span class="sxs-lookup"><span data-stu-id="9b557-2234">Preview release</span></span>
* <span data-ttu-id="9b557-2235">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="9b557-2235">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="9b557-2236">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="9b557-2236">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="9b557-2237">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="9b557-2237">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2238">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2238">Storage</span></span>

* <span data-ttu-id="9b557-2239">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="9b557-2239">Enabled setting blob tier</span></span>
* <span data-ttu-id="9b557-2240">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="9b557-2240">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="9b557-2241">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="9b557-2241">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="9b557-2242">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="9b557-2242">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="9b557-2243">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2243">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="9b557-2244">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="9b557-2244">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2245">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2245">VM</span></span>

* <span data-ttu-id="9b557-2246">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="9b557-2246">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="9b557-2247">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="9b557-2247">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="9b557-2248">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2248">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="9b557-2249">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="9b557-2249">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="9b557-2250">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="9b557-2250">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="9b557-2251">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2251">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="9b557-2252">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2252">August 15, 2017</span></span>

<span data-ttu-id="9b557-2253">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="9b557-2253">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2254">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2254">ACS</span></span>

* <span data-ttu-id="9b557-2255">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="9b557-2255">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2256">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2256">Appservice</span></span>

* <span data-ttu-id="9b557-2257">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="9b557-2257">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="9b557-2258">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9b557-2258">Event Grid</span></span>

* <span data-ttu-id="9b557-2259">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9b557-2259">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="9b557-2260">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2260">August 11, 2017</span></span>

<span data-ttu-id="9b557-2261">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="9b557-2261">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2262">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2262">ACS</span></span>

* <span data-ttu-id="9b557-2263">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="9b557-2263">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-2264">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-2264">Batch</span></span>

* <span data-ttu-id="9b557-2265">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="9b557-2265">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="9b557-2266">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="9b557-2266">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="9b557-2267">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="9b557-2267">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="9b557-2268">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="9b557-2268">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="9b557-2269">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="9b557-2269">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="9b557-2270">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="9b557-2270">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="9b557-2271">Composant</span><span class="sxs-lookup"><span data-stu-id="9b557-2271">Component</span></span>

* <span data-ttu-id="9b557-2272">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="9b557-2272">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="9b557-2273">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-2273">Container</span></span>

* <span data-ttu-id="9b557-2274">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="9b557-2274">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="9b557-2275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2275">Data Lake Store</span></span>

* <span data-ttu-id="9b557-2276">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="9b557-2276">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="9b557-2277">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9b557-2277">Event Grid</span></span>

* <span data-ttu-id="9b557-2278">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9b557-2278">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2279">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2279">Network</span></span>

* <span data-ttu-id="9b557-2280">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="9b557-2280">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="9b557-2281">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="9b557-2281">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="9b557-2282">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="9b557-2282">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="9b557-2283">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="9b557-2283">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-2284">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-2284">Profile</span></span>

* <span data-ttu-id="9b557-2285">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="9b557-2285">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2286">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2286">Storage</span></span>

* <span data-ttu-id="9b557-2287">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="9b557-2287">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2288">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2288">VM</span></span>

* <span data-ttu-id="9b557-2289">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="9b557-2289">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="9b557-2290">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="9b557-2290">Exposed `list-skus` command</span></span>
* <span data-ttu-id="9b557-2291">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="9b557-2291">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="9b557-2292">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="9b557-2292">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="9b557-2293">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="9b557-2293">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="9b557-2294">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2294">July 28, 2017</span></span>

<span data-ttu-id="9b557-2295">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="9b557-2295">Version 2.0.12</span></span>

* <span data-ttu-id="9b557-2296">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="9b557-2296">Added container commands</span></span>
* <span data-ttu-id="9b557-2297">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="9b557-2297">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="9b557-2298">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2298">Core</span></span>

* <span data-ttu-id="9b557-2299">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="9b557-2299">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="9b557-2300">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="9b557-2300">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="9b557-2301">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9b557-2301">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="9b557-2302">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="9b557-2302">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="9b557-2303">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="9b557-2303">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="9b557-2304">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="9b557-2304">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="9b557-2305">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="9b557-2305">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9b557-2306">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="9b557-2306">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="9b557-2307">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="9b557-2307">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="9b557-2308">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9b557-2308">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="9b557-2309">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="9b557-2309">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="9b557-2310">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="9b557-2310">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="9b557-2311">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-2311">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="9b557-2312">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="9b557-2312">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="9b557-2313">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9b557-2313">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="9b557-2314">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="9b557-2314">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="9b557-2315">ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-2315">ACR</span></span>

* <span data-ttu-id="9b557-2316">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="9b557-2316">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="9b557-2317">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="9b557-2317">Support SKU update for managed registries</span></span>
* <span data-ttu-id="9b557-2318">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="9b557-2318">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="9b557-2319">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="9b557-2319">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="9b557-2320">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="9b557-2320">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="9b557-2321">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="9b557-2321">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2322">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2322">ACS</span></span>

* <span data-ttu-id="9b557-2323">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="9b557-2323">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2324">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2324">Appservice</span></span>

* <span data-ttu-id="9b557-2325">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="9b557-2325">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="9b557-2326">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="9b557-2326">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="9b557-2327">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="9b557-2327">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="9b557-2328">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="9b557-2328">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="9b557-2329">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="9b557-2329">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="9b557-2330">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="9b557-2330">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="9b557-2331">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="9b557-2331">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="9b557-2332">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="9b557-2332">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="9b557-2333">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="9b557-2333">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="9b557-2334">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="9b557-2334">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="9b557-2335">Batch</span><span class="sxs-lookup"><span data-stu-id="9b557-2335">Batch</span></span>

* <span data-ttu-id="9b557-2336">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="9b557-2336">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="9b557-2337">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="9b557-2337">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="9b557-2338">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="9b557-2338">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="9b557-2339">CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-2339">CDN</span></span>

* <span data-ttu-id="9b557-2340">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="9b557-2340">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="9b557-2341">Cloud</span><span class="sxs-lookup"><span data-stu-id="9b557-2341">Cloud</span></span>

* <span data-ttu-id="9b557-2342">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="9b557-2342">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="9b557-2343">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="9b557-2343">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="9b557-2344">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="9b557-2344">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="9b557-2345">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="9b557-2345">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="9b557-2346">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="9b557-2346">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-2347">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-2347">CosmosDB</span></span>

* <span data-ttu-id="9b557-2348">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="9b557-2348">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="9b557-2349">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="9b557-2349">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9b557-2350">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9b557-2350">Data Lake Analytics</span></span>

* <span data-ttu-id="9b557-2351">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="9b557-2351">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="9b557-2352">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="9b557-2352">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="9b557-2353">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="9b557-2353">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9b557-2354">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2354">Data Lake Store</span></span>

* <span data-ttu-id="9b557-2355">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2355">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="9b557-2356">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="9b557-2356">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="9b557-2357">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="9b557-2357">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="9b557-2358">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2358">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="9b557-2359">Interactive</span><span class="sxs-lookup"><span data-stu-id="9b557-2359">Interactive</span></span>

* <span data-ttu-id="9b557-2360">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="9b557-2360">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="9b557-2361">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="9b557-2361">Increased test coverage</span></span>
* <span data-ttu-id="9b557-2362">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="9b557-2362">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="9b557-2363">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="9b557-2363">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="9b557-2364">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="9b557-2364">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="9b557-2365">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="9b557-2365">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="9b557-2366">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="9b557-2366">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9b557-2367">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="9b557-2367">Added `--progress` flag</span></span>
* <span data-ttu-id="9b557-2368">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="9b557-2368">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="9b557-2369">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="9b557-2369">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="9b557-2370">IoT</span><span class="sxs-lookup"><span data-stu-id="9b557-2370">IoT</span></span>

* <span data-ttu-id="9b557-2371">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="9b557-2371">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="9b557-2372">(#3934)</span><span class="sxs-lookup"><span data-stu-id="9b557-2372">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="9b557-2373">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="9b557-2373">Key vault</span></span>

* <span data-ttu-id="9b557-2374">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="9b557-2374">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="9b557-2375">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9b557-2375">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="9b557-2376">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9b557-2376">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9b557-2377">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9b557-2377">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9b557-2378">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9b557-2378">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="9b557-2379">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="9b557-2379">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="9b557-2380">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="9b557-2380">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="9b557-2381">(#3307)</span><span class="sxs-lookup"><span data-stu-id="9b557-2381">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="9b557-2382">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2382">Lab</span></span>

* <span data-ttu-id="9b557-2383">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="9b557-2383">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="9b557-2384">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="9b557-2384">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-2385">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-2385">Monitor</span></span>

* <span data-ttu-id="9b557-2386">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="9b557-2386">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="9b557-2387">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="9b557-2387">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="9b557-2388">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="9b557-2388">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="9b557-2389">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="9b557-2389">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="9b557-2390">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="9b557-2390">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="9b557-2391">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="9b557-2391">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="9b557-2392">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="9b557-2392">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="9b557-2393">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="9b557-2393">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="9b557-2394">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="9b557-2394">`location` no longer required</span></span>
  * <span data-ttu-id="9b557-2395">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="9b557-2395">Add name and ID support for target</span></span>
  * <span data-ttu-id="9b557-2396">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-2396">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="9b557-2397">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="9b557-2397">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="9b557-2398">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="9b557-2398">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="9b557-2399">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="9b557-2399">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="9b557-2400">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="9b557-2400">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="9b557-2401">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2401">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2402">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2402">Network</span></span>

* <span data-ttu-id="9b557-2403">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="9b557-2403">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="9b557-2404">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2404">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="9b557-2405">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="9b557-2405">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="9b557-2406">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="9b557-2406">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="9b557-2407">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2407">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="9b557-2408">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9b557-2408">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="9b557-2409">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="9b557-2409">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="9b557-2410">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="9b557-2410">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="9b557-2411">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="9b557-2411">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="9b557-2412">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9b557-2412">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="9b557-2413">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2413">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="9b557-2414">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="9b557-2414">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="9b557-2415">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="9b557-2415">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="9b557-2416">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2416">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="9b557-2417">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2417">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="9b557-2418">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2418">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="9b557-2419">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="9b557-2419">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="9b557-2420">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9b557-2420">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="9b557-2421">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2421">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="9b557-2422">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2422">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="9b557-2423">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2423">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="9b557-2424">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-2424">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="9b557-2425">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="9b557-2425">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="9b557-2426">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9b557-2426">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="9b557-2427">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9b557-2427">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="9b557-2428">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9b557-2428">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="9b557-2429">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9b557-2429">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-2430">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-2430">Profile</span></span>

* <span data-ttu-id="9b557-2431">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="9b557-2431">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="9b557-2432">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9b557-2432">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="9b557-2433">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="9b557-2433">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="9b557-2434">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="9b557-2434">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="9b557-2435">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="9b557-2435">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="9b557-2436">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9b557-2436">RDBMS</span></span>

* <span data-ttu-id="9b557-2437">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="9b557-2437">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="9b557-2438">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="9b557-2438">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="9b557-2439">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="9b557-2439">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="9b557-2440">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="9b557-2440">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2441">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2441">Resource</span></span>

* <span data-ttu-id="9b557-2442">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2442">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="9b557-2443">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9b557-2443">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="9b557-2444">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9b557-2444">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="9b557-2445">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="9b557-2445">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="9b557-2446">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="9b557-2446">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="9b557-2447">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="9b557-2447">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="9b557-2448">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="9b557-2448">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="9b557-2449">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9b557-2449">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="9b557-2450">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-2450">Role</span></span>

* <span data-ttu-id="9b557-2451">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9b557-2451">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="9b557-2452">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="9b557-2452">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="9b557-2453">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="9b557-2453">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="9b557-2454">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="9b557-2454">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="9b557-2455">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="9b557-2455">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9b557-2456">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9b557-2456">Service Fabric</span></span>
* <span data-ttu-id="9b557-2457">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="9b557-2457">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="9b557-2458">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="9b557-2458">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="9b557-2459">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="9b557-2459">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2460">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2460">SQL</span></span>

* <span data-ttu-id="9b557-2461">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="9b557-2461">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="9b557-2462">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="9b557-2462">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="9b557-2463">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="9b557-2463">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2464">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2464">Storage</span></span>

* <span data-ttu-id="9b557-2465">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="9b557-2465">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="9b557-2466">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="9b557-2466">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="9b557-2467">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="9b557-2467">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="9b557-2468">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="9b557-2468">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="9b557-2469">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="9b557-2469">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="9b557-2470">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="9b557-2470">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2471">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2471">VM</span></span>

* <span data-ttu-id="9b557-2472">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2472">Support configuring nsg</span></span>
* <span data-ttu-id="9b557-2473">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="9b557-2473">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="9b557-2474">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="9b557-2474">Support managed service identities</span></span>
* <span data-ttu-id="9b557-2475">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="9b557-2475">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="9b557-2476">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="9b557-2476">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="9b557-2477">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2477">May 10, 2017</span></span>

<span data-ttu-id="9b557-2478">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="9b557-2478">Version 2.0.6</span></span>

* <span data-ttu-id="9b557-2479">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9b557-2479">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="9b557-2480">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="9b557-2480">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="9b557-2481">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2481">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="9b557-2482">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9b557-2482">Include Cognitive Services module</span></span>
* <span data-ttu-id="9b557-2483">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9b557-2483">Include Service Fabric module</span></span>
* <span data-ttu-id="9b557-2484">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="9b557-2484">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="9b557-2485">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="9b557-2485">Add support for CDN commands</span></span>
* <span data-ttu-id="9b557-2486">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="9b557-2486">Remove Container module</span></span>
* <span data-ttu-id="9b557-2487">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="9b557-2487">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="9b557-2488">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="9b557-2488">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="9b557-2489">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2489">Core</span></span>

* <span data-ttu-id="9b557-2490">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="9b557-2490">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="9b557-2491">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="9b557-2491">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="9b557-2492">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="9b557-2492">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="9b557-2493">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="9b557-2493">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="9b557-2494">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="9b557-2494">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="9b557-2495">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="9b557-2495">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="9b557-2496">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="9b557-2496">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="9b557-2497">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="9b557-2497">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="9b557-2498">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="9b557-2498">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="9b557-2499">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="9b557-2499">core: Improved performance</span></span>
* <span data-ttu-id="9b557-2500">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="9b557-2500">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="9b557-2501">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="9b557-2501">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2502">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2502">ACS</span></span>

* <span data-ttu-id="9b557-2503">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="9b557-2503">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="9b557-2504">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="9b557-2504">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="9b557-2505">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="9b557-2505">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="9b557-2506">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="9b557-2506">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2507">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2507">AppService</span></span>

* <span data-ttu-id="9b557-2508">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="9b557-2508">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="9b557-2509">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="9b557-2509">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="9b557-2510">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="9b557-2510">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="9b557-2511">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="9b557-2511">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="9b557-2512">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="9b557-2512">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="9b557-2513">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="9b557-2513">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="9b557-2514">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="9b557-2514">support slot swap with preview</span></span>
* <span data-ttu-id="9b557-2515">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="9b557-2515">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="9b557-2516">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="9b557-2516">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9b557-2517">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9b557-2517">CosmosDB</span></span>

* <span data-ttu-id="9b557-2518">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9b557-2518">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="9b557-2519">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="9b557-2519">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="9b557-2520">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="9b557-2520">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="9b557-2521">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="9b557-2521">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9b557-2522">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9b557-2522">Data Lake Analytics</span></span>

* <span data-ttu-id="9b557-2523">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="9b557-2523">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="9b557-2524">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="9b557-2524">Add support for new catalog item type: package.</span></span> <span data-ttu-id="9b557-2525">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="9b557-2525">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="9b557-2526">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="9b557-2526">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="9b557-2527">Table</span><span class="sxs-lookup"><span data-stu-id="9b557-2527">Table</span></span>
  * <span data-ttu-id="9b557-2528">Fonction table</span><span class="sxs-lookup"><span data-stu-id="9b557-2528">Table valued function</span></span>
  * <span data-ttu-id="9b557-2529">Affichage</span><span class="sxs-lookup"><span data-stu-id="9b557-2529">View</span></span>
  * <span data-ttu-id="9b557-2530">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="9b557-2530">Table Statistics.</span></span> <span data-ttu-id="9b557-2531">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="9b557-2531">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9b557-2532">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2532">Data Lake Store</span></span>

* <span data-ttu-id="9b557-2533">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="9b557-2533">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="9b557-2534">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="9b557-2534">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="9b557-2535">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="9b557-2535">missed help for access show.</span></span> <span data-ttu-id="9b557-2536">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="9b557-2536">adding it.</span></span> <span data-ttu-id="9b557-2537">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="9b557-2537">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="9b557-2538">Rechercher</span><span class="sxs-lookup"><span data-stu-id="9b557-2538">Find</span></span>

* <span data-ttu-id="9b557-2539">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="9b557-2539">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="9b557-2540">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9b557-2540">KeyVault</span></span>

* <span data-ttu-id="9b557-2541">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="9b557-2541">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="9b557-2542">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="9b557-2542">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="9b557-2543">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="9b557-2543">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="9b557-2544">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="9b557-2544">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="9b557-2545">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="9b557-2545">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="9b557-2546">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2546">Lab</span></span>

* <span data-ttu-id="9b557-2547">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2547">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="9b557-2548">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2548">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="9b557-2549">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2549">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="9b557-2550">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2550">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="9b557-2551">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="9b557-2551">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="9b557-2552">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9b557-2552">Monitor</span></span>

* <span data-ttu-id="9b557-2553">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="9b557-2553">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="9b557-2554">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="9b557-2554">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="9b557-2555">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2555">Network</span></span>

* <span data-ttu-id="9b557-2556">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="9b557-2556">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="9b557-2557">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2557">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="9b557-2558">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9b557-2558">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="9b557-2559">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9b557-2559">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="9b557-2560">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9b557-2560">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="9b557-2561">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9b557-2561">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="9b557-2562">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="9b557-2562">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="9b557-2563">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="9b557-2563">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="9b557-2564">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="9b557-2564">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="9b557-2565">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="9b557-2565">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="9b557-2566">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="9b557-2566">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="9b557-2567">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2567">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="9b557-2568">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-2568">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="9b557-2569">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="9b557-2569">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="9b557-2570">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9b557-2570">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="9b557-2571">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="9b557-2571">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="9b557-2572">Profil</span><span class="sxs-lookup"><span data-stu-id="9b557-2572">Profile</span></span>

* <span data-ttu-id="9b557-2573">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="9b557-2573">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="9b557-2574">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="9b557-2574">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="9b557-2575">Redis</span><span class="sxs-lookup"><span data-stu-id="9b557-2575">Redis</span></span>

* <span data-ttu-id="9b557-2576">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="9b557-2576">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="9b557-2577">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="9b557-2577">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="9b557-2578">Ressource</span><span class="sxs-lookup"><span data-stu-id="9b557-2578">Resource</span></span>

* <span data-ttu-id="9b557-2579">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="9b557-2579">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="9b557-2580">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="9b557-2580">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="9b557-2581">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="9b557-2581">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="9b557-2582">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="9b557-2582">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="9b557-2583">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="9b557-2583">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="9b557-2584">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="9b557-2584">Add docs for az lock update.</span></span> <span data-ttu-id="9b557-2585">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="9b557-2585">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="9b557-2586">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="9b557-2586">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="9b557-2587">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="9b557-2587">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="9b557-2588">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="9b557-2588">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="9b557-2589">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="9b557-2589">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="9b557-2590">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="9b557-2590">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="9b557-2591">Role</span><span class="sxs-lookup"><span data-stu-id="9b557-2591">Role</span></span>

* <span data-ttu-id="9b557-2592">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="9b557-2592">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="9b557-2593">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="9b557-2593">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="9b557-2594">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="9b557-2594">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="9b557-2595">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="9b557-2595">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="9b557-2596">SQL</span><span class="sxs-lookup"><span data-stu-id="9b557-2596">SQL</span></span>

* <span data-ttu-id="9b557-2597">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="9b557-2597">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="9b557-2598">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="9b557-2598">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="9b557-2599">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2599">Storage</span></span>

* <span data-ttu-id="9b557-2600">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="9b557-2600">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="9b557-2601">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="9b557-2601">Add support for incremental blob copy</span></span>
* <span data-ttu-id="9b557-2602">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="9b557-2602">Add support for large block blob upload</span></span>
* <span data-ttu-id="9b557-2603">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="9b557-2603">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2604">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2604">VM</span></span>

* <span data-ttu-id="9b557-2605">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="9b557-2605">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="9b557-2606">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="9b557-2606">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="9b557-2607">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="9b557-2607">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="9b557-2608">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="9b557-2608">az vm/vmss disk</span></span>
  3. <span data-ttu-id="9b557-2609">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="9b557-2609">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="9b557-2610">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="9b557-2610">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="9b557-2611">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="9b557-2611">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="9b557-2612">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2612">April 3, 2017</span></span>

<span data-ttu-id="9b557-2613">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="9b557-2613">Version 2.0.2</span></span>

<span data-ttu-id="9b557-2614">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="9b557-2614">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="9b557-2615">Core</span><span class="sxs-lookup"><span data-stu-id="9b557-2615">Core</span></span>

* <span data-ttu-id="9b557-2616">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-2616">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="9b557-2617">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="9b557-2617">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="9b557-2618">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="9b557-2618">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="9b557-2619">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9b557-2619">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9b557-2620">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="9b557-2620">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="9b557-2621">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="9b557-2621">Add prompting for missing template parameters.</span></span> <span data-ttu-id="9b557-2622">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="9b557-2622">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="9b557-2623">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="9b557-2623">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="9b557-2624">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="9b557-2624">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="9b557-2625">ACS</span><span class="sxs-lookup"><span data-stu-id="9b557-2625">ACS</span></span>

* <span data-ttu-id="9b557-2626">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="9b557-2626">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="9b557-2627">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="9b557-2627">Add support for ssh key password prompting.</span></span> <span data-ttu-id="9b557-2628">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="9b557-2628">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="9b557-2629">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="9b557-2629">Add support for windows clusters.</span></span> <span data-ttu-id="9b557-2630">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="9b557-2630">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="9b557-2631">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="9b557-2631">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="9b557-2632">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="9b557-2632">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="9b557-2633">AppService</span><span class="sxs-lookup"><span data-stu-id="9b557-2633">AppService</span></span>

* <span data-ttu-id="9b557-2634">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="9b557-2634">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="9b557-2635">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="9b557-2635">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="9b557-2636">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="9b557-2636">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="9b557-2637">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="9b557-2637">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="9b557-2638">DataLake</span><span class="sxs-lookup"><span data-stu-id="9b557-2638">DataLake</span></span>

* <span data-ttu-id="9b557-2639">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9b557-2639">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="9b557-2640">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9b557-2640">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="9b557-2641">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="9b557-2641">DocuemntDB</span></span>

* <span data-ttu-id="9b557-2642">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="9b557-2642">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="9b557-2643">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9b557-2643">VM</span></span>

* <span data-ttu-id="9b557-2644">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="9b557-2644">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="9b557-2645">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="9b557-2645">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="9b557-2646">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="9b557-2646">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="9b557-2647">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9b557-2647">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9b557-2648">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="9b557-2648">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="9b557-2649">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="9b557-2649">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="9b557-2650">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="9b557-2650">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="9b557-2651">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="9b557-2651">February 27, 2017</span></span>

<span data-ttu-id="9b557-2652">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="9b557-2652">Version 2.0.0</span></span>

<span data-ttu-id="9b557-2653">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="9b557-2653">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="9b557-2654">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="9b557-2654">Container Service (acs)</span></span>
- <span data-ttu-id="9b557-2655">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="9b557-2655">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="9b557-2656">Réseau</span><span class="sxs-lookup"><span data-stu-id="9b557-2656">Networking</span></span>
- <span data-ttu-id="9b557-2657">Stockage</span><span class="sxs-lookup"><span data-stu-id="9b557-2657">Storage</span></span>

<span data-ttu-id="9b557-2658">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9b557-2658">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="9b557-2659">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="9b557-2659">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="9b557-2660">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="9b557-2660">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="9b557-2661">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="9b557-2661">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="9b557-2662">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="9b557-2662">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="9b557-2663">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="9b557-2663">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="9b557-2664">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="9b557-2664">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="9b557-2665">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="9b557-2665">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="9b557-2666">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9b557-2666">Provide feedback from the command line with the `az feedback` command</span></span>

