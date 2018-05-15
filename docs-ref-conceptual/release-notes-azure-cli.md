---
title: Notes de publication d’Azure CLI 2.0
description: En savoir plus sur les dernières mises à jour d’Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 254c7b306440d921cef6b611268839150fdf3196
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="55e40-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="55e40-103">Azure CLI 2.0 release notes</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="55e40-104">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-104">May 7, 2018</span></span>

<span data-ttu-id="55e40-105">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="55e40-105">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="55e40-106">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-106">Core</span></span>

* <span data-ttu-id="55e40-107">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="55e40-107">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="55e40-108">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="55e40-108">Added limited support for positional arguments</span></span>
* <span data-ttu-id="55e40-109">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="55e40-109">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="55e40-110">#5591</span><span class="sxs-lookup"><span data-stu-id="55e40-110">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="55e40-111">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="55e40-111">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="55e40-112">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="55e40-112">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="55e40-113">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-113">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="55e40-114">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="55e40-114">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="55e40-115">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="55e40-115">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-116">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-116">ACR</span></span>

* <span data-ttu-id="55e40-117">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-117">Added ACR Build commands</span></span>
* <span data-ttu-id="55e40-118">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="55e40-118">Improved resource not found error messages</span></span>
* <span data-ttu-id="55e40-119">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="55e40-119">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="55e40-120">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="55e40-120">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="55e40-121">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="55e40-121">Improved repository commands error messages</span></span>
* <span data-ttu-id="55e40-122">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="55e40-122">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-123">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-123">ACS</span></span>

* <span data-ttu-id="55e40-124">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="55e40-124">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="55e40-125">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="55e40-125">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="55e40-126">AMS</span><span class="sxs-lookup"><span data-stu-id="55e40-126">AMS</span></span>

* <span data-ttu-id="55e40-127">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="55e40-127">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-128">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-128">Appservice</span></span>

* <span data-ttu-id="55e40-129">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="55e40-129">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="55e40-130">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="55e40-130">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="55e40-131">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="55e40-131">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="55e40-132">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="55e40-132">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="55e40-133">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55e40-133">Batch AI</span></span>

* <span data-ttu-id="55e40-134">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="55e40-134">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55e40-135">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55e40-135">Cognitive Services</span></span>

* <span data-ttu-id="55e40-136">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="55e40-136">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="55e40-137">Consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-137">Consumption</span></span>

* <span data-ttu-id="55e40-138">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="55e40-138">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="55e40-139">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-139">Container</span></span>

* <span data-ttu-id="55e40-140">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="55e40-140">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="55e40-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="55e40-141">Cosmos DB</span></span>

* <span data-ttu-id="55e40-142">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="55e40-142">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="55e40-143">DMS</span><span class="sxs-lookup"><span data-stu-id="55e40-143">DMS</span></span>

* <span data-ttu-id="55e40-144">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="55e40-144">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-145">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-145">Extension</span></span>

* <span data-ttu-id="55e40-146">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="55e40-146">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-147">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-147">Interactive</span></span>

* <span data-ttu-id="55e40-148">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="55e40-148">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="55e40-149">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="55e40-149">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="55e40-150">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="55e40-150">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="55e40-151">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-151">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="55e40-152">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-152">Lab</span></span>

* <span data-ttu-id="55e40-153">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="55e40-153">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="55e40-154">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-154">Network</span></span>

* <span data-ttu-id="55e40-155">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="55e40-155">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="55e40-156">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-156">Profile</span></span>

* <span data-ttu-id="55e40-157">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="55e40-157">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="55e40-158">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="55e40-158">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="55e40-159">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="55e40-159">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="55e40-160">Redis</span><span class="sxs-lookup"><span data-stu-id="55e40-160">Redis</span></span>

* <span data-ttu-id="55e40-161">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="55e40-161">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="55e40-162">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="55e40-162">Deprecated `redis list-all`.</span></span> <span data-ttu-id="55e40-163">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="55e40-163">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="55e40-164">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="55e40-164">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="55e40-165">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-165">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="55e40-166">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-166">Role</span></span>

* <span data-ttu-id="55e40-167">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="55e40-167">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-168">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-168">Storage</span></span>

* <span data-ttu-id="55e40-169">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="55e40-169">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="55e40-170">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="55e40-170">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="55e40-171">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="55e40-171">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="55e40-172">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="55e40-172">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="55e40-173">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="55e40-173">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-174">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-174">VM</span></span>

* <span data-ttu-id="55e40-175">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="55e40-175">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="55e40-176">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="55e40-176">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="55e40-177">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="55e40-177">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="55e40-178">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="55e40-178">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="55e40-179">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="55e40-179">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="55e40-180">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="55e40-180">Added write accelerator support</span></span> 
* <span data-ttu-id="55e40-181">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="55e40-181">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="55e40-182">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-182">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="55e40-183">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="55e40-183">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="55e40-184">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-184">April 10, 2018</span></span>

<span data-ttu-id="55e40-185">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="55e40-185">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-186">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-186">ACR</span></span>

* <span data-ttu-id="55e40-187">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="55e40-187">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-188">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-188">ACS</span></span>

* <span data-ttu-id="55e40-189">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="55e40-189">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-190">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-190">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="55e40-192">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="55e40-192">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="55e40-193">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55e40-193">BatchAI</span></span>

* <span data-ttu-id="55e40-194">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="55e40-194">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="55e40-195">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="55e40-195">Job level mounting</span></span>
 - <span data-ttu-id="55e40-196">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="55e40-196">Environment variables with secret values</span></span>
 - <span data-ttu-id="55e40-197">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="55e40-197">Performance counters settings</span></span>
 - <span data-ttu-id="55e40-198">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="55e40-198">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="55e40-199">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="55e40-199">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="55e40-200">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="55e40-200">Usage and limits reporting</span></span>
 - <span data-ttu-id="55e40-201">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="55e40-201">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="55e40-202">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="55e40-202">Support for custom images</span></span>
 - <span data-ttu-id="55e40-203">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="55e40-203">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="55e40-204">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="55e40-204">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="55e40-205">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="55e40-205">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="55e40-206">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="55e40-206">National clouds are supported</span></span>
* <span data-ttu-id="55e40-207">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="55e40-207">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="55e40-208">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="55e40-208">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="55e40-209">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="55e40-209">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="55e40-210">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="55e40-210">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="55e40-211">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="55e40-211">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="55e40-212">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="55e40-212">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="55e40-213">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="55e40-213">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="55e40-214">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="55e40-214">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="55e40-215">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="55e40-215">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="55e40-216">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="55e40-216">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="55e40-217">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="55e40-217">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="55e40-218">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="55e40-218">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="55e40-219">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="55e40-219">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="55e40-220">Facturation</span><span class="sxs-lookup"><span data-stu-id="55e40-220">Billing</span></span>

* <span data-ttu-id="55e40-221">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="55e40-221">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="55e40-222">Consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-222">Consumption</span></span>

* <span data-ttu-id="55e40-223">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="55e40-223">Added `marketplace` commands</span></span>
* <span data-ttu-id="55e40-224">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="55e40-224">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="55e40-225">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="55e40-225">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="55e40-226">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="55e40-226">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="55e40-227">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="55e40-227">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="55e40-228">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="55e40-228">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="55e40-229">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-229">Container</span></span>

* <span data-ttu-id="55e40-230">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="55e40-230">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="55e40-231">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="55e40-231">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-232">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-232">Extension</span></span>

* <span data-ttu-id="55e40-233">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="55e40-233">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-234">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-234">Interactive</span></span>

* <span data-ttu-id="55e40-235">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="55e40-235">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="55e40-236">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="55e40-236">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="55e40-237">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="55e40-237">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="55e40-238">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-238">Network</span></span>

* <span data-ttu-id="55e40-239">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="55e40-239">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="55e40-240">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="55e40-240">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="55e40-241">#4910</span><span class="sxs-lookup"><span data-stu-id="55e40-241">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="55e40-242">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="55e40-242">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="55e40-243">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="55e40-243">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="55e40-244">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-244">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="55e40-245">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-245">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="55e40-246">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="55e40-246">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-247">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-247">Profile</span></span>

* <span data-ttu-id="55e40-248">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="55e40-248">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="55e40-249">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="55e40-249">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="55e40-250">SGBDR</span><span class="sxs-lookup"><span data-stu-id="55e40-250">RDBMS</span></span>

* <span data-ttu-id="55e40-251">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="55e40-251">Added `georestore` command</span></span>
* <span data-ttu-id="55e40-252">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="55e40-252">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-253">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-253">Resource</span></span>

* <span data-ttu-id="55e40-254">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="55e40-254">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="55e40-255">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="55e40-255">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-256">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-256">SQL</span></span>

* <span data-ttu-id="55e40-257">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="55e40-257">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-258">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-258">Storage</span></span>

* <span data-ttu-id="55e40-259">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="55e40-259">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-260">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-260">VM</span></span>

* <span data-ttu-id="55e40-261">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="55e40-261">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="55e40-262">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="55e40-262">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="55e40-264">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="55e40-264">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="55e40-265">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="55e40-265">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="55e40-266">#5718</span><span class="sxs-lookup"><span data-stu-id="55e40-266">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="55e40-267">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="55e40-267">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="55e40-268">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-268">March 27, 2018</span></span>

<span data-ttu-id="55e40-269">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="55e40-269">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="55e40-270">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-270">Core</span></span>

* <span data-ttu-id="55e40-271">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="55e40-271">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-272">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-272">ACS</span></span>

* <span data-ttu-id="55e40-273">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="55e40-273">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-274">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-274">Appservice</span></span>

* <span data-ttu-id="55e40-275">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="55e40-275">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="55e40-276">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="55e40-276">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="55e40-277">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="55e40-277">Backup</span></span>

* <span data-ttu-id="55e40-278">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="55e40-278">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="55e40-279">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="55e40-279">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="55e40-280">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="55e40-280">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="55e40-281">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="55e40-281">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="55e40-282">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-282">Container</span></span>

* <span data-ttu-id="55e40-283">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="55e40-283">Added `container exec` command.</span></span> <span data-ttu-id="55e40-284">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="55e40-284">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="55e40-285">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="55e40-285">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-286">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-286">Extension</span></span>

* <span data-ttu-id="55e40-287">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="55e40-287">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="55e40-288">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="55e40-288">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="55e40-289">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-289">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-290">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-290">Interactive</span></span>

* <span data-ttu-id="55e40-291">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="55e40-291">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="55e40-292">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="55e40-292">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="55e40-293">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="55e40-293">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="55e40-294">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="55e40-294">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="55e40-295">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-295">Lab</span></span>

* <span data-ttu-id="55e40-296">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="55e40-296">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-297">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-297">Monitor</span></span>

* <span data-ttu-id="55e40-298">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="55e40-298">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="55e40-299">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="55e40-299">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="55e40-300">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="55e40-300">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="55e40-301">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-301">Network</span></span>

* <span data-ttu-id="55e40-302">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="55e40-302">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-303">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-303">Profile</span></span>

* <span data-ttu-id="55e40-304">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="55e40-304">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="55e40-305">SGBDR</span><span class="sxs-lookup"><span data-stu-id="55e40-305">RDBMS</span></span>

* <span data-ttu-id="55e40-306">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="55e40-306">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-307">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-307">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="55e40-309">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-309">Role</span></span>

* <span data-ttu-id="55e40-310">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="55e40-310">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="55e40-311">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="55e40-311">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="55e40-312">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="55e40-312">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="55e40-313">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="55e40-313">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="55e40-314">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="55e40-314">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-315">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-315">Storage</span></span>

* <span data-ttu-id="55e40-316">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="55e40-316">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="55e40-317">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="55e40-317">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-318">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-318">VM</span></span>

* <span data-ttu-id="55e40-319">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="55e40-319">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="55e40-320">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="55e40-320">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="55e40-321">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="55e40-321">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="55e40-322">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="55e40-322">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="55e40-323">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-323">March 13, 2018</span></span>

<span data-ttu-id="55e40-324">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="55e40-324">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-325">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-325">ACR</span></span>

* <span data-ttu-id="55e40-326">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="55e40-326">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="55e40-327">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="55e40-327">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="55e40-328">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="55e40-328">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-329">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-329">ACS</span></span>

* <span data-ttu-id="55e40-330">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="55e40-330">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="55e40-331">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="55e40-331">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="55e40-332">Advisor</span><span class="sxs-lookup"><span data-stu-id="55e40-332">Advisor</span></span>

* <span data-ttu-id="55e40-333">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="55e40-333">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="55e40-334">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="55e40-334">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="55e40-335">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="55e40-335">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="55e40-336">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="55e40-336">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="55e40-337">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="55e40-337">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-338">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-338">Appservice</span></span>

* <span data-ttu-id="55e40-339">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="55e40-339">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="55e40-340">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="55e40-340">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="55e40-341">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="55e40-341">Eventhubs</span></span>

* <span data-ttu-id="55e40-342">Version initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-342">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-343">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-343">Extension</span></span>

* <span data-ttu-id="55e40-344">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="55e40-344">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-345">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-345">Interactive</span></span>

* <span data-ttu-id="55e40-346">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="55e40-346">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="55e40-347">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="55e40-347">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="55e40-348">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="55e40-348">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="55e40-349">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="55e40-349">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-350">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-350">Monitor</span></span>

* <span data-ttu-id="55e40-351">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="55e40-351">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="55e40-352">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="55e40-352">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="55e40-353">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="55e40-353">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="55e40-354">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="55e40-354">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="55e40-355">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-355">Network</span></span>

* <span data-ttu-id="55e40-356">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="55e40-356">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="55e40-357">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="55e40-357">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="55e40-358">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="55e40-358">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="55e40-359">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="55e40-359">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-360">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-360">Profile</span></span>

* <span data-ttu-id="55e40-361">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="55e40-361">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="55e40-362">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="55e40-362">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="55e40-363">SGBDR</span><span class="sxs-lookup"><span data-stu-id="55e40-363">RDBMS</span></span>

* <span data-ttu-id="55e40-364">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="55e40-364">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="55e40-365">Service Bus</span><span class="sxs-lookup"><span data-stu-id="55e40-365">Service Bus</span></span>

* <span data-ttu-id="55e40-366">Version initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-366">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-367">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-367">Storage</span></span>

* <span data-ttu-id="55e40-368">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="55e40-368">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="55e40-369">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="55e40-369">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-370">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-370">VM</span></span>

* <span data-ttu-id="55e40-371">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="55e40-371">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="55e40-372">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="55e40-372">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="55e40-373">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="55e40-373">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="55e40-374">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="55e40-374">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="55e40-375">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-375">February 27, 2018</span></span>

<span data-ttu-id="55e40-376">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="55e40-376">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="55e40-377">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-377">Core</span></span>

* <span data-ttu-id="55e40-378">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="55e40-378">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="55e40-379">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="55e40-379">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="55e40-380">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="55e40-380">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-381">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-381">ACS</span></span>

* <span data-ttu-id="55e40-382">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-382">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="55e40-383">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="55e40-383">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="55e40-384">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="55e40-384">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="55e40-385">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="55e40-385">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-386">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-386">Appservice</span></span>

* <span data-ttu-id="55e40-387">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="55e40-387">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="55e40-388">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="55e40-388">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55e40-389">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55e40-389">Cognitive Services</span></span>

* <span data-ttu-id="55e40-390">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55e40-390">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="55e40-391">Consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-391">Consumption</span></span>

* <span data-ttu-id="55e40-392">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="55e40-392">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="55e40-393">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="55e40-393">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="55e40-394">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-394">Container</span></span>

* <span data-ttu-id="55e40-395">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="55e40-395">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="55e40-396">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-396">Network</span></span>

* <span data-ttu-id="55e40-397">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="55e40-397">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-398">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-398">Resource</span></span>

* <span data-ttu-id="55e40-399">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="55e40-399">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="55e40-400">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-400">Role</span></span>

* <span data-ttu-id="55e40-401">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="55e40-401">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-402">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-402">SQL</span></span>

* <span data-ttu-id="55e40-403">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="55e40-403">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-404">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-404">Storage</span></span>

* <span data-ttu-id="55e40-405">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="55e40-405">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-406">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-406">VM</span></span>

* <span data-ttu-id="55e40-407">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="55e40-407">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="55e40-408">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-408">February 13, 2018</span></span>

<span data-ttu-id="55e40-409">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="55e40-409">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="55e40-410">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-410">Core</span></span>

* <span data-ttu-id="55e40-411">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="55e40-411">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-412">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-412">ACS</span></span>

* <span data-ttu-id="55e40-413">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="55e40-413">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="55e40-414">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="55e40-414">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="55e40-415">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="55e40-415">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="55e40-416">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="55e40-416">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="55e40-417">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="55e40-417">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="55e40-418">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="55e40-418">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="55e40-419">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="55e40-419">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="55e40-420">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="55e40-420">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-421">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-421">Appservice</span></span>

* <span data-ttu-id="55e40-422">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="55e40-422">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="55e40-423">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="55e40-423">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="55e40-424">CDN</span><span class="sxs-lookup"><span data-stu-id="55e40-424">CDN</span></span>

* <span data-ttu-id="55e40-425">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="55e40-425">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="55e40-426">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-426">Container</span></span>

* <span data-ttu-id="55e40-427">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="55e40-427">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="55e40-428">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-428">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55e40-429">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55e40-429">CosmosDB</span></span>

* <span data-ttu-id="55e40-430">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="55e40-430">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-431">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-431">Extension</span></span>

* <span data-ttu-id="55e40-432">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-432">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="55e40-433">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-433">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="55e40-434">Commentaires</span><span class="sxs-lookup"><span data-stu-id="55e40-434">Feedback</span></span>

* <span data-ttu-id="55e40-435">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="55e40-435">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-436">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-436">Interactive</span></span>

* <span data-ttu-id="55e40-437">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="55e40-437">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="55e40-438">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="55e40-438">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="55e40-439">IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-439">IoT</span></span>

* <span data-ttu-id="55e40-440">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="55e40-440">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="55e40-441">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="55e40-441">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="55e40-442">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-442">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="55e40-443">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="55e40-443">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-444">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-444">Monitor</span></span>

* <span data-ttu-id="55e40-445">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="55e40-445">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="55e40-446">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-446">Network</span></span>

* <span data-ttu-id="55e40-447">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="55e40-447">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="55e40-448">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-448">Profile</span></span>

* <span data-ttu-id="55e40-449">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="55e40-449">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-450">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-450">Resource</span></span>

* <span data-ttu-id="55e40-451">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="55e40-451">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="55e40-452">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-452">Role</span></span>

* <span data-ttu-id="55e40-453">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="55e40-453">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-454">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-454">SQL</span></span>

* <span data-ttu-id="55e40-455">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="55e40-455">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="55e40-456">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="55e40-456">Added `sql db rename`</span></span>
* <span data-ttu-id="55e40-457">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="55e40-457">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-458">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-458">Storage</span></span>

* <span data-ttu-id="55e40-459">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="55e40-459">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-460">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-460">VM</span></span>

* <span data-ttu-id="55e40-461">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="55e40-461">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="55e40-462">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="55e40-462">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="55e40-463">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="55e40-463">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="55e40-464">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-464">January 31, 2018</span></span>

<span data-ttu-id="55e40-465">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="55e40-465">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="55e40-466">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-466">Core</span></span>

* <span data-ttu-id="55e40-467">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="55e40-467">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="55e40-468">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="55e40-468">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="55e40-469">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="55e40-469">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="55e40-470">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="55e40-470">Use `--verbose` to see</span></span>
* <span data-ttu-id="55e40-471">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="55e40-471">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-472">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-472">ACS</span></span>

* <span data-ttu-id="55e40-473">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="55e40-473">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="55e40-474">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="55e40-474">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-475">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-475">Appservice</span></span>

* <span data-ttu-id="55e40-476">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="55e40-476">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="55e40-477">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="55e40-477">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="55e40-478">CDN</span><span class="sxs-lookup"><span data-stu-id="55e40-478">CDN</span></span>

* <span data-ttu-id="55e40-479">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="55e40-479">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55e40-480">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55e40-480">CosmosDB</span></span>

* <span data-ttu-id="55e40-481">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="55e40-481">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-482">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-482">Interactive</span></span>

* <span data-ttu-id="55e40-483">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="55e40-483">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="55e40-484">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-484">Network</span></span>

* <span data-ttu-id="55e40-485">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="55e40-485">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="55e40-486">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-486">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="55e40-487">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="55e40-487">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="55e40-488">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="55e40-488">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="55e40-489">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="55e40-489">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="55e40-490">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="55e40-490">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="55e40-491">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="55e40-491">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="55e40-492">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="55e40-492">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="55e40-493">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="55e40-493">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="55e40-494">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="55e40-494">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-495">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-495">Profile</span></span>

* <span data-ttu-id="55e40-496">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="55e40-496">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-497">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-497">Resource</span></span>

* <span data-ttu-id="55e40-498">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="55e40-498">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-499">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-499">Storage</span></span>

* <span data-ttu-id="55e40-500">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="55e40-500">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="55e40-501">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="55e40-501">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="55e40-502">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="55e40-502">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="55e40-503">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="55e40-503">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="55e40-504">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="55e40-504">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-505">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-505">VM</span></span>

* <span data-ttu-id="55e40-506">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="55e40-506">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="55e40-507">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="55e40-507">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="55e40-508">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="55e40-508">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="55e40-509">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-509">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="55e40-510">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="55e40-510">January 17, 2018</span></span>

<span data-ttu-id="55e40-511">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="55e40-511">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-512">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-512">ACR</span></span>

* <span data-ttu-id="55e40-513">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="55e40-513">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="55e40-514">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="55e40-514">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-515">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-515">ACS</span></span>

* <span data-ttu-id="55e40-516">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="55e40-516">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="55e40-517">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="55e40-517">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-518">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-518">Appservice</span></span>

* <span data-ttu-id="55e40-519">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="55e40-519">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="55e40-520">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="55e40-520">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="55e40-521">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="55e40-521">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="55e40-522">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="55e40-522">Backup</span></span>

* <span data-ttu-id="55e40-523">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="55e40-523">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="55e40-524">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="55e40-524">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="55e40-525">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="55e40-525">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="55e40-526">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="55e40-526">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="55e40-527">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-527">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="55e40-528">Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-528">Batch</span></span>

* <span data-ttu-id="55e40-529">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="55e40-529">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="55e40-530">Cloud</span><span class="sxs-lookup"><span data-stu-id="55e40-530">Cloud</span></span>

* <span data-ttu-id="55e40-531">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="55e40-531">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="55e40-532">Consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-532">Consumption</span></span>

* <span data-ttu-id="55e40-533">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="55e40-533">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="55e40-534">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55e40-534">Event Grid</span></span>

* <span data-ttu-id="55e40-535">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="55e40-535">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="55e40-536">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="55e40-536">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="55e40-537">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="55e40-537">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="55e40-538">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="55e40-538">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="55e40-539">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="55e40-539">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="55e40-540">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="55e40-540">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="55e40-541">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="55e40-541">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="55e40-542">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="55e40-542">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-543">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-543">Interactive</span></span>

* <span data-ttu-id="55e40-544">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="55e40-544">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="55e40-545">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="55e40-545">Fixed errors on startup</span></span>
* <span data-ttu-id="55e40-546">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="55e40-546">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="55e40-547">IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-547">IoT</span></span>

* <span data-ttu-id="55e40-548">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="55e40-548">Added support for device provisioning service</span></span>
* <span data-ttu-id="55e40-549">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-549">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="55e40-550">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-550">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-551">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-551">Monitor</span></span>

* <span data-ttu-id="55e40-552">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="55e40-552">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="55e40-553">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="55e40-553">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="55e40-554">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="55e40-554">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="55e40-555">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-555">Network</span></span>

* <span data-ttu-id="55e40-556">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="55e40-556">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="55e40-557">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-557">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-558">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-558">Profile</span></span>

* <span data-ttu-id="55e40-559">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="55e40-559">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="55e40-560">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-560">Role</span></span>

* <span data-ttu-id="55e40-561">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="55e40-561">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55e40-562">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55e40-562">Service Fabric</span></span>

* <span data-ttu-id="55e40-563">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="55e40-563">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="55e40-564">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-564">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-565">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-565">VM</span></span>

* <span data-ttu-id="55e40-566">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="55e40-566">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="55e40-567">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="55e40-567">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="55e40-568">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="55e40-568">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="55e40-569">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="55e40-569">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="55e40-570">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="55e40-570">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="55e40-571">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-571">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="55e40-572">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-572">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="55e40-573">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="55e40-573">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="55e40-574">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-574">December 19, 2017</span></span>

<span data-ttu-id="55e40-575">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="55e40-575">Version 2.0.23</span></span>

* <span data-ttu-id="55e40-576">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="55e40-576">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="55e40-577">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-577">Container</span></span>

* <span data-ttu-id="55e40-578">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-578">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="55e40-579">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-579">Network</span></span>

* <span data-ttu-id="55e40-580">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-580">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="55e40-581">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-581">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-582">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-582">Storage</span></span>

* <span data-ttu-id="55e40-583">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="55e40-583">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-584">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-584">VM</span></span>

* <span data-ttu-id="55e40-585">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="55e40-585">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="55e40-586">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-586">December 5, 2017</span></span>

<span data-ttu-id="55e40-587">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="55e40-587">Version 2.0.22</span></span>

* <span data-ttu-id="55e40-588">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="55e40-588">Removed `az component` commands.</span></span> <span data-ttu-id="55e40-589">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="55e40-589">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="55e40-590">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-590">Core</span></span>
* <span data-ttu-id="55e40-591">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="55e40-591">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="55e40-592">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="55e40-592">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-593">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-593">ACS</span></span>

* <span data-ttu-id="55e40-594">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="55e40-594">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="55e40-595">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="55e40-595">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="55e40-596">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="55e40-596">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="55e40-597">Advisor</span><span class="sxs-lookup"><span data-stu-id="55e40-597">Advisor</span></span>

* <span data-ttu-id="55e40-598">Version initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-598">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-599">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-599">Appservice</span></span>

* <span data-ttu-id="55e40-600">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="55e40-600">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="55e40-601">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="55e40-601">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="55e40-602">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="55e40-602">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="55e40-603">Consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-603">Consumption</span></span>

* <span data-ttu-id="55e40-604">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="55e40-604">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="55e40-605">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-605">Container</span></span>

* <span data-ttu-id="55e40-606">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-606">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-607">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-607">Monitor</span></span>

* <span data-ttu-id="55e40-608">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="55e40-608">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-609">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-609">Resource</span></span>

* <span data-ttu-id="55e40-610">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="55e40-610">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="55e40-611">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-611">Role</span></span>

* <span data-ttu-id="55e40-612">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="55e40-612">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="55e40-613">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="55e40-613">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="55e40-614">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="55e40-614">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-615">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-615">SQL</span></span>

* <span data-ttu-id="55e40-616">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="55e40-616">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="55e40-617">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="55e40-617">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-618">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-618">VM</span></span>

* <span data-ttu-id="55e40-619">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="55e40-619">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="55e40-620">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-620">November 14, 2017</span></span>

<span data-ttu-id="55e40-621">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="55e40-621">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-622">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-622">ACR</span></span>

* <span data-ttu-id="55e40-623">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="55e40-623">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="55e40-624">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-624">ACS</span></span>

* <span data-ttu-id="55e40-625">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="55e40-625">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="55e40-626">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="55e40-626">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="55e40-627">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="55e40-627">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="55e40-628">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="55e40-628">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="55e40-629">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="55e40-629">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-630">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-630">Appservice</span></span>

* <span data-ttu-id="55e40-631">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="55e40-631">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="55e40-632">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="55e40-632">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="55e40-633">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="55e40-633">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="55e40-634">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="55e40-634">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="55e40-635">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="55e40-635">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="55e40-636">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="55e40-636">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="55e40-637">Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-637">Batch</span></span>

* <span data-ttu-id="55e40-638">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="55e40-638">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="55e40-639">Batchai</span><span class="sxs-lookup"><span data-stu-id="55e40-639">Batchai</span></span>

* <span data-ttu-id="55e40-640">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="55e40-640">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="55e40-641">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="55e40-641">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="55e40-642">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="55e40-642">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="55e40-643">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="55e40-643">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="55e40-644">Cloud</span><span class="sxs-lookup"><span data-stu-id="55e40-644">Cloud</span></span>

* <span data-ttu-id="55e40-645">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="55e40-645">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="55e40-646">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-646">Container</span></span>

* <span data-ttu-id="55e40-647">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="55e40-647">Added support to open multiple ports</span></span>
* <span data-ttu-id="55e40-648">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="55e40-648">Added container group restart policy</span></span>
* <span data-ttu-id="55e40-649">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="55e40-649">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="55e40-650">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="55e40-650">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55e40-651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55e40-651">Data Lake Analytics</span></span>

* <span data-ttu-id="55e40-652">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="55e40-652">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55e40-653">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-653">Data Lake Store</span></span>

* <span data-ttu-id="55e40-654">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="55e40-654">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-655">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-655">Extension</span></span>

* <span data-ttu-id="55e40-656">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="55e40-656">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="55e40-657">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="55e40-657">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="55e40-658">IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-658">IoT</span></span>

* <span data-ttu-id="55e40-659">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="55e40-659">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-660">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-660">Monitor</span></span>

* <span data-ttu-id="55e40-661">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="55e40-661">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="55e40-662">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-662">Network</span></span>

* <span data-ttu-id="55e40-663">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="55e40-663">Added support for CAA DNS records</span></span>
* <span data-ttu-id="55e40-664">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="55e40-664">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="55e40-665">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="55e40-665">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="55e40-666">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="55e40-666">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="55e40-667">Réservations</span><span class="sxs-lookup"><span data-stu-id="55e40-667">Reservations</span></span>

* <span data-ttu-id="55e40-668">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-668">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-669">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-669">Resource</span></span>

* <span data-ttu-id="55e40-670">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="55e40-670">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-671">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-671">SQL</span></span>

* <span data-ttu-id="55e40-672">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-672">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-673">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-673">Storage</span></span>

* <span data-ttu-id="55e40-674">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-674">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="55e40-675">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="55e40-675">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="55e40-676">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="55e40-676">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="55e40-677">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="55e40-677">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="55e40-678">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="55e40-678">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="55e40-679">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="55e40-679">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="55e40-680">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-680">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-681">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-681">VM</span></span>

* <span data-ttu-id="55e40-682">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="55e40-682">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="55e40-683">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="55e40-683">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="55e40-684">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="55e40-684">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="55e40-685">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="55e40-685">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="55e40-686">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="55e40-686">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="55e40-687">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-687">October 24, 2017</span></span>

<span data-ttu-id="55e40-688">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="55e40-688">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="55e40-689">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-689">Core</span></span>

* <span data-ttu-id="55e40-690">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="55e40-690">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-691">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-691">ACR</span></span>

* <span data-ttu-id="55e40-692">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="55e40-692">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="55e40-693">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="55e40-693">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="55e40-694">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="55e40-694">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-695">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-695">ACS</span></span>

* <span data-ttu-id="55e40-696">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="55e40-696">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="55e40-697">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="55e40-697">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-698">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-698">Appservice</span></span>

* <span data-ttu-id="55e40-699">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="55e40-699">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="55e40-700">Composant</span><span class="sxs-lookup"><span data-stu-id="55e40-700">Component</span></span>

* <span data-ttu-id="55e40-701">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="55e40-701">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-702">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-702">Monitor</span></span>

* <span data-ttu-id="55e40-703">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="55e40-703">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-704">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-704">Resource</span></span>

* <span data-ttu-id="55e40-705">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="55e40-705">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="55e40-706">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="55e40-706">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-707">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-707">VM</span></span>

* <span data-ttu-id="55e40-708">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="55e40-708">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="55e40-709">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-709">October 9, 2017</span></span>

<span data-ttu-id="55e40-710">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="55e40-710">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="55e40-711">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-711">Core</span></span>

* <span data-ttu-id="55e40-712">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="55e40-712">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-713">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-713">Appservice</span></span>

* <span data-ttu-id="55e40-714">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="55e40-714">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="55e40-715">Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-715">Batch</span></span>

* <span data-ttu-id="55e40-716">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="55e40-716">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="55e40-717">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="55e40-717">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="55e40-718">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-718">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="55e40-719">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="55e40-719">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="55e40-720">Batchai</span><span class="sxs-lookup"><span data-stu-id="55e40-720">Batchai</span></span>

* <span data-ttu-id="55e40-721">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="55e40-721">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="55e40-722">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55e40-722">Keyvault</span></span>

* <span data-ttu-id="55e40-723">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="55e40-723">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="55e40-724">(#4448)</span><span class="sxs-lookup"><span data-stu-id="55e40-724">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="55e40-725">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-725">Network</span></span>

* <span data-ttu-id="55e40-726">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="55e40-726">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="55e40-727">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="55e40-727">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-728">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-728">Resource</span></span>

* <span data-ttu-id="55e40-729">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="55e40-729">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="55e40-730">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="55e40-730">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="55e40-731">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="55e40-731">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="55e40-732">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="55e40-732">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-733">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-733">Sql</span></span>

* <span data-ttu-id="55e40-734">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="55e40-734">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="55e40-735">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="55e40-735">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="55e40-736">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="55e40-736">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-737">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-737">Storage</span></span>

* <span data-ttu-id="55e40-738">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="55e40-738">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-739">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-739">Vm</span></span>

* <span data-ttu-id="55e40-740">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="55e40-740">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="55e40-741">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="55e40-741">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="55e40-742">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="55e40-742">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="55e40-743">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="55e40-743">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="55e40-744">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="55e40-744">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="55e40-745">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-745">September 22, 2017</span></span>

<span data-ttu-id="55e40-746">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="55e40-746">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-747">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-747">Resource</span></span>

* <span data-ttu-id="55e40-748">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="55e40-748">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="55e40-749">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="55e40-749">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="55e40-750">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="55e40-750">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="55e40-751">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="55e40-751">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="55e40-752">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-752">Network</span></span>

* <span data-ttu-id="55e40-753">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="55e40-753">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="55e40-754">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="55e40-754">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="55e40-755">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="55e40-755">Added `asg` application security group commands</span></span>
* <span data-ttu-id="55e40-756">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-756">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="55e40-757">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-757">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="55e40-758">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-758">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="55e40-759">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="55e40-759">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-760">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-760">Storage</span></span>

* <span data-ttu-id="55e40-761">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="55e40-761">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="55e40-762">Événement</span><span class="sxs-lookup"><span data-stu-id="55e40-762">Eventgrid</span></span>

* <span data-ttu-id="55e40-763">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="55e40-763">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-764">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-764">SQL</span></span>

* <span data-ttu-id="55e40-765">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="55e40-765">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="55e40-766">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="55e40-766">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="55e40-767">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-767">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="55e40-768">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55e40-768">Keyvault</span></span>

* <span data-ttu-id="55e40-769">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="55e40-769">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-770">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-770">VM</span></span>

* <span data-ttu-id="55e40-771">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-771">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="55e40-772">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="55e40-772">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="55e40-773">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="55e40-773">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="55e40-774">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="55e40-774">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="55e40-775">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="55e40-775">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="55e40-776">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="55e40-776">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-777">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-777">ACS</span></span>

* <span data-ttu-id="55e40-778">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="55e40-778">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-779">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-779">Appservice</span></span>

* <span data-ttu-id="55e40-780">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="55e40-780">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="55e40-781">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="55e40-781">Backup</span></span>

* <span data-ttu-id="55e40-782">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="55e40-782">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="55e40-783">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-783">September 11, 2017</span></span>

<span data-ttu-id="55e40-784">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="55e40-784">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="55e40-785">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-785">Core</span></span>

* <span data-ttu-id="55e40-786">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="55e40-786">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="55e40-787">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="55e40-787">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-788">Acs</span><span class="sxs-lookup"><span data-stu-id="55e40-788">Acs</span></span>

* <span data-ttu-id="55e40-789">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="55e40-789">Added `acs list-locations` command</span></span>
* <span data-ttu-id="55e40-790">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="55e40-790">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-791">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-791">Appservice</span></span>

* <span data-ttu-id="55e40-792">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="55e40-792">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="55e40-793">CDN</span><span class="sxs-lookup"><span data-stu-id="55e40-793">CDN</span></span>

* <span data-ttu-id="55e40-794">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="55e40-794">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="55e40-795">Extension</span><span class="sxs-lookup"><span data-stu-id="55e40-795">Extension</span></span>

* <span data-ttu-id="55e40-796">Version initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-796">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="55e40-797">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55e40-797">Keyvault</span></span>

* <span data-ttu-id="55e40-798">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="55e40-798">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="55e40-799">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-799">Network</span></span>

* <span data-ttu-id="55e40-800">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="55e40-800">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="55e40-801">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="55e40-801">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="55e40-802">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="55e40-802">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="55e40-803">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="55e40-803">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="55e40-804">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="55e40-804">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-805">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-805">Resource</span></span>

* <span data-ttu-id="55e40-806">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="55e40-806">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="55e40-807">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="55e40-807">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="55e40-808">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="55e40-808">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="55e40-809">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="55e40-809">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-810">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-810">SQL</span></span>

* <span data-ttu-id="55e40-811">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="55e40-811">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-812">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-812">VM</span></span>

* <span data-ttu-id="55e40-813">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="55e40-813">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="55e40-814">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="55e40-814">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="55e40-815">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-815">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="55e40-816">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="55e40-816">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="55e40-817">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="55e40-817">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="55e40-818">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-818">August 31, 2017</span></span>

<span data-ttu-id="55e40-819">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="55e40-819">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="55e40-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55e40-820">Keyvault</span></span>

* <span data-ttu-id="55e40-821">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="55e40-821">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="55e40-822">Sf</span><span class="sxs-lookup"><span data-stu-id="55e40-822">Sf</span></span>

* <span data-ttu-id="55e40-823">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="55e40-823">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-824">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-824">Storage</span></span>

* <span data-ttu-id="55e40-825">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="55e40-825">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="55e40-826">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="55e40-826">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="55e40-827">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-827">August 28, 2017</span></span>

<span data-ttu-id="55e40-828">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="55e40-828">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="55e40-829">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="55e40-829">CLI</span></span>

* <span data-ttu-id="55e40-830">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="55e40-830">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-831">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-831">ACS</span></span>

* <span data-ttu-id="55e40-832">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="55e40-832">Corrected preview regions</span></span>
* <span data-ttu-id="55e40-833">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="55e40-833">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="55e40-834">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-834">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-835">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-835">Appservice</span></span>

* <span data-ttu-id="55e40-836">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="55e40-836">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="55e40-837">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="55e40-837">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="55e40-838">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="55e40-838">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="55e40-839">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="55e40-839">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="55e40-840">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="55e40-840">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="55e40-841">IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-841">IoT</span></span>

* <span data-ttu-id="55e40-842">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="55e40-842">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="55e40-843">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-843">Network</span></span>

* <span data-ttu-id="55e40-844">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="55e40-844">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="55e40-845">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-845">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="55e40-846">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="55e40-846">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="55e40-847">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="55e40-847">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="55e40-848">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="55e40-848">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-849">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-849">Profile</span></span>

* <span data-ttu-id="55e40-850">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-850">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55e40-851">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55e40-851">Service Fabric</span></span>

* <span data-ttu-id="55e40-852">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="55e40-852">Preview release</span></span>
* <span data-ttu-id="55e40-853">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="55e40-853">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="55e40-854">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="55e40-854">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="55e40-855">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="55e40-855">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-856">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-856">Storage</span></span>

* <span data-ttu-id="55e40-857">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="55e40-857">Enabled setting blob tier</span></span>
* <span data-ttu-id="55e40-858">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="55e40-858">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="55e40-859">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="55e40-859">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="55e40-860">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="55e40-860">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="55e40-861">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="55e40-861">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="55e40-862">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="55e40-862">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-863">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-863">VM</span></span>

* <span data-ttu-id="55e40-864">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="55e40-864">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="55e40-865">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="55e40-865">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="55e40-866">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="55e40-866">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="55e40-867">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="55e40-867">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="55e40-868">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="55e40-868">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="55e40-869">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="55e40-869">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="55e40-870">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-870">August 15, 2017</span></span>

<span data-ttu-id="55e40-871">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="55e40-871">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-872">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-872">ACS</span></span>

* <span data-ttu-id="55e40-873">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="55e40-873">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-874">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-874">Appservice</span></span>

* <span data-ttu-id="55e40-875">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="55e40-875">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="55e40-876">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55e40-876">Event Grid</span></span>

* <span data-ttu-id="55e40-877">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="55e40-877">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="55e40-878">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-878">August 11, 2017</span></span>

<span data-ttu-id="55e40-879">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="55e40-879">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-880">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-880">ACS</span></span>

* <span data-ttu-id="55e40-881">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="55e40-881">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="55e40-882">Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-882">Batch</span></span>

* <span data-ttu-id="55e40-883">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="55e40-883">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="55e40-884">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="55e40-884">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="55e40-885">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="55e40-885">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="55e40-886">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="55e40-886">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="55e40-887">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="55e40-887">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="55e40-888">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="55e40-888">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="55e40-889">Composant</span><span class="sxs-lookup"><span data-stu-id="55e40-889">Component</span></span>

* <span data-ttu-id="55e40-890">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="55e40-890">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="55e40-891">Conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-891">Container</span></span>

* <span data-ttu-id="55e40-892">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="55e40-892">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="55e40-893">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-893">Data Lake Store</span></span>

* <span data-ttu-id="55e40-894">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="55e40-894">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="55e40-895">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55e40-895">Event Grid</span></span>

* <span data-ttu-id="55e40-896">Version initiale</span><span class="sxs-lookup"><span data-stu-id="55e40-896">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="55e40-897">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-897">Network</span></span>

* <span data-ttu-id="55e40-898">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="55e40-898">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="55e40-899">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="55e40-899">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="55e40-900">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="55e40-900">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="55e40-901">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="55e40-901">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-902">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-902">Profile</span></span>

* <span data-ttu-id="55e40-903">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="55e40-903">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-904">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-904">Storage</span></span>

* <span data-ttu-id="55e40-905">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="55e40-905">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-906">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-906">VM</span></span>

* <span data-ttu-id="55e40-907">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="55e40-907">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="55e40-908">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="55e40-908">Exposed `list-skus` command</span></span>
* <span data-ttu-id="55e40-909">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-909">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="55e40-910">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="55e40-910">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="55e40-911">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="55e40-911">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="55e40-912">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-912">July 28, 2017</span></span>

<span data-ttu-id="55e40-913">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="55e40-913">Version 2.0.12</span></span>

* <span data-ttu-id="55e40-914">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="55e40-914">Added container commands</span></span>
* <span data-ttu-id="55e40-915">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="55e40-915">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="55e40-916">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-916">Core</span></span>

* <span data-ttu-id="55e40-917">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="55e40-917">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="55e40-918">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="55e40-918">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="55e40-919">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="55e40-919">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="55e40-920">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="55e40-920">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="55e40-921">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="55e40-921">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="55e40-922">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="55e40-922">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="55e40-923">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="55e40-923">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="55e40-924">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="55e40-924">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="55e40-925">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="55e40-925">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="55e40-926">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="55e40-926">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="55e40-927">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="55e40-927">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="55e40-928">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="55e40-928">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="55e40-929">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="55e40-929">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="55e40-930">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="55e40-930">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="55e40-931">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="55e40-931">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="55e40-932">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="55e40-932">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="55e40-933">ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-933">ACR</span></span>

* <span data-ttu-id="55e40-934">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="55e40-934">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="55e40-935">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="55e40-935">Support SKU update for managed registries</span></span>
* <span data-ttu-id="55e40-936">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="55e40-936">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="55e40-937">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="55e40-937">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="55e40-938">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="55e40-938">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="55e40-939">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="55e40-939">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-940">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-940">ACS</span></span>

* <span data-ttu-id="55e40-941">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="55e40-941">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-942">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-942">Appservice</span></span>

* <span data-ttu-id="55e40-943">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="55e40-943">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="55e40-944">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="55e40-944">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="55e40-945">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="55e40-945">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="55e40-946">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="55e40-946">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="55e40-947">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="55e40-947">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="55e40-948">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="55e40-948">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="55e40-949">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="55e40-949">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="55e40-950">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="55e40-950">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="55e40-951">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="55e40-951">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="55e40-952">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="55e40-952">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="55e40-953">Batch</span><span class="sxs-lookup"><span data-stu-id="55e40-953">Batch</span></span>

* <span data-ttu-id="55e40-954">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="55e40-954">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="55e40-955">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="55e40-955">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="55e40-956">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="55e40-956">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="55e40-957">CDN</span><span class="sxs-lookup"><span data-stu-id="55e40-957">CDN</span></span>

* <span data-ttu-id="55e40-958">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="55e40-958">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="55e40-959">Cloud</span><span class="sxs-lookup"><span data-stu-id="55e40-959">Cloud</span></span>

* <span data-ttu-id="55e40-960">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="55e40-960">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="55e40-961">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="55e40-961">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="55e40-962">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="55e40-962">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="55e40-963">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="55e40-963">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="55e40-964">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="55e40-964">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55e40-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55e40-965">CosmosDB</span></span>

* <span data-ttu-id="55e40-966">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="55e40-966">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="55e40-967">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="55e40-967">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55e40-968">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55e40-968">Data Lake Analytics</span></span>

* <span data-ttu-id="55e40-969">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="55e40-969">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="55e40-970">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="55e40-970">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="55e40-971">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="55e40-971">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55e40-972">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-972">Data Lake Store</span></span>

* <span data-ttu-id="55e40-973">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="55e40-973">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="55e40-974">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="55e40-974">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="55e40-975">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="55e40-975">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="55e40-976">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-976">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="55e40-977">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e40-977">Interactive</span></span>

* <span data-ttu-id="55e40-978">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="55e40-978">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="55e40-979">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="55e40-979">Increased test coverage</span></span>
* <span data-ttu-id="55e40-980">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="55e40-980">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="55e40-981">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="55e40-981">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="55e40-982">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="55e40-982">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="55e40-983">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="55e40-983">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="55e40-984">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="55e40-984">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="55e40-985">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="55e40-985">Added `--progress` flag</span></span>
* <span data-ttu-id="55e40-986">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="55e40-986">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="55e40-987">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="55e40-987">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="55e40-988">IoT</span><span class="sxs-lookup"><span data-stu-id="55e40-988">IoT</span></span>

* <span data-ttu-id="55e40-989">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="55e40-989">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="55e40-990">(#3934)</span><span class="sxs-lookup"><span data-stu-id="55e40-990">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="55e40-991">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="55e40-991">Key vault</span></span>

* <span data-ttu-id="55e40-992">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="55e40-992">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="55e40-993">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55e40-993">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="55e40-994">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55e40-994">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="55e40-995">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55e40-995">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="55e40-996">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55e40-996">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="55e40-997">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="55e40-997">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="55e40-998">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="55e40-998">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="55e40-999">(#3307)</span><span class="sxs-lookup"><span data-stu-id="55e40-999">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="55e40-1000">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1000">Lab</span></span>

* <span data-ttu-id="55e40-1001">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="55e40-1001">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="55e40-1002">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="55e40-1002">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-1003">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-1003">Monitor</span></span>

* <span data-ttu-id="55e40-1004">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="55e40-1004">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="55e40-1005">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="55e40-1005">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="55e40-1006">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="55e40-1006">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="55e40-1007">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="55e40-1007">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="55e40-1008">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="55e40-1008">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="55e40-1009">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="55e40-1009">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="55e40-1010">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="55e40-1010">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="55e40-1011">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="55e40-1011">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="55e40-1012">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="55e40-1012">`location` no longer required</span></span>
  * <span data-ttu-id="55e40-1013">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="55e40-1013">Add name and ID support for target</span></span>
  * <span data-ttu-id="55e40-1014">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="55e40-1014">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="55e40-1015">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="55e40-1015">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="55e40-1016">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="55e40-1016">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="55e40-1017">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="55e40-1017">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="55e40-1018">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="55e40-1018">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="55e40-1019">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1019">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="55e40-1020">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-1020">Network</span></span>

* <span data-ttu-id="55e40-1021">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="55e40-1021">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="55e40-1022">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1022">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="55e40-1023">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="55e40-1023">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="55e40-1024">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="55e40-1024">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="55e40-1025">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1025">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="55e40-1026">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="55e40-1026">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="55e40-1027">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="55e40-1027">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="55e40-1028">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="55e40-1028">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="55e40-1029">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="55e40-1029">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="55e40-1030">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="55e40-1030">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="55e40-1031">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1031">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="55e40-1032">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="55e40-1032">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="55e40-1033">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="55e40-1033">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="55e40-1034">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1034">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="55e40-1035">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1035">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="55e40-1036">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1036">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="55e40-1037">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="55e40-1037">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="55e40-1038">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="55e40-1038">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="55e40-1039">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1039">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="55e40-1040">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1040">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="55e40-1041">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1041">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="55e40-1042">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-1042">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="55e40-1043">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="55e40-1043">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="55e40-1044">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="55e40-1044">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="55e40-1045">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="55e40-1045">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="55e40-1046">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="55e40-1046">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="55e40-1047">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="55e40-1047">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-1048">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-1048">Profile</span></span>

* <span data-ttu-id="55e40-1049">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="55e40-1049">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="55e40-1050">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="55e40-1050">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="55e40-1051">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="55e40-1051">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="55e40-1052">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="55e40-1052">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="55e40-1053">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="55e40-1053">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="55e40-1054">SGBDR</span><span class="sxs-lookup"><span data-stu-id="55e40-1054">RDBMS</span></span>

* <span data-ttu-id="55e40-1055">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="55e40-1055">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="55e40-1056">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="55e40-1056">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="55e40-1057">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="55e40-1057">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="55e40-1058">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="55e40-1058">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-1059">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-1059">Resource</span></span>

* <span data-ttu-id="55e40-1060">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1060">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="55e40-1061">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="55e40-1061">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="55e40-1062">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="55e40-1062">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="55e40-1063">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="55e40-1063">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="55e40-1064">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="55e40-1064">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="55e40-1065">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="55e40-1065">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="55e40-1066">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="55e40-1066">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="55e40-1067">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="55e40-1067">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="55e40-1068">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-1068">Role</span></span>

* <span data-ttu-id="55e40-1069">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="55e40-1069">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="55e40-1070">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="55e40-1070">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="55e40-1071">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="55e40-1071">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="55e40-1072">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="55e40-1072">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="55e40-1073">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="55e40-1073">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55e40-1074">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55e40-1074">Service Fabric</span></span>
* <span data-ttu-id="55e40-1075">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="55e40-1075">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="55e40-1076">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="55e40-1076">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="55e40-1077">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="55e40-1077">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-1078">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-1078">SQL</span></span>

* <span data-ttu-id="55e40-1079">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="55e40-1079">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="55e40-1080">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="55e40-1080">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="55e40-1081">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="55e40-1081">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-1082">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-1082">Storage</span></span>

* <span data-ttu-id="55e40-1083">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="55e40-1083">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="55e40-1084">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="55e40-1084">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="55e40-1085">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="55e40-1085">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="55e40-1086">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="55e40-1086">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="55e40-1087">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="55e40-1087">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="55e40-1088">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="55e40-1088">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-1089">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-1089">VM</span></span>

* <span data-ttu-id="55e40-1090">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-1090">Support configuring nsg</span></span>
* <span data-ttu-id="55e40-1091">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="55e40-1091">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="55e40-1092">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="55e40-1092">Support managed service identities</span></span>
* <span data-ttu-id="55e40-1093">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="55e40-1093">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="55e40-1094">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="55e40-1094">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="55e40-1095">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-1095">May 10, 2017</span></span>

<span data-ttu-id="55e40-1096">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="55e40-1096">Version 2.0.6</span></span>

* <span data-ttu-id="55e40-1097">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="55e40-1097">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="55e40-1098">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="55e40-1098">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="55e40-1099">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-1099">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="55e40-1100">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55e40-1100">Include Cognitive Services module</span></span>
* <span data-ttu-id="55e40-1101">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55e40-1101">Include Service Fabric module</span></span>
* <span data-ttu-id="55e40-1102">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="55e40-1102">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="55e40-1103">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="55e40-1103">Add support for CDN commands</span></span>
* <span data-ttu-id="55e40-1104">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="55e40-1104">Remove Container module</span></span>
* <span data-ttu-id="55e40-1105">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="55e40-1105">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="55e40-1106">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="55e40-1106">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="55e40-1107">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-1107">Core</span></span>

* <span data-ttu-id="55e40-1108">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="55e40-1108">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="55e40-1109">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="55e40-1109">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="55e40-1110">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="55e40-1110">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="55e40-1111">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="55e40-1111">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="55e40-1112">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="55e40-1112">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="55e40-1113">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="55e40-1113">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="55e40-1114">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="55e40-1114">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="55e40-1115">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="55e40-1115">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="55e40-1116">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="55e40-1116">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="55e40-1117">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="55e40-1117">core: Improved performance</span></span>
* <span data-ttu-id="55e40-1118">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="55e40-1118">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="55e40-1119">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="55e40-1119">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-1120">ACS</span></span>

* <span data-ttu-id="55e40-1121">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="55e40-1121">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="55e40-1122">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="55e40-1122">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="55e40-1123">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="55e40-1123">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="55e40-1124">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="55e40-1124">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-1125">AppService</span></span>

* <span data-ttu-id="55e40-1126">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="55e40-1126">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="55e40-1127">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="55e40-1127">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="55e40-1128">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="55e40-1128">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="55e40-1129">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="55e40-1129">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="55e40-1130">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="55e40-1130">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="55e40-1131">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="55e40-1131">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="55e40-1132">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="55e40-1132">support slot swap with preview</span></span>
* <span data-ttu-id="55e40-1133">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="55e40-1133">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="55e40-1134">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="55e40-1134">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55e40-1135">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55e40-1135">CosmosDB</span></span>

* <span data-ttu-id="55e40-1136">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="55e40-1136">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="55e40-1137">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="55e40-1137">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="55e40-1138">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="55e40-1138">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="55e40-1139">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="55e40-1139">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55e40-1140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55e40-1140">Data Lake Analytics</span></span>

* <span data-ttu-id="55e40-1141">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="55e40-1141">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="55e40-1142">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="55e40-1142">Add support for new catalog item type: package.</span></span> <span data-ttu-id="55e40-1143">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="55e40-1143">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="55e40-1144">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="55e40-1144">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="55e40-1145">Table</span><span class="sxs-lookup"><span data-stu-id="55e40-1145">Table</span></span>
  * <span data-ttu-id="55e40-1146">Fonction table</span><span class="sxs-lookup"><span data-stu-id="55e40-1146">Table valued function</span></span>
  * <span data-ttu-id="55e40-1147">Affichage</span><span class="sxs-lookup"><span data-stu-id="55e40-1147">View</span></span>
  * <span data-ttu-id="55e40-1148">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="55e40-1148">Table Statistics.</span></span> <span data-ttu-id="55e40-1149">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="55e40-1149">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55e40-1150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-1150">Data Lake Store</span></span>

* <span data-ttu-id="55e40-1151">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="55e40-1151">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="55e40-1152">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="55e40-1152">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="55e40-1153">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="55e40-1153">missed help for access show.</span></span> <span data-ttu-id="55e40-1154">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="55e40-1154">adding it.</span></span> <span data-ttu-id="55e40-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="55e40-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="55e40-1156">Rechercher</span><span class="sxs-lookup"><span data-stu-id="55e40-1156">Find</span></span>

* <span data-ttu-id="55e40-1157">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="55e40-1157">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="55e40-1158">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55e40-1158">KeyVault</span></span>

* <span data-ttu-id="55e40-1159">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="55e40-1159">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="55e40-1160">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="55e40-1160">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="55e40-1161">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="55e40-1161">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="55e40-1162">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="55e40-1162">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="55e40-1163">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="55e40-1163">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="55e40-1164">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1164">Lab</span></span>

* <span data-ttu-id="55e40-1165">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1165">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="55e40-1166">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1166">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="55e40-1167">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1167">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="55e40-1168">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1168">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="55e40-1169">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="55e40-1169">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="55e40-1170">Surveiller</span><span class="sxs-lookup"><span data-stu-id="55e40-1170">Monitor</span></span>

* <span data-ttu-id="55e40-1171">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="55e40-1171">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="55e40-1172">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="55e40-1172">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="55e40-1173">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-1173">Network</span></span>

* <span data-ttu-id="55e40-1174">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="55e40-1174">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="55e40-1175">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1175">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="55e40-1176">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="55e40-1176">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="55e40-1177">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="55e40-1177">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="55e40-1178">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="55e40-1178">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="55e40-1179">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55e40-1179">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="55e40-1180">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="55e40-1180">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="55e40-1181">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="55e40-1181">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="55e40-1182">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="55e40-1182">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="55e40-1183">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="55e40-1183">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="55e40-1184">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="55e40-1184">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="55e40-1185">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1185">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="55e40-1186">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="55e40-1186">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="55e40-1187">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="55e40-1187">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="55e40-1188">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="55e40-1188">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="55e40-1189">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="55e40-1189">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="55e40-1190">Profil</span><span class="sxs-lookup"><span data-stu-id="55e40-1190">Profile</span></span>

* <span data-ttu-id="55e40-1191">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="55e40-1191">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="55e40-1192">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="55e40-1192">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="55e40-1193">Redis</span><span class="sxs-lookup"><span data-stu-id="55e40-1193">Redis</span></span>

* <span data-ttu-id="55e40-1194">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="55e40-1194">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="55e40-1195">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="55e40-1195">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="55e40-1196">Ressource</span><span class="sxs-lookup"><span data-stu-id="55e40-1196">Resource</span></span>

* <span data-ttu-id="55e40-1197">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="55e40-1197">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="55e40-1198">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="55e40-1198">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="55e40-1199">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="55e40-1199">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="55e40-1200">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="55e40-1200">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="55e40-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="55e40-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="55e40-1202">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="55e40-1202">Add docs for az lock update.</span></span> <span data-ttu-id="55e40-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="55e40-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="55e40-1204">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="55e40-1204">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="55e40-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="55e40-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="55e40-1206">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="55e40-1206">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="55e40-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="55e40-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="55e40-1208">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="55e40-1208">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="55e40-1209">Rôle</span><span class="sxs-lookup"><span data-stu-id="55e40-1209">Role</span></span>

* <span data-ttu-id="55e40-1210">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="55e40-1210">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="55e40-1211">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="55e40-1211">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="55e40-1212">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="55e40-1212">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="55e40-1213">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="55e40-1213">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="55e40-1214">SQL</span><span class="sxs-lookup"><span data-stu-id="55e40-1214">SQL</span></span>

* <span data-ttu-id="55e40-1215">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="55e40-1215">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="55e40-1216">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="55e40-1216">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="55e40-1217">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-1217">Storage</span></span>

* <span data-ttu-id="55e40-1218">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="55e40-1218">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="55e40-1219">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="55e40-1219">Add support for incremental blob copy</span></span>
* <span data-ttu-id="55e40-1220">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="55e40-1220">Add support for large block blob upload</span></span>
* <span data-ttu-id="55e40-1221">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="55e40-1221">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-1222">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-1222">VM</span></span>

* <span data-ttu-id="55e40-1223">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="55e40-1223">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="55e40-1224">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="55e40-1224">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="55e40-1225">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="55e40-1225">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="55e40-1226">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="55e40-1226">az vm/vmss disk</span></span>
  3. <span data-ttu-id="55e40-1227">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="55e40-1227">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="55e40-1228">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="55e40-1228">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="55e40-1229">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="55e40-1229">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="55e40-1230">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-1230">April 3, 2017</span></span>

<span data-ttu-id="55e40-1231">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="55e40-1231">Version 2.0.2</span></span>

<span data-ttu-id="55e40-1232">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="55e40-1232">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```
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

### <a name="core"></a><span data-ttu-id="55e40-1233">Principal</span><span class="sxs-lookup"><span data-stu-id="55e40-1233">Core</span></span>

* <span data-ttu-id="55e40-1234">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-1234">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="55e40-1235">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="55e40-1235">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="55e40-1236">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="55e40-1236">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="55e40-1237">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="55e40-1237">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="55e40-1238">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="55e40-1238">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="55e40-1239">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="55e40-1239">Add prompting for missing template parameters.</span></span> <span data-ttu-id="55e40-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="55e40-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="55e40-1241">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="55e40-1241">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="55e40-1242">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="55e40-1242">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="55e40-1243">ACS</span><span class="sxs-lookup"><span data-stu-id="55e40-1243">ACS</span></span>

* <span data-ttu-id="55e40-1244">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="55e40-1244">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="55e40-1245">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="55e40-1245">Add support for ssh key password prompting.</span></span> <span data-ttu-id="55e40-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="55e40-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="55e40-1247">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="55e40-1247">Add support for windows clusters.</span></span> <span data-ttu-id="55e40-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="55e40-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="55e40-1249">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="55e40-1249">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="55e40-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="55e40-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="55e40-1251">AppService</span><span class="sxs-lookup"><span data-stu-id="55e40-1251">AppService</span></span>

* <span data-ttu-id="55e40-1252">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="55e40-1252">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="55e40-1253">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="55e40-1253">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="55e40-1254">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="55e40-1254">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="55e40-1255">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="55e40-1255">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="55e40-1256">DataLake</span><span class="sxs-lookup"><span data-stu-id="55e40-1256">DataLake</span></span>

* <span data-ttu-id="55e40-1257">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55e40-1257">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="55e40-1258">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55e40-1258">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="55e40-1259">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="55e40-1259">DocuemntDB</span></span>

* <span data-ttu-id="55e40-1260">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="55e40-1260">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="55e40-1261">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="55e40-1261">VM</span></span>

* <span data-ttu-id="55e40-1262">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="55e40-1262">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="55e40-1263">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="55e40-1263">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="55e40-1264">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="55e40-1264">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="55e40-1265">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="55e40-1265">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="55e40-1266">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="55e40-1266">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="55e40-1267">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="55e40-1267">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="55e40-1268">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="55e40-1268">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="55e40-1269">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="55e40-1269">February 27, 2017</span></span>

<span data-ttu-id="55e40-1270">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="55e40-1270">Version 2.0.0</span></span>

<span data-ttu-id="55e40-1271">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="55e40-1271">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="55e40-1272">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="55e40-1272">Container Service (acs)</span></span>
- <span data-ttu-id="55e40-1273">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="55e40-1273">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="55e40-1274">Réseau</span><span class="sxs-lookup"><span data-stu-id="55e40-1274">Networking</span></span>
- <span data-ttu-id="55e40-1275">Stockage</span><span class="sxs-lookup"><span data-stu-id="55e40-1275">Storage</span></span>

<span data-ttu-id="55e40-1276">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="55e40-1276">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="55e40-1277">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="55e40-1277">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="55e40-1278">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="55e40-1278">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```
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
> <span data-ttu-id="55e40-1279">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="55e40-1279">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="55e40-1280">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="55e40-1280">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="55e40-1281">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="55e40-1281">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="55e40-1282">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="55e40-1282">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="55e40-1283">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="55e40-1283">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="55e40-1284">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="55e40-1284">Provide feedback from the command line with the `az feedback` command</span></span>

