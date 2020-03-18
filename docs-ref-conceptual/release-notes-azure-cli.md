---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/10/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff3a1da2343b96bfd78b20742c2c15707932f3d7
ms.sourcegitcommit: 21bc2a7125b6c38bf1c4def0a0e66e6673de4805
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2020
ms.locfileid: "79037946"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="c3884-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c3884-103">Azure CLI release notes</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="c3884-104">10 mars 2020</span><span class="sxs-lookup"><span data-stu-id="c3884-104">March 10, 2020</span></span>

<span data-ttu-id="c3884-105">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="c3884-105">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-106">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-106">ACR</span></span>

* <span data-ttu-id="c3884-107">Correctif : `az acr login` déclenche une erreur de manière erronée</span><span class="sxs-lookup"><span data-stu-id="c3884-107">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="c3884-108">Ajout d’une nouvelle commande `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="c3884-108">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="c3884-109">Ajout d’un lien privé et de la prise en charge CMK</span><span class="sxs-lookup"><span data-stu-id="c3884-109">Add private link and CMK support</span></span>
* <span data-ttu-id="c3884-110">Ajout de la commande « private-link-resource list »</span><span class="sxs-lookup"><span data-stu-id="c3884-110">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-111">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-111">AKS</span></span>

* <span data-ttu-id="c3884-112">Correction de la navigation aks dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-112">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="c3884-113">az aks : correction de la supervision des erreurs NoneType addon et agentpool</span><span class="sxs-lookup"><span data-stu-id="c3884-113">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="c3884-114">Ajout de --nodepool-tags au pool de nœuds lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-114">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="c3884-115">Ajout de --tags lors de l’ajout ou de la mise à jour d’un nodepool à un cluster</span><span class="sxs-lookup"><span data-stu-id="c3884-115">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="c3884-116">aks create : ajout de `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="c3884-116">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="c3884-117">Ajout de --nodepool-labels lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-117">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="c3884-118">Ajout de --labels lors de l’ajout d’un nouveau nodepool à un cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-118">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="c3884-119">Ajout d’un caractère / manquant à l’URL de tableau de bord</span><span class="sxs-lookup"><span data-stu-id="c3884-119">add missing / in the dashboard url</span></span>
* <span data-ttu-id="c3884-120">Prise en charge de la création de clusters AKS activant l’identité managée</span><span class="sxs-lookup"><span data-stu-id="c3884-120">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="c3884-121">az aks : validation du plug-in réseau pour qu’il soit « azure » ou « kubenet »</span><span class="sxs-lookup"><span data-stu-id="c3884-121">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="c3884-122">az aks : Ajout de la prise en charge des clés de session AAD</span><span class="sxs-lookup"><span data-stu-id="c3884-122">az aks: Add aad session key support</span></span>
* <span data-ttu-id="c3884-123">[CHANGEMENT CASSANT] az aks : prise en charge des modifications MSI pour GF et BF pour omsagent (supervision de conteneur) (#1)</span><span class="sxs-lookup"><span data-stu-id="c3884-123">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="c3884-124">az aks use-dev-spaces : ajout de l’option de type de point de terminaison à la commande use-dev-spaces pour personnaliser le point de terminaison créé sur un contrôleur Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="c3884-124">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-125">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-125">AppConfig</span></span>

* <span data-ttu-id="c3884-126">Déblocage de l’utilisation de « kv set » pour ajouter la fonctionnalité et la référence de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c3884-126">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-127">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-127">AppService</span></span>

* <span data-ttu-id="c3884-128">az webapp create : résolution d’un problème lors de l’exécution de la commande avec --runtime</span><span class="sxs-lookup"><span data-stu-id="c3884-128">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="c3884-129">az functionapp deployment source config-zip : ajout d’un message d’erreur si le nom du groupe de ressources ou de la fonction n’est pas valide ou n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c3884-129">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="c3884-130">functionapp create : correction du message d’avertissement qui s’affiche aujourd’hui avec `functionapp create`, qui mentionne un indicateur `--functions_version` mais utilise de manière erronée un `_` au lieu d’un `-` dans le nom de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="c3884-130">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="c3884-131">az functionapp create : mise à jour de la façon dont linuxFxVersion et le nom de l’image conteneur étaient définis pour les applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-131">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="c3884-132">az functionapp deployment source config-zip : résolution d’un problème dû à une condition de concurrence en cas de modification des paramètres d’application pendant le déploiement de fichier zip, provoquant des erreurs 5xx lors du déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-132">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="c3884-133">Correctif 5720946 : az webapp backup ne parvient pas à définir le nom</span><span class="sxs-lookup"><span data-stu-id="c3884-133">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-134">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-134">ARM</span></span>

* <span data-ttu-id="c3884-135">az resource : amélioration des exemples du module de ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-135">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="c3884-136">az policy assignment list : prise en charge de l’énumération des affectations de stratégie au niveau de l’étendue du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="c3884-136">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="c3884-137">Ajout de `az deployment group` et `az deployment operation group` pour le déploiement de modèle au niveau des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="c3884-137">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="c3884-138">Il s’agit d’un doublon de `az group deployment` et `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="c3884-138">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="c3884-139">Ajout de `az deployment sub` et `az deployment operation sub` pour le déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3884-139">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="c3884-140">Il s’agit d’un doublon de `az deployment` et `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="c3884-140">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="c3884-141">Ajout de `az deployment mg` et `az deployment operation mg` pour le déploiement de modèle au niveau des groupes de gestion</span><span class="sxs-lookup"><span data-stu-id="c3884-141">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="c3884-142">Ajout de `az deployment tenant` et `az deployment operation tenant` pour le déploiement de modèle à l’étendue du locataire</span><span class="sxs-lookup"><span data-stu-id="c3884-142">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="c3884-143">az policy assignment create : ajout d’une description au paramètre `--location`</span><span class="sxs-lookup"><span data-stu-id="c3884-143">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="c3884-144">az group deployment create : ajout du paramètre `--aux-tenants` pour prendre en charge les locataires croisés</span><span class="sxs-lookup"><span data-stu-id="c3884-144">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-145">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-145">CDN</span></span>

* <span data-ttu-id="c3884-146">Ajouter de commandes WAF CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-146">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-147">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-147">Compute</span></span>

* <span data-ttu-id="c3884-148">az sig image-version : ajout de --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="c3884-148">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="c3884-149">az ppg show: ajout de --colocation-status pour permettre l’extraction de l’état de colocalisation de toutes les ressources dans le groupe de placement de proximité</span><span class="sxs-lookup"><span data-stu-id="c3884-149">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="c3884-150">az vmss create/update : prise en charge des réparations automatiques</span><span class="sxs-lookup"><span data-stu-id="c3884-150">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="c3884-151">[CHANGEMENT CASSANT] az image template : template a été renommé builder</span><span class="sxs-lookup"><span data-stu-id="c3884-151">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="c3884-152">az image builder create : ajout de --image-template</span><span class="sxs-lookup"><span data-stu-id="c3884-152">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c3884-153">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-153">Cosmos DB</span></span>

* <span data-ttu-id="c3884-154">Ajout d’applets de commande de déclencheur, de procédure stockée SQL et de fonctions définies par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c3884-154">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="c3884-155">az cosmosdb create : ajout de --key-uri pour prendre en charge l’ajout d’informations de chiffrement de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c3884-155">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-156">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-156">KeyVault</span></span>

* <span data-ttu-id="c3884-157">keyvault create : activation de la suppression réversible par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-157">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-158">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-158">Monitor</span></span>

* <span data-ttu-id="c3884-159">az monitor metrics alert create : prise en charge de `~` dans `--condition`</span><span class="sxs-lookup"><span data-stu-id="c3884-159">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-160">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-160">Network</span></span>

* <span data-ttu-id="c3884-161">az network application-gateway rewrite-rule create : prise en charge de la configuration d’URL</span><span class="sxs-lookup"><span data-stu-id="c3884-161">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="c3884-162">az network dns zone import : --zone-name respectera la casse à l’avenir</span><span class="sxs-lookup"><span data-stu-id="c3884-162">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="c3884-163">az network private-endpoint/private-link-service : suppression de l’étiquette d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c3884-163">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="c3884-164">az network bastion : prise en charge de bastion</span><span class="sxs-lookup"><span data-stu-id="c3884-164">az network bastion: support bastion</span></span>
* <span data-ttu-id="c3884-165">az network vnet list-available-ips : prise en charge de l’énumération des adresses IP disponibles sur un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c3884-165">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="c3884-166">az network watcher flow-log create/list/delete/update : ajout de nouvelles commandes pour gérer le journal de flux d’observateur et l’exposition de --location pour identifier explicitement l’observateur</span><span class="sxs-lookup"><span data-stu-id="c3884-166">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="c3884-167">az network watcher flow-log configure : dépréciée</span><span class="sxs-lookup"><span data-stu-id="c3884-167">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="c3884-168">az network watcher flow-log show : prise en charge de --location et de --name pour obtenir un résultat au format ARM. L’ancienne sortie mise en forme est dépréciée</span><span class="sxs-lookup"><span data-stu-id="c3884-168">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="c3884-169">Stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-169">Policy</span></span>

* <span data-ttu-id="c3884-170">az policy assignment create : correction du bogue qui générait automatiquement un nom d’attribution de stratégie dépassant la limite</span><span class="sxs-lookup"><span data-stu-id="c3884-170">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-171">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-171">RBAC</span></span>

* <span data-ttu-id="c3884-172">az ad group show : correction du bogue qui faisait que --group était traité comme un problème Regex</span><span class="sxs-lookup"><span data-stu-id="c3884-172">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-173">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-173">RDBMS</span></span>

* <span data-ttu-id="c3884-174">Passage du SDK azure-mgmt-rdbms à la version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-174">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="c3884-175">az postgres private-endpoint-connection : gestion des connexions de point de terminaison privé postgres</span><span class="sxs-lookup"><span data-stu-id="c3884-175">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="c3884-176">az postgres private-link-resource : gestion des ressources de lien privé postgres</span><span class="sxs-lookup"><span data-stu-id="c3884-176">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="c3884-177">az mysql private-endpoint-connection : gestion des connexions de point de terminaison privé mysql</span><span class="sxs-lookup"><span data-stu-id="c3884-177">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="c3884-178">az mysql private-link-resource : gestion des ressources de lien privé mysql</span><span class="sxs-lookup"><span data-stu-id="c3884-178">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="c3884-179">az mariadb private-endpoint-connection : gestion des connexions de point de terminaison privé mariadb</span><span class="sxs-lookup"><span data-stu-id="c3884-179">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="c3884-180">az mariadb private-link-resource : gestion des ressources de lien privé mariadb</span><span class="sxs-lookup"><span data-stu-id="c3884-180">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="c3884-181">Mise à jour des tests de point de terminaison privé SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-181">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-182">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-182">SQL</span></span>

* <span data-ttu-id="c3884-183">Sql midb ; ajout de list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="c3884-183">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="c3884-184">(sql server create :) Ajout de l’indicateur facultatif « Enable »/« Disable » d’accès au réseau public à sql server create</span><span class="sxs-lookup"><span data-stu-id="c3884-184">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="c3884-185">(sql server update :) modifications du client</span><span class="sxs-lookup"><span data-stu-id="c3884-185">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="c3884-186">Ajout de propriété minimal_tls_version pour MI et SQL DB</span><span class="sxs-lookup"><span data-stu-id="c3884-186">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-187">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-187">Storage</span></span>

* <span data-ttu-id="c3884-188">az storage blob delete-batch : comportement incorrect de l’indicateur `--dryrun`</span><span class="sxs-lookup"><span data-stu-id="c3884-188">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="c3884-189">az storage account network-rule add (correctif de bogue) : l’opération d’ajout doit être idempotent</span><span class="sxs-lookup"><span data-stu-id="c3884-189">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="c3884-190">az storage account create/update : Ajout de la prise en charge des préférences de routage</span><span class="sxs-lookup"><span data-stu-id="c3884-190">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="c3884-191">Mise à niveau de la version azure-mgmt-storage vers 8.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-191">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="c3884-192">az storage container immutability create : ajout du paramètre --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="c3884-192">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="c3884-193">az storage account private-link-resource list : ajout de la prise en charge de l’énumération des ressources de lien privé pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-193">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="c3884-194">az storage account private-endpoint-connection approve/reject/show/delete : prise en charge de la gestion des connexions de point de terminaison privé</span><span class="sxs-lookup"><span data-stu-id="c3884-194">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="c3884-195">az storage account blob-service-properties update : ajout de --enable-restore-policy et --restore-days</span><span class="sxs-lookup"><span data-stu-id="c3884-195">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="c3884-196">az storage blob restore : ajout de la prise en charge de la restauration des plages d’objets blob</span><span class="sxs-lookup"><span data-stu-id="c3884-196">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="c3884-197">18 février 2020</span><span class="sxs-lookup"><span data-stu-id="c3884-197">February 18, 2020</span></span>

<span data-ttu-id="c3884-198">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="c3884-198">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-199">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-199">ACR</span></span>

* <span data-ttu-id="c3884-200">Ajoute un nouvel argument `--expose-token` pour `az acr login`</span><span class="sxs-lookup"><span data-stu-id="c3884-200">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="c3884-201">Corrige la sortie incorrecte de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="c3884-201">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="c3884-202">az acr login : lève une CLIError si des erreurs sont retournées par la commande docker</span><span class="sxs-lookup"><span data-stu-id="c3884-202">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-203">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-203">ACS</span></span>

* <span data-ttu-id="c3884-204">aks create/update : ajoute la validation `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="c3884-204">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="c3884-205">Aladdin</span><span class="sxs-lookup"><span data-stu-id="c3884-205">Aladdin</span></span>

* <span data-ttu-id="c3884-206">Analyse les exemples générés dans le _help.py des commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-206">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-207">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-207">AMS</span></span>

* <span data-ttu-id="c3884-208">az ams est désormais en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="c3884-208">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-209">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-209">AppConfig</span></span>

* <span data-ttu-id="c3884-210">Modifie le message d’aide pour exclure les filtres de clé ou d’étiquette non pris en charge</span><span class="sxs-lookup"><span data-stu-id="c3884-210">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="c3884-211">Supprimer l’étiquette d’aperçu pour la plupart des commandes, à l’exception des indicateurs d’identité managée et de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c3884-211">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="c3884-212">Ajoute une clé gérée par le client lors de la mise à jour des magasins</span><span class="sxs-lookup"><span data-stu-id="c3884-212">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-213">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-213">AppService</span></span>

* <span data-ttu-id="c3884-214">az webapp list-runtimes : correction du bogue concernant list-runtimes</span><span class="sxs-lookup"><span data-stu-id="c3884-214">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="c3884-215">Ajoute az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="c3884-215">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="c3884-216">Ajoute la prise en charge des applications de fonction v3 et du nœud 12</span><span class="sxs-lookup"><span data-stu-id="c3884-216">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-217">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-217">ARM</span></span>

* <span data-ttu-id="c3884-218">az policy assignment create : correction du message d’erreur lorsque le paramètre `--policy` n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="c3884-218">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="c3884-219">az group deployment create : correction de l’erreur « stat: path too long for Windows » (Chemin trop long pour Windows) lors de l’utilisation d’un fichier parameters.json volumineux</span><span class="sxs-lookup"><span data-stu-id="c3884-219">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-220">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-220">Backup</span></span>

* <span data-ttu-id="c3884-221">Correction du flux de récupération au niveau de l’élément dans OLR</span><span class="sxs-lookup"><span data-stu-id="c3884-221">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="c3884-222">Ajout de la prise en charge de la restauration sous forme de fichiers pour les bases de données SQL et SAP</span><span class="sxs-lookup"><span data-stu-id="c3884-222">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-223">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-223">Compute</span></span>

* <span data-ttu-id="c3884-224">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="c3884-224">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="c3884-225">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="c3884-225">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="c3884-226">az vm host : supprime l’étiquette d’aperçu pour `vm host` et `vm host group`</span><span class="sxs-lookup"><span data-stu-id="c3884-226">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="c3884-227">[CHANGEMENT CASSANT] Correctif n° 10728 : `az vm create` Création automatique d’un sous-réseau si un réseau virtuel est spécifié et s’il n’existe pas de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-227">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="c3884-228">Amélioration de la robustesse de la liste d’images de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="c3884-228">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="c3884-229">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="c3884-229">Eventhub</span></span>

* <span data-ttu-id="c3884-230">Prise en charge d’Azure Stack pour le profil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="c3884-230">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-231">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-231">KeyVault</span></span>

* <span data-ttu-id="c3884-232">az keyvault key create : ajouter une nouvelle valeur `import` pour le paramètre `--ops`</span><span class="sxs-lookup"><span data-stu-id="c3884-232">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="c3884-233">az keyvault key list-versions : prise en charge du paramètre `--id` pour la spécification des clés</span><span class="sxs-lookup"><span data-stu-id="c3884-233">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="c3884-234">Prise en charge des connexions de points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="c3884-234">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="c3884-235">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-235">Network</span></span>

* <span data-ttu-id="c3884-236">Passage à azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-236">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="c3884-237">az network private-link-service update/create: support --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="c3884-237">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="c3884-238">Ajout de la fonctionnalité Moniteur de connexion v2</span><span class="sxs-lookup"><span data-stu-id="c3884-238">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="c3884-239">Packaging</span><span class="sxs-lookup"><span data-stu-id="c3884-239">Packaging</span></span>

* <span data-ttu-id="c3884-240">[CHANGEMENT CASSANT] Python 2.7 n’est plus pris en charge</span><span class="sxs-lookup"><span data-stu-id="c3884-240">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-241">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-241">Profile</span></span>

* <span data-ttu-id="c3884-242">Aperçu : Ajoutez les nouveaux attributs `homeTenantId` et `managedByTenants` aux comptes d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3884-242">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="c3884-243">Réexécutez `az login` pour que les modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="c3884-243">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="c3884-244">az login : affiche un avertissement lorsqu’un abonnement est listé par plusieurs locataires et s’affiche par défaut pour le premier.</span><span class="sxs-lookup"><span data-stu-id="c3884-244">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="c3884-245">Pour sélectionner un locataire lors de l’accès à cet abonnement, ajoutez `--tenant` dans `az login`</span><span class="sxs-lookup"><span data-stu-id="c3884-245">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="c3884-246">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-246">Role</span></span>

* <span data-ttu-id="c3884-247">az role assignment create : correction de l’erreur lors de laquelle l’attribution d’un rôle à un principal de service par nom d’affichage générait une erreur HTTP 400</span><span class="sxs-lookup"><span data-stu-id="c3884-247">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-248">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-248">SQL</span></span>

* <span data-ttu-id="c3884-249">Mise à jour de l’applet de commande SQL Managed Instance `az sql mi update` avec deux nouveaux paramètres : tier et family</span><span class="sxs-lookup"><span data-stu-id="c3884-249">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-250">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-250">Storage</span></span>

* <span data-ttu-id="c3884-251">[CHANGEMENT CASSANT] `az storage account create` : Remplacement du type de compte de stockage par défaut par StorageV2</span><span class="sxs-lookup"><span data-stu-id="c3884-251">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="c3884-252">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="c3884-252">February 04, 2020</span></span>

<span data-ttu-id="c3884-253">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="c3884-253">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-254">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-254">ACS</span></span>

* <span data-ttu-id="c3884-255">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="c3884-255">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="c3884-256">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="c3884-256">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-257">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-257">ACR</span></span>

* <span data-ttu-id="c3884-258">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="c3884-258">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="c3884-259">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="c3884-259">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="c3884-260">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="c3884-260">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-261">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-261">AKS</span></span>

* <span data-ttu-id="c3884-262">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="c3884-262">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-263">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-263">AppConfig</span></span>

* <span data-ttu-id="c3884-264">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="c3884-264">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="c3884-265">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="c3884-265">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="c3884-266">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="c3884-266">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="c3884-267">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="c3884-267">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="c3884-268">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="c3884-268">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-269">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-269">AppService</span></span>

* <span data-ttu-id="c3884-270">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="c3884-270">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="c3884-271">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-271">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-272">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-272">ARM</span></span>

* <span data-ttu-id="c3884-273">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-273">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="c3884-274">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="c3884-274">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="c3884-275">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="c3884-275">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="c3884-276">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="c3884-276">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="c3884-277">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="c3884-277">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="c3884-278">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="c3884-278">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="c3884-279">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="c3884-279">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-280">BotService</span><span class="sxs-lookup"><span data-stu-id="c3884-280">BotService</span></span>

* <span data-ttu-id="c3884-281">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="c3884-281">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="c3884-282">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="c3884-282">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-283">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-283">CDN</span></span>

* <span data-ttu-id="c3884-284">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="c3884-284">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="c3884-285">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="c3884-285">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="c3884-286">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="c3884-286">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="c3884-287">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-287">Deployment Manager</span></span>

* <span data-ttu-id="c3884-288">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="c3884-288">Add list operation for all resources.</span></span>
* <span data-ttu-id="c3884-289">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="c3884-289">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="c3884-290">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="c3884-290">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-291">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-291">IoT</span></span>

* <span data-ttu-id="c3884-292">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="c3884-292">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="c3884-293">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c3884-293">IoT Central</span></span>

* <span data-ttu-id="c3884-294">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="c3884-294">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-295">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-295">Key Vault</span></span>

* <span data-ttu-id="c3884-296">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="c3884-296">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="c3884-297">Divers</span><span class="sxs-lookup"><span data-stu-id="c3884-297">Misc</span></span>

* <span data-ttu-id="c3884-298">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="c3884-298">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="c3884-299">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-299">Network</span></span>

* <span data-ttu-id="c3884-300">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="c3884-300">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="c3884-301">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="c3884-301">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="c3884-302">Stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-302">Policy</span></span>

* <span data-ttu-id="c3884-303">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="c3884-303">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="c3884-304">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="c3884-304">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-305">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-305">Profile</span></span>

* <span data-ttu-id="c3884-306">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-306">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-307">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-307">RBAC</span></span>

* <span data-ttu-id="c3884-308">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-308">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="c3884-309">Sécurité</span><span class="sxs-lookup"><span data-stu-id="c3884-309">Security</span></span>

* <span data-ttu-id="c3884-310">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="c3884-310">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-311">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-311">SQL</span></span>

* <span data-ttu-id="c3884-312">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="c3884-312">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="c3884-313">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="c3884-313">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="c3884-314">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="c3884-314">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="c3884-315">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="c3884-315">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="c3884-316">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="c3884-316">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="c3884-317">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="c3884-317">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-318">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-318">Storage</span></span>

* <span data-ttu-id="c3884-319">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="c3884-319">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="c3884-320">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="c3884-320">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="c3884-321">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="c3884-321">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="c3884-322">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="c3884-322">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="c3884-323">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="c3884-323">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="c3884-324">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="c3884-324">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="c3884-325">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c3884-325">ServiceFabric</span></span>

* <span data-ttu-id="c3884-326">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="c3884-326">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="c3884-327">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="c3884-327">January 13, 2020</span></span>

<span data-ttu-id="c3884-328">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="c3884-328">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-329">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-329">Compute</span></span>

* <span data-ttu-id="c3884-330">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="c3884-330">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="c3884-331">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="c3884-331">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-332">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-332">Storage</span></span>

* <span data-ttu-id="c3884-333">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="c3884-333">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="c3884-334">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="c3884-334">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="c3884-335">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="c3884-335">January 07, 2020</span></span>

<span data-ttu-id="c3884-336">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="c3884-336">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-337">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-337">ACR</span></span>

* <span data-ttu-id="c3884-338">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="c3884-338">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="c3884-339">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="c3884-339">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-340">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-340">AppConfig</span></span>

* <span data-ttu-id="c3884-341">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="c3884-341">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="c3884-342">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-342">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="c3884-343">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="c3884-343">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-344">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-344">AppService</span></span>

* <span data-ttu-id="c3884-345">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="c3884-345">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="c3884-346">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-346">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="c3884-347">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="c3884-347">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-348">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-348">ARM</span></span>

* <span data-ttu-id="c3884-349">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="c3884-349">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-350">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-350">Backup</span></span>

* <span data-ttu-id="c3884-351">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="c3884-351">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="c3884-352">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="c3884-352">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="c3884-353">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="c3884-353">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-354">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-354">Compute</span></span>

* <span data-ttu-id="c3884-355">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c3884-355">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="c3884-356">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="c3884-356">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="c3884-357">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="c3884-357">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-358">HDInsight</span></span>

* <span data-ttu-id="c3884-359">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="c3884-359">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="c3884-360">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="c3884-360">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="c3884-361">Divers</span><span class="sxs-lookup"><span data-stu-id="c3884-361">Misc.</span></span>

* <span data-ttu-id="c3884-362">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="c3884-362">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="c3884-363">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="c3884-363">Event Hubs</span></span>

* <span data-ttu-id="c3884-364">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="c3884-364">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="c3884-365">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="c3884-365">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="c3884-366">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-366">Service Bus</span></span>

* <span data-ttu-id="c3884-367">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="c3884-367">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="c3884-368">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="c3884-368">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-369">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-369">RBAC</span></span>

* <span data-ttu-id="c3884-370">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c3884-370">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-371">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-371">Storage</span></span>

* <span data-ttu-id="c3884-372">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="c3884-372">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="c3884-373">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="c3884-373">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="c3884-374">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="c3884-374">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="c3884-375">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-375">December 17, 2019</span></span>

<span data-ttu-id="c3884-376">2.0.78</span><span class="sxs-lookup"><span data-stu-id="c3884-376">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-377">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-377">ACR</span></span>

* <span data-ttu-id="c3884-378">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="c3884-378">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-379">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-379">ACS</span></span>

* <span data-ttu-id="c3884-380">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="c3884-380">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-381">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-381">AMS</span></span>

* <span data-ttu-id="c3884-382">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="c3884-382">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-383">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-383">AppConfig</span></span>

* <span data-ttu-id="c3884-384">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="c3884-384">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="c3884-385">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="c3884-385">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="c3884-386">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="c3884-386">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-387">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-387">AppService</span></span>

* <span data-ttu-id="c3884-388">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="c3884-388">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="c3884-389">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="c3884-389">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="c3884-390">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="c3884-390">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="c3884-391">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="c3884-391">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-392">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-392">ARM</span></span>

* <span data-ttu-id="c3884-393">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-393">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="c3884-394">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="c3884-394">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="c3884-395">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="c3884-395">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-396">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-396">Backup</span></span>

* <span data-ttu-id="c3884-397">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="c3884-397">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-398">BotService</span><span class="sxs-lookup"><span data-stu-id="c3884-398">BotService</span></span>

* <span data-ttu-id="c3884-399">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="c3884-399">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="c3884-400">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="c3884-400">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="c3884-401">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="c3884-401">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="c3884-402">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="c3884-402">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="c3884-403">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="c3884-403">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="c3884-404">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="c3884-404">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="c3884-405">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="c3884-405">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="c3884-406">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="c3884-406">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="c3884-407">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="c3884-407">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-408">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-408">Compute</span></span>

* <span data-ttu-id="c3884-409">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="c3884-409">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="c3884-410">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="c3884-410">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="c3884-411">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="c3884-411">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="c3884-412">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="c3884-412">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="c3884-413">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="c3884-413">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="c3884-414">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="c3884-414">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="c3884-415">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-415">Core</span></span>

* <span data-ttu-id="c3884-416">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="c3884-416">Removed support for Python 3.4</span></span>
* <span data-ttu-id="c3884-417">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-417">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="c3884-418">DLS</span><span class="sxs-lookup"><span data-stu-id="c3884-418">DLS</span></span>

* <span data-ttu-id="c3884-419">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="c3884-419">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="c3884-420">Installer</span><span class="sxs-lookup"><span data-stu-id="c3884-420">Install</span></span>

* <span data-ttu-id="c3884-421">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="c3884-421">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-422">IOT</span><span class="sxs-lookup"><span data-stu-id="c3884-422">IOT</span></span>

* <span data-ttu-id="c3884-423">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="c3884-423">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="c3884-424">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="c3884-424">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-425">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-425">Key Vault</span></span>

* <span data-ttu-id="c3884-426">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-426">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="c3884-427">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="c3884-427">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="c3884-428">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="c3884-428">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="c3884-429">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c3884-429">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="c3884-430">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="c3884-430">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-431">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-431">Network</span></span>

* <span data-ttu-id="c3884-432">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-432">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="c3884-433">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-433">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="c3884-434">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="c3884-434">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="c3884-435">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="c3884-435">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="c3884-436">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="c3884-436">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="c3884-437">Packaging</span><span class="sxs-lookup"><span data-stu-id="c3884-437">Packaging</span></span>

* <span data-ttu-id="c3884-438">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="c3884-438">Added back edge builds for pip install</span></span>
* <span data-ttu-id="c3884-439">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="c3884-439">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="c3884-440">Stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-440">Policy</span></span>

* <span data-ttu-id="c3884-441">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="c3884-441">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="c3884-442">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="c3884-442">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="c3884-443">Redis</span><span class="sxs-lookup"><span data-stu-id="c3884-443">Redis</span></span>

* <span data-ttu-id="c3884-444">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="c3884-444">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="c3884-445">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="c3884-445">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="c3884-446">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c3884-446">ServiceFabric</span></span>

* <span data-ttu-id="c3884-447">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="c3884-447">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="c3884-448">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="c3884-448">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-449">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-449">SQL</span></span>

* <span data-ttu-id="c3884-450">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="c3884-450">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-451">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-451">Storage</span></span>

* <span data-ttu-id="c3884-452">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="c3884-452">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="c3884-453">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="c3884-453">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="c3884-454">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="c3884-454">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="c3884-455">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="c3884-455">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="c3884-456">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="c3884-456">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="c3884-457">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-457">November 26, 2019</span></span>

<span data-ttu-id="c3884-458">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="c3884-458">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-459">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-459">ACR</span></span>

* <span data-ttu-id="c3884-460">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="c3884-460">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="c3884-461">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="c3884-461">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="c3884-462">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="c3884-462">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="c3884-463">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="c3884-463">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-464">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-464">AKS</span></span>

* <span data-ttu-id="c3884-465">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="c3884-465">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-466">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-466">AppConfig</span></span>

* <span data-ttu-id="c3884-467">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="c3884-467">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="c3884-468">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="c3884-468">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="c3884-469">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="c3884-469">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="c3884-470">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-470">AppService</span></span>

* <span data-ttu-id="c3884-471">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="c3884-471">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="c3884-472">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="c3884-472">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="c3884-473">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="c3884-473">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-474">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-474">Backup</span></span>

* <span data-ttu-id="c3884-475">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="c3884-475">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="c3884-476">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3884-476">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-477">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-477">Compute</span></span>

* <span data-ttu-id="c3884-478">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="c3884-478">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="c3884-479">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="c3884-479">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="c3884-480">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="c3884-480">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="c3884-481">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="c3884-481">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="c3884-482">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="c3884-482">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="c3884-483">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="c3884-483">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="c3884-484">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-484">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="c3884-485">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="c3884-485">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="c3884-486">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="c3884-486">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="c3884-487">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="c3884-487">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-488">IOT</span><span class="sxs-lookup"><span data-stu-id="c3884-488">IOT</span></span>

* <span data-ttu-id="c3884-489">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="c3884-489">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="c3884-490">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="c3884-490">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="c3884-491">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="c3884-491">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-492">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-492">Key Vault</span></span>

* <span data-ttu-id="c3884-493">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="c3884-493">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="c3884-494">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="c3884-494">NetAppFiles</span></span>

* <span data-ttu-id="c3884-495">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="c3884-495">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="c3884-496">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-496">Network</span></span>

* <span data-ttu-id="c3884-497">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="c3884-497">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="c3884-498">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="c3884-498">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="c3884-499">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="c3884-499">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="c3884-500">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="c3884-500">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="c3884-501">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="c3884-501">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="c3884-502">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="c3884-502">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="c3884-503">Packaging</span><span class="sxs-lookup"><span data-stu-id="c3884-503">Packaging</span></span>

* <span data-ttu-id="c3884-504">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="c3884-504">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="c3884-505">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="c3884-505">Added support for Python 3.8</span></span>
* <span data-ttu-id="c3884-506">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="c3884-506">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-507">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-507">Profile</span></span>

* <span data-ttu-id="c3884-508">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="c3884-508">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="c3884-509">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="c3884-509">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="c3884-510">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="c3884-510">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="c3884-511">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="c3884-511">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="c3884-512">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="c3884-512">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-513">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-513">RBAC</span></span>

* <span data-ttu-id="c3884-514">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c3884-514">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="c3884-515">Redis</span><span class="sxs-lookup"><span data-stu-id="c3884-515">Redis</span></span>

* <span data-ttu-id="c3884-516">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="c3884-516">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="c3884-517">Réservations</span><span class="sxs-lookup"><span data-stu-id="c3884-517">Reservations</span></span>

* <span data-ttu-id="c3884-518">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="c3884-518">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="c3884-519">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="c3884-519">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="c3884-520">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="c3884-520">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="c3884-521">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="c3884-521">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="c3884-522">Rest</span><span class="sxs-lookup"><span data-stu-id="c3884-522">Rest</span></span>
* <span data-ttu-id="c3884-523">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c3884-523">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-524">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-524">SQL</span></span>

* <span data-ttu-id="c3884-525">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="c3884-525">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-526">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-526">Storage</span></span>

* <span data-ttu-id="c3884-527">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="c3884-527">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="c3884-528">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-528">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="c3884-529">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="c3884-529">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="c3884-530">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="c3884-530">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="c3884-531">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-531">November 4, 2019</span></span>

<span data-ttu-id="c3884-532">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="c3884-532">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-533">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-533">ACR</span></span>

* <span data-ttu-id="c3884-534">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="c3884-534">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="c3884-535">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="c3884-535">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="c3884-536">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="c3884-536">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-537">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-537">AKS</span></span>

* <span data-ttu-id="c3884-538">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="c3884-538">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="c3884-539">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="c3884-539">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="c3884-540">AppConfig</span><span class="sxs-lookup"><span data-stu-id="c3884-540">AppConfig</span></span>

* <span data-ttu-id="c3884-541">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="c3884-541">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="c3884-542">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="c3884-542">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="c3884-543">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="c3884-543">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-544">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-544">AppService</span></span>

* <span data-ttu-id="c3884-545">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="c3884-545">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="c3884-546">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-546">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="c3884-547">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="c3884-547">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="c3884-548">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-548">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="c3884-549">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="c3884-549">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-550">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-550">ARM</span></span>

* <span data-ttu-id="c3884-551">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="c3884-551">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="c3884-552">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="c3884-552">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-553">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-553">Backup</span></span>

* <span data-ttu-id="c3884-554">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="c3884-554">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-555">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-555">Compute</span></span>

* <span data-ttu-id="c3884-556">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="c3884-556">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="c3884-557">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="c3884-557">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="c3884-558">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="c3884-558">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="c3884-559">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="c3884-559">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="c3884-560">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="c3884-560">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="c3884-561">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c3884-561">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="c3884-562">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="c3884-562">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="c3884-563">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="c3884-563">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-564">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-564">CosmosDB</span></span>

* <span data-ttu-id="c3884-565">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="c3884-565">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="c3884-566">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="c3884-566">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="c3884-567">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-567">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="c3884-568">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="c3884-568">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="c3884-569">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-569">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="c3884-570">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="c3884-570">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="c3884-571">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-571">Fixed typo in help message</span></span>
* <span data-ttu-id="c3884-572">base de données : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="c3884-572">database: Added deprecation information</span></span>
* <span data-ttu-id="c3884-573">collection : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="c3884-573">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-574">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-574">IoT</span></span>

* <span data-ttu-id="c3884-575">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="c3884-575">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="c3884-576">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="c3884-576">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-577">Key Vault</span></span>

* <span data-ttu-id="c3884-578">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c3884-578">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="c3884-579">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-579">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="c3884-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="c3884-580">NetAppFiles</span></span>

* <span data-ttu-id="c3884-581">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="c3884-581">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="c3884-582">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c3884-582">This new API version includes:</span></span>

    - <span data-ttu-id="c3884-583">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="c3884-583">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="c3884-584">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="c3884-584">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="c3884-585">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="c3884-585">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="c3884-586">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="c3884-586">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="c3884-587">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-587">Network</span></span>

* <span data-ttu-id="c3884-588">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="c3884-588">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="c3884-589">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="c3884-589">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="c3884-590">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="c3884-590">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="c3884-591">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="c3884-591">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="c3884-592">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="c3884-592">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="c3884-593">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="c3884-593">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-594">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-594">Profile</span></span>

* <span data-ttu-id="c3884-595">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-595">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="c3884-596">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="c3884-596">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-597">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-597">RBAC</span></span>

* <span data-ttu-id="c3884-598">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-598">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="c3884-599">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c3884-599">ServiceFabric</span></span>

* <span data-ttu-id="c3884-600">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="c3884-600">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-601">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-601">SQL</span></span>

* <span data-ttu-id="c3884-602">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="c3884-602">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-603">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-603">Storage</span></span>

* <span data-ttu-id="c3884-604">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="c3884-604">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="c3884-605">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="c3884-605">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="c3884-606">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-606">October 15, 2019</span></span>

<span data-ttu-id="c3884-607">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="c3884-607">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-608">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-608">AKS</span></span>

* <span data-ttu-id="c3884-609">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-609">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="c3884-610">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-610">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-611">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-611">AMS</span></span>

* <span data-ttu-id="c3884-612">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="c3884-612">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="c3884-613">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="c3884-613">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-614">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-614">AppService</span></span>

* <span data-ttu-id="c3884-615">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="c3884-615">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="c3884-616">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-616">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="c3884-617">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="c3884-617">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-618">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-618">ARM</span></span>

* <span data-ttu-id="c3884-619">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="c3884-619">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-620">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-620">Compute</span></span>

* <span data-ttu-id="c3884-621">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-621">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="c3884-622">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="c3884-622">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="c3884-623">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-623">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="c3884-624">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="c3884-624">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="c3884-625">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-625">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="c3884-626">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="c3884-626">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="c3884-627">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-627">Core</span></span>

* <span data-ttu-id="c3884-628">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c3884-628">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-629">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-629">IoT</span></span>

* <span data-ttu-id="c3884-630">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="c3884-630">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-631">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-631">Monitor</span></span>

* <span data-ttu-id="c3884-632">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="c3884-632">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-633">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-633">Network</span></span>

* <span data-ttu-id="c3884-634">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-634">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="c3884-635">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-635">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-636">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-636">SQL</span></span>

* <span data-ttu-id="c3884-637">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="c3884-637">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-638">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-638">Storage</span></span>

* <span data-ttu-id="c3884-639">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="c3884-639">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="c3884-640">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-640">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="c3884-641">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-641">September 24, 2019</span></span>

<span data-ttu-id="c3884-642">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="c3884-642">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-643">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-643">ACR</span></span>

* <span data-ttu-id="c3884-644">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="c3884-644">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="c3884-645">[CHANGEMENT CASSANT] Renommage du paramètre `--name -n` en `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="c3884-645">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-646">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-646">AKS</span></span>

* <span data-ttu-id="c3884-647">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="c3884-647">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="c3884-648">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="c3884-648">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="c3884-649">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="c3884-649">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-650">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-650">ARM</span></span>

* <span data-ttu-id="c3884-651">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="c3884-651">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-652">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-652">Compute</span></span>

* <span data-ttu-id="c3884-653">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="c3884-653">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="c3884-654">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="c3884-654">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="c3884-655">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-655">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="c3884-656">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="c3884-656">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="c3884-657">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="c3884-657">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c3884-658">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-658">Cosmos DB</span></span>

* <span data-ttu-id="c3884-659">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="c3884-659">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="c3884-660">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="c3884-660">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="c3884-661">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="c3884-661">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c3884-662">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c3884-662">EventGrid</span></span>

* <span data-ttu-id="c3884-663">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="c3884-663">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-664">Key Vault</span></span>

* <span data-ttu-id="c3884-665">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="c3884-665">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-666">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-666">Monitor</span></span>

* <span data-ttu-id="c3884-667">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="c3884-667">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="c3884-668">Stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-668">Policy</span></span>

* <span data-ttu-id="c3884-669">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="c3884-669">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="c3884-670">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c3884-670">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-671">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-671">Storage</span></span>

* <span data-ttu-id="c3884-672">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="c3884-672">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="c3884-673">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-673">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-674">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-674">ACR</span></span>

* <span data-ttu-id="c3884-675">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="c3884-675">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-676">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-676">AKS</span></span>

* <span data-ttu-id="c3884-677">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3884-677">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="c3884-678">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-678">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="c3884-679">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-679">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-680">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-680">ARM</span></span>

* <span data-ttu-id="c3884-681">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="c3884-681">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-682">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-682">Batch</span></span>

* <span data-ttu-id="c3884-683">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="c3884-683">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="c3884-684">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="c3884-684">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="c3884-685">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="c3884-685">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="c3884-686">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="c3884-686">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="c3884-687">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="c3884-687">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="c3884-688">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="c3884-688">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="c3884-689">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="c3884-689">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-690">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-690">HDInsight</span></span>

* <span data-ttu-id="c3884-691">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c3884-691">GA release</span></span>
* <span data-ttu-id="c3884-692">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3884-692">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-693">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-693">Key Vault</span></span>

* <span data-ttu-id="c3884-694">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-694">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="c3884-695">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-695">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="c3884-696">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-696">Network</span></span>

* <span data-ttu-id="c3884-697">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="c3884-697">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="c3884-698">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="c3884-698">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="c3884-699">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="c3884-699">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="c3884-700">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="c3884-700">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="c3884-701">Stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-701">Policy</span></span>

* <span data-ttu-id="c3884-702">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="c3884-702">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="c3884-703">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-703">August 27, 2019</span></span>

<span data-ttu-id="c3884-704">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="c3884-704">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-705">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-705">ACR</span></span>

* <span data-ttu-id="c3884-706">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="c3884-706">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="c3884-707">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="c3884-707">API Management</span></span>

* <span data-ttu-id="c3884-708">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="c3884-708">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-709">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-709">AppService</span></span>

* <span data-ttu-id="c3884-710">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="c3884-710">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="c3884-711">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-711">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-712">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-712">Keyvault</span></span>

* <span data-ttu-id="c3884-713">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="c3884-713">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="c3884-714">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-714">Network</span></span>

* <span data-ttu-id="c3884-715">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="c3884-715">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="c3884-716">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="c3884-716">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="c3884-717">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="c3884-717">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="c3884-718">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c3884-718">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-719">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-719">RBAC</span></span>

* <span data-ttu-id="c3884-720">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-720">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="c3884-721">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c3884-721">ServiceFabric</span></span>

* <span data-ttu-id="c3884-722">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="c3884-722">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="c3884-723">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-723">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="c3884-724">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="c3884-724">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="c3884-725">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c3884-725">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="c3884-726">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-726">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="c3884-727">SignalR</span><span class="sxs-lookup"><span data-stu-id="c3884-727">SignalR</span></span>

* <span data-ttu-id="c3884-728">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="c3884-728">Added new commands:</span></span>
  * <span data-ttu-id="c3884-729">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="c3884-729">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="c3884-730">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="c3884-730">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="c3884-731">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="c3884-731">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="c3884-732">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="c3884-732">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-733">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-733">Storage</span></span>

* <span data-ttu-id="c3884-734">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="c3884-734">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="c3884-735">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-735">August 13, 2019</span></span>

<span data-ttu-id="c3884-736">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="c3884-736">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-737">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-737">AppService</span></span>

* <span data-ttu-id="c3884-738">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="c3884-738">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-739">BotService</span><span class="sxs-lookup"><span data-stu-id="c3884-739">BotService</span></span>

* <span data-ttu-id="c3884-740">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="c3884-740">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="c3884-741">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c3884-741">CognitiveServices</span></span>

* <span data-ttu-id="c3884-742">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-742">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c3884-743">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-743">Cosmos DB</span></span>

* <span data-ttu-id="c3884-744">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="c3884-744">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="c3884-745">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-745">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-746">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-746">HDInsight</span></span>

<span data-ttu-id="c3884-747">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="c3884-747">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="c3884-748">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="c3884-748">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="c3884-749">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="c3884-749">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="c3884-750">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="c3884-750">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="c3884-751">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="c3884-751">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="c3884-752">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="c3884-752">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="c3884-753">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="c3884-753">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="c3884-754">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="c3884-754">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="c3884-755">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="c3884-755">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="c3884-756">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="c3884-756">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="c3884-757">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="c3884-757">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="c3884-758">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="c3884-758">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="c3884-759">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="c3884-759">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="c3884-760">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="c3884-760">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="c3884-761">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="c3884-761">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="c3884-762">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="c3884-762">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="c3884-763">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="c3884-763">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="c3884-764">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="c3884-764">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="c3884-765">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="c3884-765">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="c3884-766">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="c3884-766">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="c3884-767">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="c3884-767">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="c3884-768">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-768">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="c3884-769">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="c3884-769">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="c3884-770">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-770">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-771">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-771">Interactive</span></span>

* <span data-ttu-id="c3884-772">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="c3884-772">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="c3884-773">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-773">Kubernetes</span></span>

* <span data-ttu-id="c3884-774">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="c3884-774">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-775">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-775">Network</span></span>

* <span data-ttu-id="c3884-776">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-776">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-777">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-777">Profile</span></span>

* <span data-ttu-id="c3884-778">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-778">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="c3884-779">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c3884-779">ServiceFabric</span></span>

* <span data-ttu-id="c3884-780">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="c3884-780">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="c3884-781">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="c3884-781">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-782">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-782">Storage</span></span>

* <span data-ttu-id="c3884-783">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="c3884-783">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="c3884-784">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-784">July 30, 2019</span></span>

<span data-ttu-id="c3884-785">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="c3884-785">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-786">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-786">ACR</span></span>

* <span data-ttu-id="c3884-787">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="c3884-787">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="c3884-788">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="c3884-788">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-789">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-789">Appservice</span></span>

* <span data-ttu-id="c3884-790">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="c3884-790">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="c3884-791">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="c3884-791">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="c3884-792">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="c3884-792">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="c3884-793">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-793">Network</span></span>

* <span data-ttu-id="c3884-794">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="c3884-794">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="c3884-795">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="c3884-795">Fixes #9604.</span></span> <span data-ttu-id="c3884-796">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c3884-796">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="c3884-797">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="c3884-797">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-798">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-798">RBAC</span></span>

* <span data-ttu-id="c3884-799">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="c3884-799">Added `user update` command</span></span>
* <span data-ttu-id="c3884-800">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c3884-800">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="c3884-801">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="c3884-801">Use replacement argument `--id`</span></span>
* <span data-ttu-id="c3884-802">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c3884-802">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-803">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-803">SQL</span></span>

* <span data-ttu-id="c3884-804">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="c3884-804">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-805">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-805">Storage</span></span>

* <span data-ttu-id="c3884-806">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="c3884-806">Added `storage remove` command</span></span>
* <span data-ttu-id="c3884-807">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="c3884-807">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-808">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-808">VM</span></span>

* <span data-ttu-id="c3884-809">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="c3884-809">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="c3884-810">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c3884-810">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="c3884-811">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-811">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="c3884-812">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="c3884-812">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="c3884-813">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-813">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="c3884-814">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-814">July 16, 2019</span></span>

<span data-ttu-id="c3884-815">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="c3884-815">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-816">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-816">Appservice</span></span>

* <span data-ttu-id="c3884-817">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="c3884-817">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="c3884-818">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-818">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="c3884-819">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="c3884-819">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="c3884-820">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-820">Core</span></span>

* <span data-ttu-id="c3884-821">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-821">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-822">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-822">Batch</span></span>

* <span data-ttu-id="c3884-823">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="c3884-823">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="c3884-824">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="c3884-824">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="c3884-825">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="c3884-825">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="c3884-826">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-826">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c3884-827">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c3884-827">Eventhubs</span></span>

* <span data-ttu-id="c3884-828">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="c3884-828">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-829">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-829">RDBMS</span></span>

* <span data-ttu-id="c3884-830">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="c3884-830">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="c3884-831">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="c3884-831">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="c3884-832">Relais</span><span class="sxs-lookup"><span data-stu-id="c3884-832">Relay</span></span>

* <span data-ttu-id="c3884-833">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="c3884-833">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="c3884-834">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="c3884-834">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="c3884-835">Servicebus</span><span class="sxs-lookup"><span data-stu-id="c3884-835">Servicebus</span></span>

* <span data-ttu-id="c3884-836">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="c3884-836">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-837">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-837">Storage</span></span>

* <span data-ttu-id="c3884-838">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-838">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="c3884-839">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="c3884-839">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="c3884-840">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-840">July 2, 2019</span></span>

<span data-ttu-id="c3884-841">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="c3884-841">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="c3884-842">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-842">Core</span></span>

* <span data-ttu-id="c3884-843">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="c3884-843">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="c3884-844">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="c3884-844">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="c3884-845">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="c3884-845">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-846">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-846">ACR</span></span>

* <span data-ttu-id="c3884-847">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="c3884-847">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-848">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-848">Appservice</span></span>

* <span data-ttu-id="c3884-849">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-849">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="c3884-850">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="c3884-850">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="c3884-851">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="c3884-851">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="c3884-852">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="c3884-852">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c3884-853">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-853">Cosmos DB</span></span>

* <span data-ttu-id="c3884-854">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="c3884-854">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="c3884-855">DLS</span><span class="sxs-lookup"><span data-stu-id="c3884-855">DLS</span></span>

* <span data-ttu-id="c3884-856">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="c3884-856">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="c3884-857">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c3884-857">Feedback</span></span>

* <span data-ttu-id="c3884-858">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="c3884-858">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-859">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-859">HDInsight</span></span>

* <span data-ttu-id="c3884-860">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="c3884-860">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="c3884-861">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="c3884-861">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="c3884-862">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="c3884-862">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="c3884-863">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="c3884-863">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="c3884-864">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="c3884-864">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="c3884-865">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-865">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="c3884-866">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="c3884-866">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="c3884-867">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="c3884-867">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="c3884-868">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="c3884-868">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="c3884-869">Services gérés</span><span class="sxs-lookup"><span data-stu-id="c3884-869">Managed Services</span></span>

* <span data-ttu-id="c3884-870">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-870">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-871">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-871">Profile</span></span>
* <span data-ttu-id="c3884-872">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="c3884-872">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-873">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-873">RBAC</span></span>

* <span data-ttu-id="c3884-874">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c3884-874">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="c3884-875">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="c3884-875">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="c3884-876">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="c3884-876">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="c3884-877">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="c3884-877">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-878">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-878">RDBMS</span></span>

* <span data-ttu-id="c3884-879">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="c3884-879">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-880">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-880">SQL</span></span>

* <span data-ttu-id="c3884-881">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-881">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-882">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-882">Storage</span></span>

* <span data-ttu-id="c3884-883">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c3884-883">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="c3884-884">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c3884-884">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="c3884-885">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-885">VM</span></span>

* <span data-ttu-id="c3884-886">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-886">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="c3884-887">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="c3884-887">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="c3884-888">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-888">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="c3884-889">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="c3884-889">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="c3884-890">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-890">June 18, 2019</span></span>

<span data-ttu-id="c3884-891">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="c3884-891">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="c3884-892">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-892">Core</span></span>

<span data-ttu-id="c3884-893">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="c3884-893">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="c3884-894">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="c3884-894">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="c3884-895">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="c3884-895">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="c3884-896">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="c3884-896">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="c3884-897">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="c3884-897">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="c3884-898">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="c3884-898">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="c3884-899">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="c3884-899">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-900">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-900">ACR</span></span>
* <span data-ttu-id="c3884-901">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="c3884-901">Added 'acr check-health' command</span></span>
* <span data-ttu-id="c3884-902">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="c3884-902">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-903">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-903">ACS</span></span>
* <span data-ttu-id="c3884-904">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-904">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-905">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-905">AMS</span></span>
* <span data-ttu-id="c3884-906">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="c3884-906">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-907">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-907">AppService</span></span>
* <span data-ttu-id="c3884-908">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="c3884-908">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="c3884-909">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-909">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="c3884-910">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="c3884-910">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="c3884-911">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-911">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="c3884-912">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="c3884-912">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="c3884-913">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="c3884-913">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-914">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-914">Batch</span></span>
* <span data-ttu-id="c3884-915">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="c3884-915">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-916">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-916">BatchAI</span></span>
* <span data-ttu-id="c3884-917">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="c3884-917">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-918">BotService</span><span class="sxs-lookup"><span data-stu-id="c3884-918">BotService</span></span>
* <span data-ttu-id="c3884-919">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="c3884-919">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-920">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-920">CosmosDB</span></span>
* <span data-ttu-id="c3884-921">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="c3884-921">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="c3884-922">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="c3884-922">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="c3884-923">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="c3884-923">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="c3884-924">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="c3884-924">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c3884-925">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c3884-925">EventGrid</span></span>
* <span data-ttu-id="c3884-926">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="c3884-926">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="c3884-927">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="c3884-927">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="c3884-928">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="c3884-928">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="c3884-929">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="c3884-929">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="c3884-930">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-930">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-931">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-931">HDInsight</span></span>
* <span data-ttu-id="c3884-932">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c3884-932">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-933">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-933">IoT</span></span>
* <span data-ttu-id="c3884-934">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="c3884-934">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="c3884-935">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="c3884-935">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="c3884-936">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-936">Network</span></span>
* <span data-ttu-id="c3884-937">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="c3884-937">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="c3884-938">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="c3884-938">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="c3884-939">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="c3884-939">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="c3884-940">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="c3884-940">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-941">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-941">Resource</span></span>
* <span data-ttu-id="c3884-942">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="c3884-942">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="c3884-943">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="c3884-943">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="c3884-944">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c3884-944">ServiceBus</span></span>
* <span data-ttu-id="c3884-945">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="c3884-945">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-946">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-946">SQL</span></span>
* <span data-ttu-id="c3884-947">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c3884-947">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="c3884-948">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="c3884-948">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="c3884-949">SQLVm</span><span class="sxs-lookup"><span data-stu-id="c3884-949">SQLVm</span></span>
* <span data-ttu-id="c3884-950">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="c3884-950">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="c3884-951">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-951">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-952">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-952">Storage</span></span>
* <span data-ttu-id="c3884-953">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c3884-953">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="c3884-954">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-954">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-955">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-955">VM</span></span>
* <span data-ttu-id="c3884-956">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-956">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="c3884-957">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-957">June 4, 2019</span></span>

<span data-ttu-id="c3884-958">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="c3884-958">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="c3884-959">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-959">Core</span></span>
* <span data-ttu-id="c3884-960">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="c3884-960">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-961">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-961">ACR</span></span>
* <span data-ttu-id="c3884-962">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="c3884-962">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-963">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-963">ACS</span></span>
* <span data-ttu-id="c3884-964">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-964">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="c3884-965">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="c3884-965">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-966">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-966">Batch</span></span>
* <span data-ttu-id="c3884-967">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="c3884-967">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-968">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-968">IoT</span></span>
* <span data-ttu-id="c3884-969">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c3884-969">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="c3884-970">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-970">Network</span></span>
* <span data-ttu-id="c3884-971">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="c3884-971">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="c3884-972">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-972">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="c3884-973">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-973">Resource</span></span>
* <span data-ttu-id="c3884-974">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="c3884-974">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="c3884-975">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-975">Role</span></span>
* <span data-ttu-id="c3884-976">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-976">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-977">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-977">Compute</span></span>
* <span data-ttu-id="c3884-978">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="c3884-978">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="c3884-979">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-979">May 21, 2019</span></span>

<span data-ttu-id="c3884-980">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="c3884-980">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="c3884-981">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-981">Core</span></span>
* <span data-ttu-id="c3884-982">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="c3884-982">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="c3884-983">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="c3884-983">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="c3884-984">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="c3884-984">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-985">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-985">ACR</span></span>
* <span data-ttu-id="c3884-986">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="c3884-986">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-987">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-987">ACS</span></span>
* <span data-ttu-id="c3884-988">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="c3884-988">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-989">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-989">AppService</span></span>
* <span data-ttu-id="c3884-990">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="c3884-990">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="c3884-991">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="c3884-991">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="c3884-992">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="c3884-992">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="c3884-993">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="c3884-993">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="c3884-994">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-994">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="c3884-995">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="c3884-995">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="c3884-996">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-996">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-997">BotService</span><span class="sxs-lookup"><span data-stu-id="c3884-997">BotService</span></span>
* <span data-ttu-id="c3884-998">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-998">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="c3884-999">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-999">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-1000">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-1000">Consumption</span></span>
* <span data-ttu-id="c3884-1001">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-1001">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-1002">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1002">IoT</span></span>
* <span data-ttu-id="c3884-1003">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="c3884-1003">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1004">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1004">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="c3884-1006">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="c3884-1006">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="c3884-1007">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="c3884-1007">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1008">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-1008">RDBMS</span></span>
* <span data-ttu-id="c3884-1009">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="c3884-1009">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-1010">RBAC</span><span class="sxs-lookup"><span data-stu-id="c3884-1010">RBAC</span></span>
* <span data-ttu-id="c3884-1011">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="c3884-1011">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1012">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1012">Storage</span></span>
* <span data-ttu-id="c3884-1013">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1013">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="c3884-1014">Calcul</span><span class="sxs-lookup"><span data-stu-id="c3884-1014">Compute</span></span>
* <span data-ttu-id="c3884-1015">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1015">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="c3884-1016">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="c3884-1016">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="c3884-1017">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="c3884-1017">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="c3884-1018">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1018">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="c3884-1019">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1019">May 6, 2019</span></span>

<span data-ttu-id="c3884-1020">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="c3884-1020">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1021">ACS</span></span>
* <span data-ttu-id="c3884-1022">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="c3884-1022">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="c3884-1023">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="c3884-1023">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="c3884-1024">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1024">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="c3884-1025">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-1025">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1026">Appservice</span></span>
* <span data-ttu-id="c3884-1027">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="c3884-1027">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="c3884-1028">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="c3884-1028">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="c3884-1029">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-1029">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="c3884-1030">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="c3884-1030">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="c3884-1031">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-1031">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="c3884-1032">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="c3884-1032">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="c3884-1033">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="c3884-1033">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="c3884-1034">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="c3884-1034">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="c3884-1035">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-1035">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="c3884-1036">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="c3884-1036">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-1037">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-1037">Batch</span></span>
* <span data-ttu-id="c3884-1038">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="c3884-1038">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-1039">Botservice</span><span class="sxs-lookup"><span data-stu-id="c3884-1039">Botservice</span></span>
* <span data-ttu-id="c3884-1040">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="c3884-1040">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="c3884-1041">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="c3884-1041">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="c3884-1042">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="c3884-1042">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="c3884-1043">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1043">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="c3884-1044">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1044">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="c3884-1045">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-1045">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="c3884-1046">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1046">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="c3884-1047">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="c3884-1047">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="c3884-1048">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="c3884-1048">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="c3884-1049">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="c3884-1049">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="c3884-1050">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="c3884-1050">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="c3884-1051">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="c3884-1051">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="c3884-1052">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="c3884-1052">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="c3884-1053">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="c3884-1053">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="c3884-1054">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1054">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="c3884-1055">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="c3884-1055">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="c3884-1056">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="c3884-1056">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="c3884-1057">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="c3884-1057">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="c3884-1058">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c3884-1058">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="c3884-1059">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="c3884-1059">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="c3884-1060">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="c3884-1060">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="c3884-1061">Configurer</span><span class="sxs-lookup"><span data-stu-id="c3884-1061">Configure</span></span>
* <span data-ttu-id="c3884-1062">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="c3884-1062">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c3884-1063">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c3884-1063">Eventhubs</span></span>
* <span data-ttu-id="c3884-1064">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-1064">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="c3884-1065">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1065">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1066">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1066">Network</span></span>
* <span data-ttu-id="c3884-1067">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1067">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="c3884-1068">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c3884-1068">Policy Insights</span></span>
* <span data-ttu-id="c3884-1069">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1069">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1070">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1070">Role</span></span>
* <span data-ttu-id="c3884-1071">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1071">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="c3884-1072">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-1072">Service Bus</span></span>
* <span data-ttu-id="c3884-1073">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-1073">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="c3884-1074">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1074">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="c3884-1075">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="c3884-1075">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1076">SQL</span></span>
* <span data-ttu-id="c3884-1077">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1077">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1078">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1078">VM</span></span>
* <span data-ttu-id="c3884-1079">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="c3884-1079">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="c3884-1080">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="c3884-1080">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="c3884-1081">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1081">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="c3884-1082">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="c3884-1082">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="c3884-1083">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="c3884-1083">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="c3884-1084">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1084">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="c3884-1085">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1085">April 23, 2019</span></span>

<span data-ttu-id="c3884-1086">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="c3884-1086">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1087">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1087">ACS</span></span>
* <span data-ttu-id="c3884-1088">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="c3884-1088">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="c3884-1089">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="c3884-1089">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-1090">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-1090">AMS</span></span>
* <span data-ttu-id="c3884-1091">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="c3884-1091">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1092">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1092">AppService</span></span>
* <span data-ttu-id="c3884-1093">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="c3884-1093">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="c3884-1094">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="c3884-1094">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="c3884-1095">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="c3884-1095">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="c3884-1096">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="c3884-1096">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="c3884-1097">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="c3884-1097">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="c3884-1098">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-1098">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="c3884-1099">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="c3884-1099">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="c3884-1100">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="c3884-1100">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="c3884-1101">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="c3884-1101">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="c3884-1102">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-1102">Deployment Manager</span></span>
* <span data-ttu-id="c3884-1103">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="c3884-1103">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="c3884-1104">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-1104">Lab</span></span>
* <span data-ttu-id="c3884-1105">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="c3884-1105">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1106">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1106">Network</span></span>
* <span data-ttu-id="c3884-1107">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="c3884-1107">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1108">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1108">Resource</span></span>
* <span data-ttu-id="c3884-1109">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="c3884-1109">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="c3884-1110">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="c3884-1110">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="c3884-1111">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1111">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="c3884-1112">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-1112">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1113">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1113">SQL</span></span>
* <span data-ttu-id="c3884-1114">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="c3884-1114">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="c3884-1115">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1115">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="c3884-1116">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1116">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="c3884-1117">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1117">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1118">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1118">Storage</span></span>
* <span data-ttu-id="c3884-1119">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="c3884-1119">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1120">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1120">VM</span></span>
* <span data-ttu-id="c3884-1121">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="c3884-1121">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="c3884-1122">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="c3884-1122">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="c3884-1123">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="c3884-1123">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="c3884-1124">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1124">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1125">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1125">Core</span></span>
* <span data-ttu-id="c3884-1126">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-1126">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1127">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1127">ACR</span></span>
* <span data-ttu-id="c3884-1128">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="c3884-1128">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-1129">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-1129">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="c3884-1132">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1132">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="c3884-1133">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1133">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1134">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1134">AppService</span></span>
* <span data-ttu-id="c3884-1135">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-1135">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="c3884-1136">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1136">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="c3884-1137">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1137">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="c3884-1138">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="c3884-1138">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="c3884-1139">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-1139">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="c3884-1140">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="c3884-1140">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="c3884-1141">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="c3884-1141">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-1142">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-1142">CDN</span></span>
* <span data-ttu-id="c3884-1143">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="c3884-1143">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="c3884-1144">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c3884-1144">Feedback</span></span>
* <span data-ttu-id="c3884-1145">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="c3884-1145">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="c3884-1146">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="c3884-1146">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="c3884-1147">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="c3884-1147">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1148">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1148">Monitor</span></span>
* <span data-ttu-id="c3884-1149">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1149">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="c3884-1150">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1150">Network</span></span>
* <span data-ttu-id="c3884-1151">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="c3884-1151">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="c3884-1152">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-1152">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="c3884-1153">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="c3884-1153">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="c3884-1154">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1154">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="c3884-1155">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="c3884-1155">PrivateDNS</span></span>
* <span data-ttu-id="c3884-1156">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c3884-1156">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1157">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1157">Resource</span></span>
* <span data-ttu-id="c3884-1158">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-1158">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1159">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1159">Role</span></span>
* <span data-ttu-id="c3884-1160">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-1160">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="c3884-1161">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1161">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1162">SQL</span></span>
* <span data-ttu-id="c3884-1163">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="c3884-1163">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1164">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1164">Storage</span></span>
* <span data-ttu-id="c3884-1165">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-1165">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="c3884-1166">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="c3884-1166">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="c3884-1167">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="c3884-1167">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="c3884-1168">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="c3884-1168">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="c3884-1169">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1169">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="c3884-1170">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1170">Core</span></span>
* <span data-ttu-id="c3884-1171">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="c3884-1171">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="c3884-1172">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="c3884-1172">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="c3884-1173">Cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-1173">Cloud</span></span>
* <span data-ttu-id="c3884-1174">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="c3884-1174">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1175">ACR</span></span>
* <span data-ttu-id="c3884-1176">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c3884-1176">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="c3884-1177">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1177">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="c3884-1178">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="c3884-1178">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="c3884-1179">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="c3884-1179">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1180">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1180">AppService</span></span>
* <span data-ttu-id="c3884-1181">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="c3884-1181">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="c3884-1182">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="c3884-1182">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="c3884-1183">Service BOT</span><span class="sxs-lookup"><span data-stu-id="c3884-1183">BOT Service</span></span>
* <span data-ttu-id="c3884-1184">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="c3884-1184">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="c3884-1185">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-1185">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="c3884-1186">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="c3884-1186">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="c3884-1187">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c3884-1187">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-1188">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-1188">CDN</span></span>
* <span data-ttu-id="c3884-1189">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1189">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="c3884-1190">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1190">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="c3884-1191">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="c3884-1191">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c3884-1192">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c3884-1192">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-1193">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c3884-1193">Cosmosdb</span></span>
* <span data-ttu-id="c3884-1194">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="c3884-1194">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="c3884-1195">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-1195">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-1196">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-1196">Interactive</span></span>
* <span data-ttu-id="c3884-1197">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="c3884-1197">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1198">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1198">Monitor</span></span>
* <span data-ttu-id="c3884-1199">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1199">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1200">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1200">Network</span></span>
* <span data-ttu-id="c3884-1201">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="c3884-1201">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-1202">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-1202">Profile</span></span>
* <span data-ttu-id="c3884-1203">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="c3884-1203">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="c3884-1204">Postgres</span><span class="sxs-lookup"><span data-stu-id="c3884-1204">Postgres</span></span> 
* <span data-ttu-id="c3884-1205">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="c3884-1205">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="c3884-1206">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="c3884-1206">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1207">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1207">Resource</span></span>
* <span data-ttu-id="c3884-1208">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1208">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="c3884-1209">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="c3884-1209">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="c3884-1210">Graph</span><span class="sxs-lookup"><span data-stu-id="c3884-1210">Graph</span></span>
* <span data-ttu-id="c3884-1211">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="c3884-1211">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="c3884-1212">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="c3884-1212">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="c3884-1213">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="c3884-1213">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="c3884-1214">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1214">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="c3884-1215">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-1215">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1216">storage</span><span class="sxs-lookup"><span data-stu-id="c3884-1216">storage</span></span>
* <span data-ttu-id="c3884-1217">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="c3884-1217">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="c3884-1218">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="c3884-1218">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="c3884-1219">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c3884-1219">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="c3884-1220">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="c3884-1220">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1221">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1221">VM</span></span>
* <span data-ttu-id="c3884-1222">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1222">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="c3884-1223">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1223">March 12, 2019</span></span>

<span data-ttu-id="c3884-1224">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="c3884-1224">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1225">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1225">Core</span></span>

* <span data-ttu-id="c3884-1226">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="c3884-1226">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1227">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1227">ACR</span></span>

* <span data-ttu-id="c3884-1228">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c3884-1228">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1229">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1229">ACS</span></span>

* <span data-ttu-id="c3884-1230">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="c3884-1230">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="c3884-1231">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1231">AppService</span></span>

* <span data-ttu-id="c3884-1232">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="c3884-1232">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="c3884-1233">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1233">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="c3884-1234">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-1234">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="c3884-1235">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="c3884-1235">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-1236">Botservice</span><span class="sxs-lookup"><span data-stu-id="c3884-1236">Botservice</span></span>

* <span data-ttu-id="c3884-1237">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c3884-1237">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c3884-1238">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c3884-1238">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c3884-1239">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1239">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="c3884-1240">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="c3884-1240">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1241">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1241">Container</span></span>

* <span data-ttu-id="c3884-1242">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1242">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="c3884-1243">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c3884-1243">EventHub</span></span>

* <span data-ttu-id="c3884-1244">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="c3884-1244">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="c3884-1245">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c3884-1245">Find</span></span>

* <span data-ttu-id="c3884-1246">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c3884-1246">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-1247">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-1247">HDInsight</span></span>

* <span data-ttu-id="c3884-1248">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="c3884-1248">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1249">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1249">Network</span></span>

* <span data-ttu-id="c3884-1250">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="c3884-1250">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1251">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c3884-1251">Rdbms</span></span>

* <span data-ttu-id="c3884-1252">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="c3884-1252">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1253">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1253">Role</span></span>

* <span data-ttu-id="c3884-1254">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="c3884-1254">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="c3884-1255">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="c3884-1255">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c3884-1256">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c3884-1256">Service Fabric</span></span>

* <span data-ttu-id="c3884-1257">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="c3884-1257">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="c3884-1258">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1258">February 26, 2019</span></span>

<span data-ttu-id="c3884-1259">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="c3884-1259">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1260">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1260">Core</span></span>

* <span data-ttu-id="c3884-1261">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="c3884-1261">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1262">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1262">ACR</span></span>

* <span data-ttu-id="c3884-1263">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1263">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="c3884-1264">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="c3884-1264">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1265">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1265">ACS</span></span>

* <span data-ttu-id="c3884-1266">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="c3884-1266">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1267">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1267">AppService</span></span>

* <span data-ttu-id="c3884-1268">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="c3884-1268">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-1269">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-1269">Batch</span></span>
* <span data-ttu-id="c3884-1270">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="c3884-1270">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="c3884-1271">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="c3884-1271">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="c3884-1272">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="c3884-1272">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="c3884-1273">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="c3884-1273">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="c3884-1274">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="c3884-1274">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="c3884-1275">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="c3884-1275">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-1276">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-1276">CosmosDB</span></span>

* <span data-ttu-id="c3884-1277">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-1277">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="c3884-1278">Kusto</span><span class="sxs-lookup"><span data-stu-id="c3884-1278">Kusto</span></span>

* <span data-ttu-id="c3884-1279">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="c3884-1279">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1280">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1280">Network</span></span>

* <span data-ttu-id="c3884-1281">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1281">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="c3884-1282">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="c3884-1282">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="c3884-1283">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="c3884-1283">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="c3884-1284">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1284">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="c3884-1285">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1285">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="c3884-1286">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1286">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="c3884-1287">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="c3884-1287">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1288">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1288">Resource</span></span>

* <span data-ttu-id="c3884-1289">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-1289">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="c3884-1290">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1290">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="c3884-1291">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1291">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="c3884-1292">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1292">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="c3884-1293">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1293">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1294">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1294">Role</span></span>

* <span data-ttu-id="c3884-1295">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1295">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1296">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1296">VM</span></span>

* <span data-ttu-id="c3884-1297">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="c3884-1297">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="c3884-1298">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1298">February 12, 2019</span></span>

<span data-ttu-id="c3884-1299">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="c3884-1299">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1300">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1300">Core</span></span>

* <span data-ttu-id="c3884-1301">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-1301">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="c3884-1302">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="c3884-1302">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1303">ACR</span></span>
* <span data-ttu-id="c3884-1304">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="c3884-1304">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="c3884-1305">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-1305">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1306">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1306">ACS</span></span>
* <span data-ttu-id="c3884-1307">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1307">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="c3884-1308">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="c3884-1308">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="c3884-1309">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c3884-1309">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-1310">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-1310">AMS</span></span>
* <span data-ttu-id="c3884-1311">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1311">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="c3884-1312">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1312">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1313">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1313">Appservice</span></span>
* <span data-ttu-id="c3884-1314">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1314">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="c3884-1315">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="c3884-1315">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="c3884-1316">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1316">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="c3884-1317">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="c3884-1317">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="c3884-1318">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="c3884-1318">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-1319">Botservice</span><span class="sxs-lookup"><span data-stu-id="c3884-1319">Botservice</span></span>
* <span data-ttu-id="c3884-1320">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="c3884-1320">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="c3884-1321">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="c3884-1321">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="c3884-1322">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1322">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="c3884-1323">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="c3884-1323">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="c3884-1324">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="c3884-1324">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="c3884-1325">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="c3884-1325">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="c3884-1326">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="c3884-1326">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="c3884-1327">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="c3884-1327">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="c3884-1328">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="c3884-1328">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="c3884-1329">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="c3884-1329">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-1330">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-1330">Key Vault</span></span>
* <span data-ttu-id="c3884-1331">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="c3884-1331">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1332">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1332">Monitor</span></span>
* <span data-ttu-id="c3884-1333">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="c3884-1333">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1334">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1334">Network</span></span>
* <span data-ttu-id="c3884-1335">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="c3884-1335">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="c3884-1336">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c3884-1336">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="c3884-1337">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-1337">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="c3884-1338">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1338">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c3884-1339">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c3884-1339">Policy Insights</span></span>
* <span data-ttu-id="c3884-1340">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-1340">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1341">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-1341">RDBMS</span></span>
* <span data-ttu-id="c3884-1342">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-1342">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="c3884-1343">Redis</span><span class="sxs-lookup"><span data-stu-id="c3884-1343">Redis</span></span>
* <span data-ttu-id="c3884-1344">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c3884-1344">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="c3884-1345">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c3884-1345">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="c3884-1346">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="c3884-1346">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="c3884-1347">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="c3884-1347">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="c3884-1348">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="c3884-1348">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="c3884-1349">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="c3884-1349">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="c3884-1350">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="c3884-1350">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1351">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1351">Role</span></span>
* <span data-ttu-id="c3884-1352">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="c3884-1352">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="c3884-1353">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1353">SQL VM</span></span>
* <span data-ttu-id="c3884-1354">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="c3884-1354">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1355">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1355">VM</span></span>
* <span data-ttu-id="c3884-1356">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="c3884-1356">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="c3884-1357">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1357">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="c3884-1358">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="c3884-1358">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="c3884-1359">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="c3884-1359">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="c3884-1360">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1360">January 31, 2019</span></span>

<span data-ttu-id="c3884-1361">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="c3884-1361">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1362">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1362">Core</span></span>

* <span data-ttu-id="c3884-1363">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="c3884-1363">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="c3884-1364">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1364">January 28, 2019</span></span>

<span data-ttu-id="c3884-1365">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="c3884-1365">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1366">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1366">ACR</span></span>
* <span data-ttu-id="c3884-1367">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="c3884-1367">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1368">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1368">ACS</span></span>
* <span data-ttu-id="c3884-1369">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c3884-1369">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c3884-1370">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="c3884-1370">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="c3884-1371">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="c3884-1371">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-1372">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-1372">AMS</span></span>
* <span data-ttu-id="c3884-1373">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="c3884-1373">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="c3884-1374">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="c3884-1374">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1375">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1375">Appservice</span></span>
* <span data-ttu-id="c3884-1376">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1376">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="c3884-1377">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="c3884-1377">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="c3884-1378">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="c3884-1378">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1379">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1379">Container</span></span>
* <span data-ttu-id="c3884-1380">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="c3884-1380">Added `container start` command</span></span>
* <span data-ttu-id="c3884-1381">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1381">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c3884-1382">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c3884-1382">EventGrid</span></span>
* <span data-ttu-id="c3884-1383">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1383">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="c3884-1384">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="c3884-1384">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="c3884-1385">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="c3884-1385">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="c3884-1386">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="c3884-1386">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="c3884-1387">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="c3884-1387">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-1388">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-1388">HDInsight</span></span>
* <span data-ttu-id="c3884-1389">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1389">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="c3884-1390">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c3884-1390">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="c3884-1391">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1391">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="c3884-1392">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1392">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="c3884-1393">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="c3884-1393">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="c3884-1394">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1394">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-1395">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1395">IoT</span></span>
* <span data-ttu-id="c3884-1396">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="c3884-1396">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="c3884-1397">Kusto</span><span class="sxs-lookup"><span data-stu-id="c3884-1397">Kusto</span></span>
* <span data-ttu-id="c3884-1398">Préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-1398">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1399">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1399">Monitor</span></span>
* <span data-ttu-id="c3884-1400">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-1400">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-1401">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-1401">Profile</span></span>
* <span data-ttu-id="c3884-1402">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="c3884-1402">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1403">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1403">Network</span></span>
* <span data-ttu-id="c3884-1404">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="c3884-1404">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="c3884-1405">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="c3884-1405">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1406">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1406">Resource</span></span>
* <span data-ttu-id="c3884-1407">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1407">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="c3884-1408">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1408">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="c3884-1409">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1409">SQL Virtual Machine</span></span>
* <span data-ttu-id="c3884-1410">Préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-1410">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1411">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1411">Storage</span></span>
* <span data-ttu-id="c3884-1412">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="c3884-1412">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="c3884-1413">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="c3884-1413">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1414">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1414">VM</span></span>
* <span data-ttu-id="c3884-1415">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="c3884-1415">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="c3884-1416">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c3884-1416">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="c3884-1417">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c3884-1417">January 15, 2019</span></span>

<span data-ttu-id="c3884-1418">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="c3884-1418">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1419">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1419">ACR</span></span>
* <span data-ttu-id="c3884-1420">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c3884-1420">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="c3884-1421">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-1421">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="c3884-1422">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="c3884-1422">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="c3884-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1423">ACS</span></span>
* <span data-ttu-id="c3884-1424">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="c3884-1424">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1425">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1425">Appservice</span></span>
* <span data-ttu-id="c3884-1426">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="c3884-1426">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="c3884-1427">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-1427">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="c3884-1428">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-1428">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="c3884-1429">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="c3884-1429">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-1430">Botservice</span><span class="sxs-lookup"><span data-stu-id="c3884-1430">Botservice</span></span>
* <span data-ttu-id="c3884-1431">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1431">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="c3884-1432">Configurer</span><span class="sxs-lookup"><span data-stu-id="c3884-1432">Configure</span></span>
* <span data-ttu-id="c3884-1433">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="c3884-1433">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-1434">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-1434">CosmosDB</span></span>
* <span data-ttu-id="c3884-1435">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="c3884-1435">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-1436">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-1436">HDInsight</span></span>
* <span data-ttu-id="c3884-1437">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="c3884-1437">Added commands for managing applications</span></span>
* <span data-ttu-id="c3884-1438">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="c3884-1438">Added commands for managing script actions</span></span>
* <span data-ttu-id="c3884-1439">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="c3884-1439">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="c3884-1440">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="c3884-1440">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="c3884-1441">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1441">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1442">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1442">Network</span></span>
* <span data-ttu-id="c3884-1443">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1443">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="c3884-1444">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="c3884-1444">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="c3884-1445">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1445">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="c3884-1446">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-1446">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1447">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1447">Role</span></span>
* <span data-ttu-id="c3884-1448">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1448">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="c3884-1449">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="c3884-1449">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="c3884-1450">Sécurité</span><span class="sxs-lookup"><span data-stu-id="c3884-1450">Security</span></span>
* <span data-ttu-id="c3884-1451">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-1451">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1452">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1452">Storage</span></span>
* <span data-ttu-id="c3884-1453">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="c3884-1453">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="c3884-1454">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="c3884-1454">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="c3884-1455">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1455">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="c3884-1456">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1456">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="c3884-1457">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1457">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1458">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1458">VM</span></span>
* <span data-ttu-id="c3884-1459">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="c3884-1459">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="c3884-1460">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1460">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c3884-1461">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="c3884-1461">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="c3884-1462">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="c3884-1462">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="c3884-1463">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1463">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="c3884-1464">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-1464">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="c3884-1465">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1465">December 20, 2018</span></span>

<span data-ttu-id="c3884-1466">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="c3884-1466">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="c3884-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1467">Appservice</span></span>
* <span data-ttu-id="c3884-1468">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c3884-1468">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="c3884-1469">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="c3884-1469">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="c3884-1470">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-1470">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c3884-1471">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c3884-1471">IoTCentral</span></span>
* <span data-ttu-id="c3884-1472">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-1472">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1473">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1473">Role</span></span>
* <span data-ttu-id="c3884-1474">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="c3884-1474">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1475">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1475">SQL</span></span>
* <span data-ttu-id="c3884-1476">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="c3884-1476">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1477">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1477">VM</span></span>
* <span data-ttu-id="c3884-1478">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1478">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="c3884-1479">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1479">December 18, 2018</span></span>

<span data-ttu-id="c3884-1480">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="c3884-1480">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="c3884-1481">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1481">ACR</span></span>
* <span data-ttu-id="c3884-1482">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="c3884-1482">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="c3884-1483">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="c3884-1483">Condensed the table layout for task list</span></span>
* <span data-ttu-id="c3884-1484">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="c3884-1484">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1485">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1485">ACS</span></span>
* <span data-ttu-id="c3884-1486">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c3884-1486">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c3884-1487">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1487">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="c3884-1488">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1488">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="c3884-1489">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="c3884-1489">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="c3884-1490">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-1490">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="c3884-1491">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="c3884-1491">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1492">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1492">Appservice</span></span>
* <span data-ttu-id="c3884-1493">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="c3884-1493">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="c3884-1494">Botservice</span><span class="sxs-lookup"><span data-stu-id="c3884-1494">Botservice</span></span>
* <span data-ttu-id="c3884-1495">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="c3884-1495">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="c3884-1496">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="c3884-1496">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="c3884-1497">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="c3884-1497">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="c3884-1498">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="c3884-1498">Reduced Kudu network calls</span></span>
* <span data-ttu-id="c3884-1499">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="c3884-1499">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-1500">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-1500">Consumption</span></span>
* <span data-ttu-id="c3884-1501">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="c3884-1501">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-1502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-1502">CosmosDB</span></span>
* <span data-ttu-id="c3884-1503">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="c3884-1503">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="c3884-1504">Cartes</span><span class="sxs-lookup"><span data-stu-id="c3884-1504">Maps</span></span>
* <span data-ttu-id="c3884-1505">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1505">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1506">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1506">Network</span></span>
* <span data-ttu-id="c3884-1507">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="c3884-1507">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="c3884-1508">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-1508">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1509">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1509">Resource</span></span>
* <span data-ttu-id="c3884-1510">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1510">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="c3884-1511">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1511">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1512">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1512">Storage</span></span>
*  <span data-ttu-id="c3884-1513">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1513">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1514">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1514">VM</span></span>
* <span data-ttu-id="c3884-1515">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="c3884-1515">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="c3884-1516">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1516">December 4, 2018</span></span>

<span data-ttu-id="c3884-1517">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="c3884-1517">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="c3884-1518">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1518">Core</span></span>
* <span data-ttu-id="c3884-1519">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="c3884-1519">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="c3884-1520">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c3884-1520">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1521">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1521">Appservice</span></span>
* <span data-ttu-id="c3884-1522">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="c3884-1522">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="c3884-1523">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c3884-1523">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1524">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1524">Network</span></span>
* <span data-ttu-id="c3884-1525">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="c3884-1525">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1526">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1526">Role</span></span>
* <span data-ttu-id="c3884-1527">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="c3884-1527">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="c3884-1528">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1528">VM</span></span>
* <span data-ttu-id="c3884-1529">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="c3884-1529">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="c3884-1530">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="c3884-1530">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="c3884-1531">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="c3884-1531">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="c3884-1532">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="c3884-1532">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="c3884-1533">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1533">November 20, 2018</span></span>

<span data-ttu-id="c3884-1534">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="c3884-1534">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="c3884-1535">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1535">Core</span></span>
* <span data-ttu-id="c3884-1536">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="c3884-1536">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1537">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1537">ACR</span></span>
* <span data-ttu-id="c3884-1538">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="c3884-1538">Added context token to task step</span></span>
* <span data-ttu-id="c3884-1539">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="c3884-1539">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="c3884-1540">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c3884-1540">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1541">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1541">Appservice</span></span>
* <span data-ttu-id="c3884-1542">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="c3884-1542">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="c3884-1543">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1543">Updated the default `node_version`.</span></span> <span data-ttu-id="c3884-1544">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="c3884-1544">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="c3884-1545">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-1545">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="c3884-1546">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="c3884-1546">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c3884-1547">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c3884-1547">IotCentral</span></span>
* <span data-ttu-id="c3884-1548">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="c3884-1548">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-1549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-1549">KeyVault</span></span>
* <span data-ttu-id="c3884-1550">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="c3884-1550">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1551">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1551">Network</span></span>
* <span data-ttu-id="c3884-1552">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="c3884-1552">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="c3884-1553">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="c3884-1553">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="c3884-1554">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1554">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="c3884-1555">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="c3884-1555">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1556">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c3884-1556">Rdbms</span></span>
* <span data-ttu-id="c3884-1557">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="c3884-1557">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="c3884-1558">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="c3884-1558">Rbac</span></span>
* <span data-ttu-id="c3884-1559">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1559">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="c3884-1560">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1560">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="c3884-1561">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1561">Storage</span></span>
* <span data-ttu-id="c3884-1562">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1562">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="c3884-1563">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1563">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="c3884-1564">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="c3884-1564">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="c3884-1565">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="c3884-1565">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1566">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1566">VM</span></span>
* <span data-ttu-id="c3884-1567">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="c3884-1567">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="c3884-1568">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="c3884-1568">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="c3884-1569">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="c3884-1569">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="c3884-1570">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="c3884-1570">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="c3884-1571">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1571">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="c3884-1572">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1572">Added `snapshot wait` command</span></span>
* <span data-ttu-id="c3884-1573">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-1573">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="c3884-1574">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1574">November 6, 2018</span></span>

<span data-ttu-id="c3884-1575">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="c3884-1575">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1576">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1576">Core</span></span>
* <span data-ttu-id="c3884-1577">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="c3884-1577">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1578">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1578">ACR</span></span>
* <span data-ttu-id="c3884-1579">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="c3884-1579">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="c3884-1580">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="c3884-1580">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1581">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1581">ACS</span></span>
* <span data-ttu-id="c3884-1582">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1582">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="c3884-1583">Advisor</span><span class="sxs-lookup"><span data-stu-id="c3884-1583">Advisor</span></span>
* <span data-ttu-id="c3884-1584">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c3884-1584">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-1585">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-1585">AMS</span></span>
* <span data-ttu-id="c3884-1586">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="c3884-1586">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="c3884-1587">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="c3884-1587">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="c3884-1588">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1588">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="c3884-1589">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="c3884-1589">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="c3884-1590">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="c3884-1590">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="c3884-1591">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="c3884-1591">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="c3884-1592">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="c3884-1592">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="c3884-1593">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="c3884-1593">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="c3884-1594">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c3884-1594">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="c3884-1595">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c3884-1595">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="c3884-1596">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-1596">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="c3884-1597">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1597">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="c3884-1598">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="c3884-1598">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="c3884-1599">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="c3884-1599">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="c3884-1600">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1600">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="c3884-1601">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="c3884-1601">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="c3884-1602">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="c3884-1602">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1603">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1603">AppService</span></span>
* <span data-ttu-id="c3884-1604">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="c3884-1604">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="c3884-1605">Configurer</span><span class="sxs-lookup"><span data-stu-id="c3884-1605">Configure</span></span>
* <span data-ttu-id="c3884-1606">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="c3884-1606">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1607">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1607">Container</span></span>
* <span data-ttu-id="c3884-1608">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="c3884-1608">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="c3884-1609">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c3884-1609">EventHub</span></span>
* <span data-ttu-id="c3884-1610">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1610">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-1611">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-1611">Interactive</span></span>
* <span data-ttu-id="c3884-1612">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="c3884-1612">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1613">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1613">Monitor</span></span>
* <span data-ttu-id="c3884-1614">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1614">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1615">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1615">Network</span></span>
* <span data-ttu-id="c3884-1616">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="c3884-1616">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="c3884-1617">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1617">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="c3884-1618">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1618">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="c3884-1619">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-1619">Profile</span></span>
* <span data-ttu-id="c3884-1620">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="c3884-1620">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1621">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-1621">RDBMS</span></span>
* <span data-ttu-id="c3884-1622">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="c3884-1622">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1623">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1623">Resource</span></span>
* <span data-ttu-id="c3884-1624">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="c3884-1624">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1625">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1625">Role</span></span>
* <span data-ttu-id="c3884-1626">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="c3884-1626">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="c3884-1627">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="c3884-1627">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="c3884-1628">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="c3884-1628">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1629">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1629">Storage</span></span>
* <span data-ttu-id="c3884-1630">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="c3884-1630">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1631">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1631">VM</span></span>
* <span data-ttu-id="c3884-1632">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="c3884-1632">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="c3884-1633">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="c3884-1633">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="c3884-1634">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="c3884-1634">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="c3884-1635">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="c3884-1635">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="c3884-1636">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="c3884-1636">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="c3884-1637">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="c3884-1637">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="c3884-1638">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1638">October 23, 2018</span></span>

<span data-ttu-id="c3884-1639">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="c3884-1639">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1640">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1640">Core</span></span>
* <span data-ttu-id="c3884-1641">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="c3884-1641">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="c3884-1642">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="c3884-1642">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1643">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1643">ACR</span></span>
* <span data-ttu-id="c3884-1644">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="c3884-1644">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-1645">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-1645">CDN</span></span>
* <span data-ttu-id="c3884-1646">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="c3884-1646">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c3884-1647">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c3884-1647">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1648">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1648">Container</span></span>
* <span data-ttu-id="c3884-1649">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="c3884-1649">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="c3884-1650">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-1650">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="c3884-1651">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="c3884-1651">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="c3884-1652">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-1652">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="c3884-1653">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c3884-1653">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="c3884-1654">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="c3884-1654">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="c3884-1655">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="c3884-1655">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-1656">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-1656">CosmosDB</span></span>
* <span data-ttu-id="c3884-1657">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1657">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-1658">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-1658">Interactive</span></span>
* <span data-ttu-id="c3884-1659">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="c3884-1659">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="c3884-1660">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c3884-1660">IoT Central</span></span>
* <span data-ttu-id="c3884-1661">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="c3884-1661">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="c3884-1662">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="c3884-1662">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1663">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1663">Monitor</span></span>
* <span data-ttu-id="c3884-1664">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="c3884-1664">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="c3884-1665">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1665">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="c3884-1666">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c3884-1666">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c3884-1667">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c3884-1667">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="c3884-1668">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="c3884-1668">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="c3884-1669">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c3884-1669">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="c3884-1670">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="c3884-1670">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="c3884-1671">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c3884-1671">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c3884-1672">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c3884-1672">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="c3884-1673">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1673">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1674">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1674">Network</span></span>
* <span data-ttu-id="c3884-1675">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1675">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="c3884-1676">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1676">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="c3884-1677">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c3884-1677">ServiceBus</span></span>
* <span data-ttu-id="c3884-1678">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-1678">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1679">SQL</span></span>
* <span data-ttu-id="c3884-1680">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c3884-1680">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1681">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1681">Storage</span></span>
* <span data-ttu-id="c3884-1682">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="c3884-1682">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="c3884-1683">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="c3884-1683">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1684">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1684">VM</span></span>
* <span data-ttu-id="c3884-1685">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1685">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="c3884-1686">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1686">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="c3884-1687">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1687">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="c3884-1688">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1688">October 16, 2018</span></span>

<span data-ttu-id="c3884-1689">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="c3884-1689">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1690">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1690">VM</span></span>
* <span data-ttu-id="c3884-1691">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="c3884-1691">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="c3884-1692">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1692">October 9, 2018</span></span>

<span data-ttu-id="c3884-1693">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="c3884-1693">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1694">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1694">Core</span></span>
* <span data-ttu-id="c3884-1695">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="c3884-1695">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1696">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1696">ACR</span></span>
* <span data-ttu-id="c3884-1697">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="c3884-1697">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1698">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1698">ACS</span></span>
* <span data-ttu-id="c3884-1699">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="c3884-1699">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="c3884-1700">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="c3884-1700">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="c3884-1701">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="c3884-1701">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="c3884-1702">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="c3884-1702">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1703">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1703">Container</span></span>
* <span data-ttu-id="c3884-1704">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="c3884-1704">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="c3884-1705">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-1705">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="c3884-1706">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c3884-1706">Event Hub</span></span>
* <span data-ttu-id="c3884-1707">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1707">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="c3884-1708">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c3884-1708">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="c3884-1709">Extensions</span><span class="sxs-lookup"><span data-stu-id="c3884-1709">Extensions</span></span>
* <span data-ttu-id="c3884-1710">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="c3884-1710">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c3884-1711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c3884-1711">HDInsight</span></span>
* <span data-ttu-id="c3884-1712">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-1712">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-1713">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1713">IoT</span></span>
* <span data-ttu-id="c3884-1714">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="c3884-1714">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-1715">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-1715">KeyVault</span></span>
* <span data-ttu-id="c3884-1716">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="c3884-1716">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1717">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1717">Network</span></span>
* <span data-ttu-id="c3884-1718">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="c3884-1718">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="c3884-1719">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="c3884-1719">See #6052</span></span>
* <span data-ttu-id="c3884-1720">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1720">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="c3884-1721">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="c3884-1721">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="c3884-1722">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c3884-1722">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="c3884-1723">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c3884-1723">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="c3884-1724">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="c3884-1724">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="c3884-1725">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1725">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1726">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1726">Role</span></span>
* <span data-ttu-id="c3884-1727">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="c3884-1727">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="c3884-1728">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="c3884-1728">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="c3884-1729">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="c3884-1729">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="c3884-1730">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="c3884-1730">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="c3884-1731">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-1731">Service Bus</span></span>
* <span data-ttu-id="c3884-1732">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c3884-1732">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1733">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1733">VM</span></span>
* <span data-ttu-id="c3884-1734">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="c3884-1734">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="c3884-1735">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1735">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="c3884-1736">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="c3884-1736">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="c3884-1737">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="c3884-1737">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="c3884-1738">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1738">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="c3884-1739">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="c3884-1739">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="c3884-1740">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1740">September 21, 2018</span></span>

<span data-ttu-id="c3884-1741">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="c3884-1741">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1742">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1742">ACR</span></span>
* <span data-ttu-id="c3884-1743">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1743">Added ACR Task commands</span></span>
* <span data-ttu-id="c3884-1744">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="c3884-1744">Added quick run command</span></span>
* <span data-ttu-id="c3884-1745">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c3884-1745">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="c3884-1746">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1746">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="c3884-1747">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="c3884-1747">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="c3884-1748">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="c3884-1748">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1749">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1749">ACS</span></span>
* <span data-ttu-id="c3884-1750">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-1750">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="c3884-1751">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="c3884-1751">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1752">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1752">AppService</span></span>

* <span data-ttu-id="c3884-1753">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="c3884-1753">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="c3884-1754">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="c3884-1754">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="c3884-1755">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="c3884-1755">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="c3884-1756">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="c3884-1756">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-1757">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-1757">Batch</span></span>
* <span data-ttu-id="c3884-1758">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="c3884-1758">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="c3884-1759">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="c3884-1759">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="c3884-1760">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1760">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="c3884-1761">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="c3884-1761">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c3884-1762">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-1762">Batch AI</span></span> 
* <span data-ttu-id="c3884-1763">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1763">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c3884-1764">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-1764">Cognitive Services</span></span>
* <span data-ttu-id="c3884-1765">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="c3884-1765">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="c3884-1766">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="c3884-1766">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="c3884-1767">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="c3884-1767">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="c3884-1768">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1768">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="c3884-1769">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c3884-1769">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="c3884-1770">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="c3884-1770">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1771">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1771">Container</span></span>
* <span data-ttu-id="c3884-1772">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="c3884-1772">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="c3884-1773">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1773">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="c3884-1774">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c3884-1774">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="c3884-1775">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-1775">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="c3884-1776">DataLake</span><span class="sxs-lookup"><span data-stu-id="c3884-1776">Datalake</span></span>
* <span data-ttu-id="c3884-1777">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c3884-1777">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="c3884-1778">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="c3884-1778">Interactive Shell</span></span>
* <span data-ttu-id="c3884-1779">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-1779">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="c3884-1780">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="c3884-1780">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-1781">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1781">IoT</span></span>
* <span data-ttu-id="c3884-1782">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1782">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-1783">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c3884-1783">Key Vault</span></span>
* <span data-ttu-id="c3884-1784">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="c3884-1784">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1785">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1785">Network</span></span>
* <span data-ttu-id="c3884-1786">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1786">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="c3884-1787">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="c3884-1787">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="c3884-1788">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="c3884-1788">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="c3884-1789">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1789">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="c3884-1790">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1790">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="c3884-1791">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c3884-1791">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="c3884-1792">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="c3884-1792">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="c3884-1793">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="c3884-1793">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="c3884-1794">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="c3884-1794">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="c3884-1795">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="c3884-1795">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="c3884-1796">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="c3884-1796">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="c3884-1797">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="c3884-1797">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="c3884-1798">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="c3884-1798">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="c3884-1799">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="c3884-1799">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="c3884-1800">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="c3884-1800">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="c3884-1801">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="c3884-1801">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="c3884-1802">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1802">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="c3884-1803">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="c3884-1803">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-1804">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-1804">RDBMS</span></span>
* <span data-ttu-id="c3884-1805">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="c3884-1805">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="c3884-1806">Réservation</span><span class="sxs-lookup"><span data-stu-id="c3884-1806">Reservation</span></span>
* <span data-ttu-id="c3884-1807">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="c3884-1807">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="c3884-1808">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="c3884-1808">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="c3884-1809">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="c3884-1809">Manage App</span></span>
* <span data-ttu-id="c3884-1810">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="c3884-1810">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="c3884-1811">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="c3884-1811">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1812">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1812">Role</span></span>
* <span data-ttu-id="c3884-1813">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="c3884-1813">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="c3884-1814">SignalR</span><span class="sxs-lookup"><span data-stu-id="c3884-1814">SignalR</span></span>
* <span data-ttu-id="c3884-1815">Première version</span><span class="sxs-lookup"><span data-stu-id="c3884-1815">First release</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1816">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1816">Storage</span></span>
* <span data-ttu-id="c3884-1817">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="c3884-1817">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="c3884-1818">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="c3884-1818">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1819">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1819">VM</span></span>
* <span data-ttu-id="c3884-1820">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="c3884-1820">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="c3884-1821">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="c3884-1821">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="c3884-1822">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1822">August 28, 2018</span></span>

<span data-ttu-id="c3884-1823">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="c3884-1823">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1824">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1824">Core</span></span>

* <span data-ttu-id="c3884-1825">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="c3884-1825">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="c3884-1826">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c3884-1826">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1827">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1827">ACR</span></span>

* <span data-ttu-id="c3884-1828">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-1828">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="c3884-1829">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="c3884-1829">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1830">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1830">ACS</span></span>

* <span data-ttu-id="c3884-1831">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="c3884-1831">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="c3884-1832">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="c3884-1832">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1833">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1833">AppService</span></span>

* <span data-ttu-id="c3884-1834">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="c3884-1834">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="c3884-1835">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="c3884-1835">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="c3884-1836">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1836">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-1837">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-1837">Backup</span></span>

* <span data-ttu-id="c3884-1838">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1838">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="c3884-1839">Service de robot</span><span class="sxs-lookup"><span data-stu-id="c3884-1839">Bot Service</span></span>

* <span data-ttu-id="c3884-1840">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="c3884-1840">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c3884-1841">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-1841">Cognitive Services</span></span>

* <span data-ttu-id="c3884-1842">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="c3884-1842">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-1843">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1843">IoT</span></span>

* <span data-ttu-id="c3884-1844">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="c3884-1844">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-1845">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-1845">Monitor</span></span>

* <span data-ttu-id="c3884-1846">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="c3884-1846">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="c3884-1847">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="c3884-1847">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1848">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1848">Network</span></span>

* <span data-ttu-id="c3884-1849">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1849">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-1850">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1850">Resource</span></span>

* <span data-ttu-id="c3884-1851">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1851">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1852">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1852">Storage</span></span>

* <span data-ttu-id="c3884-1853">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1853">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1854">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1854">VM</span></span>

* <span data-ttu-id="c3884-1855">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1855">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="c3884-1856">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1856">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="c3884-1857">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1857">Auguest 14, 2018</span></span>

<span data-ttu-id="c3884-1858">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="c3884-1858">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1859">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1859">Core</span></span>

* <span data-ttu-id="c3884-1860">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="c3884-1860">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="c3884-1861">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="c3884-1861">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="c3884-1862">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="c3884-1862">Telemetry</span></span>

* <span data-ttu-id="c3884-1863">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c3884-1863">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1864">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1864">ACR</span></span>

* <span data-ttu-id="c3884-1865">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-1865">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="c3884-1866">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c3884-1866">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1867">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1867">ACS</span></span>

* <span data-ttu-id="c3884-1868">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-1868">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="c3884-1869">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-1869">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="c3884-1870">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c3884-1870">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="c3884-1871">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c3884-1871">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="c3884-1872">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="c3884-1872">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="c3884-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1873">AppService</span></span>

* <span data-ttu-id="c3884-1874">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c3884-1874">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="c3884-1875">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="c3884-1875">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-1876">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-1876">BatchAI</span></span>

* <span data-ttu-id="c3884-1877">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="c3884-1877">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="c3884-1878">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1878">Container</span></span>

* <span data-ttu-id="c3884-1879">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1879">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="c3884-1880">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-1880">IoT</span></span>

* <span data-ttu-id="c3884-1881">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="c3884-1881">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="c3884-1882">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="c3884-1882">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="c3884-1883">Iot Central</span><span class="sxs-lookup"><span data-stu-id="c3884-1883">Iot Central</span></span>

* <span data-ttu-id="c3884-1884">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="c3884-1884">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-1885">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-1885">KeyVault</span></span>


* <span data-ttu-id="c3884-1886">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="c3884-1886">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="c3884-1887">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1887">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="c3884-1888">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="c3884-1888">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="c3884-1889">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c3884-1889">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="c3884-1890">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c3884-1890">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="c3884-1891">Relais</span><span class="sxs-lookup"><span data-stu-id="c3884-1891">Relay</span></span>

* <span data-ttu-id="c3884-1892">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-1892">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1893">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1893">Sql</span></span>

* <span data-ttu-id="c3884-1894">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="c3884-1894">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1895">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1895">Storage</span></span>

* <span data-ttu-id="c3884-1896">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="c3884-1896">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="c3884-1897">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="c3884-1897">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="c3884-1898">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="c3884-1898">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="c3884-1899">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="c3884-1899">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="c3884-1900">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1900">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1901">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1901">VM</span></span>

* <span data-ttu-id="c3884-1902">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="c3884-1902">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="c3884-1903">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1903">July 31, 2018</span></span>

<span data-ttu-id="c3884-1904">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="c3884-1904">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1905">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1905">ACR</span></span>

* <span data-ttu-id="c3884-1906">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="c3884-1906">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="c3884-1907">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="c3884-1907">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1908">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1908">ACS</span></span>

* <span data-ttu-id="c3884-1909">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="c3884-1909">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-1910">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-1910">Batch</span></span>

* <span data-ttu-id="c3884-1911">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-1911">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1912">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1912">Container</span></span>

* <span data-ttu-id="c3884-1913">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="c3884-1913">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1914">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1914">Network</span></span>

* <span data-ttu-id="c3884-1915">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c3884-1915">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="c3884-1916">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1916">Resource</span></span>

* <span data-ttu-id="c3884-1917">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-1917">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="c3884-1918">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-1918">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="c3884-1919">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-1919">Role</span></span>

* <span data-ttu-id="c3884-1920">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="c3884-1920">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="c3884-1921">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-1921">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="c3884-1922">Recherche</span><span class="sxs-lookup"><span data-stu-id="c3884-1922">Search</span></span>

* <span data-ttu-id="c3884-1923">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="c3884-1923">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="c3884-1924">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-1924">Service Bus</span></span>

* <span data-ttu-id="c3884-1925">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="c3884-1925">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="c3884-1926">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1926">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="c3884-1927">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="c3884-1927">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="c3884-1928">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="c3884-1928">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1929">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1929">Storage</span></span>

* <span data-ttu-id="c3884-1930">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="c3884-1930">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="c3884-1931">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1931">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1932">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1932">VM</span></span>

* <span data-ttu-id="c3884-1933">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1933">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="c3884-1934">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="c3884-1934">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="c3884-1935">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="c3884-1935">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="c3884-1936">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="c3884-1936">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="c3884-1937">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1937">July 18, 2018</span></span>

<span data-ttu-id="c3884-1938">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="c3884-1938">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1939">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1939">Core</span></span>

* <span data-ttu-id="c3884-1940">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-1940">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="c3884-1941">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c3884-1941">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="c3884-1942">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c3884-1942">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1943">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1943">ACR</span></span>

* <span data-ttu-id="c3884-1944">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="c3884-1944">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="c3884-1945">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="c3884-1945">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="c3884-1946">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="c3884-1946">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="c3884-1947">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="c3884-1947">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1948">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1948">ACS</span></span>

* <span data-ttu-id="c3884-1949">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="c3884-1949">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-1950">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-1950">AppService</span></span>

* <span data-ttu-id="c3884-1951">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="c3884-1951">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-1952">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-1952">Batch</span></span>

* <span data-ttu-id="c3884-1953">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-1953">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="c3884-1954">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-1954">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c3884-1955">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-1955">Batch AI</span></span>

* <span data-ttu-id="c3884-1956">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="c3884-1956">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="c3884-1957">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-1957">Container</span></span>

* <span data-ttu-id="c3884-1958">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="c3884-1958">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="c3884-1959">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="c3884-1959">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="c3884-1960">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-1960">Network</span></span>

* <span data-ttu-id="c3884-1961">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1961">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="c3884-1962">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1962">Added `network nic wait`</span></span>
* <span data-ttu-id="c3884-1963">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1963">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="c3884-1964">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="c3884-1964">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="c3884-1965">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-1965">Resource</span></span>

* <span data-ttu-id="c3884-1966">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-1966">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="c3884-1967">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-1967">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="c3884-1968">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1968">Added `deployment wait` command</span></span>
* <span data-ttu-id="c3884-1969">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="c3884-1969">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-1970">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-1970">SQL</span></span>

* <span data-ttu-id="c3884-1971">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="c3884-1971">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="c3884-1972">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="c3884-1972">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="c3884-1973">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="c3884-1973">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-1974">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-1974">Storage</span></span>

* <span data-ttu-id="c3884-1975">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="c3884-1975">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-1976">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-1976">VM</span></span>

* <span data-ttu-id="c3884-1977">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1977">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="c3884-1978">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="c3884-1978">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="c3884-1979">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="c3884-1979">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c3884-1980">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1980">July 3, 2018</span></span>

<span data-ttu-id="c3884-1981">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="c3884-1981">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-1982">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-1982">AKS</span></span>

* <span data-ttu-id="c3884-1983">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-1983">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c3884-1984">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-1984">July 3, 2018</span></span>

<span data-ttu-id="c3884-1985">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="c3884-1985">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="c3884-1986">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-1986">Core</span></span>

* <span data-ttu-id="c3884-1987">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-1987">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-1988">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-1988">ACR</span></span>

* <span data-ttu-id="c3884-1989">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="c3884-1989">Added polling build status</span></span>
* <span data-ttu-id="c3884-1990">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-1990">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="c3884-1991">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c3884-1991">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-1992">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-1992">ACS</span></span>

* <span data-ttu-id="c3884-1993">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1993">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="c3884-1994">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-1994">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="c3884-1995">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1995">Updated options for `aks browse` command.</span></span> <span data-ttu-id="c3884-1996">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="c3884-1996">Added `--listen-port` support</span></span>
* <span data-ttu-id="c3884-1997">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c3884-1997">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="c3884-1998">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="c3884-1998">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="c3884-1999">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="c3884-1999">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2000">AppService</span></span>

* <span data-ttu-id="c3884-2001">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="c3884-2001">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="c3884-2002">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="c3884-2002">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-2003">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-2003">Backup</span></span>

* <span data-ttu-id="c3884-2004">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="c3884-2004">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-2005">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2005">BatchAI</span></span>

* <span data-ttu-id="c3884-2006">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2006">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="c3884-2007">Cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-2007">Cloud</span></span>

* <span data-ttu-id="c3884-2008">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-2008">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2009">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2009">Container</span></span>

* <span data-ttu-id="c3884-2010">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="c3884-2010">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="c3884-2011">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="c3884-2011">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="c3884-2012">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="c3884-2012">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2013">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2013">Extension</span></span>

* <span data-ttu-id="c3884-2014">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="c3884-2014">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2015">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2015">Network</span></span>

* <span data-ttu-id="c3884-2016">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="c3884-2016">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-2017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c3884-2017">Rdbms</span></span>

* <span data-ttu-id="c3884-2018">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-2018">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2019">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2019">Resource</span></span>

* <span data-ttu-id="c3884-2020">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="c3884-2020">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2021">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2021">VM</span></span>

* <span data-ttu-id="c3884-2022">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="c3884-2022">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="c3884-2023">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2023">June 25, 2018</span></span>

<span data-ttu-id="c3884-2024">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="c3884-2024">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="c3884-2025">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2025">CLI</span></span>

* <span data-ttu-id="c3884-2026">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2026">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="c3884-2027">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2027">June 19, 2018</span></span>

<span data-ttu-id="c3884-2028">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="c3884-2028">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2029">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2029">Core</span></span>

* <span data-ttu-id="c3884-2030">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2030">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2031">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2031">ACR</span></span>

* <span data-ttu-id="c3884-2032">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="c3884-2032">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="c3884-2033">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2033">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2034">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2034">ACS</span></span>

* <span data-ttu-id="c3884-2035">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2035">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="c3884-2036">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2036">Added `--update` support</span></span>
* <span data-ttu-id="c3884-2037">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="c3884-2037">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="c3884-2038">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="c3884-2038">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="c3884-2039">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="c3884-2039">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="c3884-2040">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c3884-2040">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="c3884-2041">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c3884-2041">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="c3884-2042">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c3884-2042">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2043">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2043">AppService</span></span>

* <span data-ttu-id="c3884-2044">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="c3884-2044">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="c3884-2045">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c3884-2045">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2046">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2046">Batch</span></span>

* <span data-ttu-id="c3884-2047">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="c3884-2047">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c3884-2048">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2048">Batch AI</span></span>

* <span data-ttu-id="c3884-2049">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="c3884-2049">Added support for workspaces.</span></span> <span data-ttu-id="c3884-2050">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="c3884-2050">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="c3884-2051">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="c3884-2051">Added support for experiments.</span></span> <span data-ttu-id="c3884-2052">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="c3884-2052">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="c3884-2053">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="c3884-2053">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="c3884-2054">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2054">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="c3884-2055">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="c3884-2055">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="c3884-2056">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="c3884-2056">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="c3884-2057">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2057">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="c3884-2058">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="c3884-2058">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="c3884-2059">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2059">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="c3884-2060">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="c3884-2060">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="c3884-2061">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2061">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="c3884-2062">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="c3884-2062">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="c3884-2063">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="c3884-2063">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="c3884-2064">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="c3884-2064">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="c3884-2065">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2065">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="c3884-2066">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="c3884-2066">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="c3884-2067">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="c3884-2067">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="c3884-2068">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c3884-2068">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c3884-2069">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c3884-2069">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c3884-2070">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="c3884-2070">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="c3884-2071">Cartes</span><span class="sxs-lookup"><span data-stu-id="c3884-2071">Maps</span></span>

* <span data-ttu-id="c3884-2072">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="c3884-2072">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2073">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2073">Network</span></span>

* <span data-ttu-id="c3884-2074">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="c3884-2074">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="c3884-2075">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="c3884-2075">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="c3884-2076">#6502</span><span class="sxs-lookup"><span data-stu-id="c3884-2076">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="c3884-2077">Réservations</span><span class="sxs-lookup"><span data-stu-id="c3884-2077">Reservations</span></span>

* <span data-ttu-id="c3884-2078">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2078">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="c3884-2079">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2079">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="c3884-2080">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="c3884-2080">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="c3884-2081">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c3884-2081">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="c3884-2082">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c3884-2082">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="c3884-2083">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2083">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2084">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2084">Role</span></span>

* <span data-ttu-id="c3884-2085">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2085">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2086">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2086">SQL</span></span>

* <span data-ttu-id="c3884-2087">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-2087">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2088">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2088">Storage</span></span>

* <span data-ttu-id="c3884-2089">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="c3884-2089">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2090">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2090">VM</span></span>

* <span data-ttu-id="c3884-2091">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2091">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="c3884-2092">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="c3884-2092">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="c3884-2093">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="c3884-2093">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c3884-2094">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2094">June 13, 2018</span></span>

<span data-ttu-id="c3884-2095">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="c3884-2095">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2096">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2096">Core</span></span>

* <span data-ttu-id="c3884-2097">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2097">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c3884-2098">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2098">June 13, 2018</span></span>

<span data-ttu-id="c3884-2099">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="c3884-2099">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-2100">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-2100">AKS</span></span>

* <span data-ttu-id="c3884-2101">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2101">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="c3884-2102">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="c3884-2102">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="c3884-2103">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2103">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="c3884-2104">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2104">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="c3884-2105">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2105">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2106">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2106">AppService</span></span>

* <span data-ttu-id="c3884-2107">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="c3884-2107">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c3884-2108">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2108">June 5, 2018</span></span>

<span data-ttu-id="c3884-2109">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="c3884-2109">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2110">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2110">Interactive</span></span>

* <span data-ttu-id="c3884-2111">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c3884-2111">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c3884-2112">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2112">June 5, 2018</span></span>

<span data-ttu-id="c3884-2113">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="c3884-2113">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2114">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2114">Core</span></span>

* <span data-ttu-id="c3884-2115">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="c3884-2115">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="c3884-2116">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c3884-2116">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2117">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2117">ACR</span></span>

* <span data-ttu-id="c3884-2118">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="c3884-2118">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="c3884-2119">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="c3884-2119">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="c3884-2120">AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-2120">AKS</span></span>

* <span data-ttu-id="c3884-2121">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="c3884-2121">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2122">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2122">Batch</span></span>

* <span data-ttu-id="c3884-2123">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="c3884-2123">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-2124">IOT</span><span class="sxs-lookup"><span data-stu-id="c3884-2124">IOT</span></span>

* <span data-ttu-id="c3884-2125">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="c3884-2125">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2126">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2126">Network</span></span>

* <span data-ttu-id="c3884-2127">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="c3884-2127">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c3884-2128">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c3884-2128">Policy Insights</span></span>

* <span data-ttu-id="c3884-2129">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2129">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="c3884-2130">ARM</span><span class="sxs-lookup"><span data-stu-id="c3884-2130">ARM</span></span>

* <span data-ttu-id="c3884-2131">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2131">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2132">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2132">SQL</span></span>

* <span data-ttu-id="c3884-2133">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="c3884-2133">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="c3884-2134">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="c3884-2134">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="c3884-2135">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2135">Storage</span></span>

* <span data-ttu-id="c3884-2136">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="c3884-2136">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2137">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2137">VM</span></span>

* <span data-ttu-id="c3884-2138">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="c3884-2138">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="c3884-2139">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2139">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="c3884-2140">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2140">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="c3884-2141">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2141">May 22, 2018</span></span>

<span data-ttu-id="c3884-2142">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="c3884-2142">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2143">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2143">Core</span></span>

* <span data-ttu-id="c3884-2144">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="c3884-2144">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2145">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2145">ACS</span></span>

* <span data-ttu-id="c3884-2146">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="c3884-2146">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="c3884-2147">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-2147">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2148">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2148">AppService</span></span>

* <span data-ttu-id="c3884-2149">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c3884-2149">Improved generic update commands</span></span>
* <span data-ttu-id="c3884-2150">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="c3884-2150">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2151">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2151">Container</span></span>

* <span data-ttu-id="c3884-2152">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="c3884-2152">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="c3884-2153">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2153">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2154">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2154">Extension</span></span>

* <span data-ttu-id="c3884-2155">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="c3884-2155">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2156">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2156">Interactive</span></span>

* <span data-ttu-id="c3884-2157">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="c3884-2157">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="c3884-2158">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="c3884-2158">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-2159">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-2159">KeyVault</span></span>

* <span data-ttu-id="c3884-2160">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c3884-2160">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2161">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2161">Network</span></span>

* <span data-ttu-id="c3884-2162">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="c3884-2162">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="c3884-2163">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="c3884-2163">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2164">SQL</span></span>

* <span data-ttu-id="c3884-2165">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="c3884-2165">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="c3884-2166">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="c3884-2166">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="c3884-2167">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="c3884-2167">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="c3884-2168">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c3884-2168">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="c3884-2169">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c3884-2169">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="c3884-2170">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2170">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="c3884-2171">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="c3884-2171">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="c3884-2172">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2172">`edition`.</span></span> <span data-ttu-id="c3884-2173">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="c3884-2173">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="c3884-2174">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2174">`elasticPoolName`.</span></span> <span data-ttu-id="c3884-2175">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="c3884-2175">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="c3884-2176">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c3884-2176">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="c3884-2177">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2177">`edition`.</span></span> <span data-ttu-id="c3884-2178">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="c3884-2178">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="c3884-2179">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2179">`dtu`.</span></span> <span data-ttu-id="c3884-2180">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="c3884-2180">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="c3884-2181">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2181">`databaseDtuMin`.</span></span> <span data-ttu-id="c3884-2182">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="c3884-2182">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="c3884-2183">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2183">`databaseDtuMax`.</span></span> <span data-ttu-id="c3884-2184">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="c3884-2184">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="c3884-2185">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c3884-2185">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="c3884-2186">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c3884-2186">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2187">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2187">Storage</span></span>

* <span data-ttu-id="c3884-2188">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-2188">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="c3884-2189">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="c3884-2189">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2190">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2190">VM</span></span>

* <span data-ttu-id="c3884-2191">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2191">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="c3884-2192">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="c3884-2192">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="c3884-2193">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="c3884-2193">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="c3884-2194">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="c3884-2194">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="c3884-2195">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2195">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="c3884-2196">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2196">May 7, 2018</span></span>

<span data-ttu-id="c3884-2197">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="c3884-2197">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2198">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2198">Core</span></span>

* <span data-ttu-id="c3884-2199">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="c3884-2199">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="c3884-2200">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="c3884-2200">Added limited support for positional arguments</span></span>
* <span data-ttu-id="c3884-2201">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2201">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="c3884-2202">#5591</span><span class="sxs-lookup"><span data-stu-id="c3884-2202">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="c3884-2203">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2203">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="c3884-2204">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="c3884-2204">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="c3884-2205">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2205">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="c3884-2206">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="c3884-2206">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="c3884-2207">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2207">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2208">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2208">ACR</span></span>

* <span data-ttu-id="c3884-2209">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2209">Added ACR Build commands</span></span>
* <span data-ttu-id="c3884-2210">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="c3884-2210">Improved resource not found error messages</span></span>
* <span data-ttu-id="c3884-2211">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2211">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="c3884-2212">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="c3884-2212">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="c3884-2213">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="c3884-2213">Improved repository commands error messages</span></span>
* <span data-ttu-id="c3884-2214">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="c3884-2214">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2215">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2215">ACS</span></span>

* <span data-ttu-id="c3884-2216">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2216">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="c3884-2217">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c3884-2217">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="c3884-2218">AMS</span><span class="sxs-lookup"><span data-stu-id="c3884-2218">AMS</span></span>

* <span data-ttu-id="c3884-2219">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="c3884-2219">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2220">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2220">Appservice</span></span>

* <span data-ttu-id="c3884-2221">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="c3884-2221">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="c3884-2222">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2222">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="c3884-2223">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="c3884-2223">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="c3884-2224">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2224">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c3884-2225">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2225">Batch AI</span></span>

* <span data-ttu-id="c3884-2226">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="c3884-2226">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c3884-2227">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-2227">Cognitive Services</span></span>

* <span data-ttu-id="c3884-2228">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="c3884-2228">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-2229">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-2229">Consumption</span></span>

* <span data-ttu-id="c3884-2230">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="c3884-2230">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2231">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2231">Container</span></span>

* <span data-ttu-id="c3884-2232">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="c3884-2232">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c3884-2233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-2233">Cosmos DB</span></span>

* <span data-ttu-id="c3884-2234">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3884-2234">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="c3884-2235">DMS</span><span class="sxs-lookup"><span data-stu-id="c3884-2235">DMS</span></span>

* <span data-ttu-id="c3884-2236">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="c3884-2236">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2237">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2237">Extension</span></span>

* <span data-ttu-id="c3884-2238">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="c3884-2238">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2239">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2239">Interactive</span></span>

* <span data-ttu-id="c3884-2240">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="c3884-2240">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="c3884-2241">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="c3884-2241">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="c3884-2242">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="c3884-2242">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="c3884-2243">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2243">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="c3884-2244">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-2244">Lab</span></span>

* <span data-ttu-id="c3884-2245">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="c3884-2245">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2246">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2246">Network</span></span>

* <span data-ttu-id="c3884-2247">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="c3884-2247">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="c3884-2248">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2248">Profile</span></span>

* <span data-ttu-id="c3884-2249">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2249">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="c3884-2250">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="c3884-2250">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="c3884-2251">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="c3884-2251">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="c3884-2252">Redis</span><span class="sxs-lookup"><span data-stu-id="c3884-2252">Redis</span></span>

* <span data-ttu-id="c3884-2253">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2253">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="c3884-2254">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="c3884-2254">Deprecated `redis list-all`.</span></span> <span data-ttu-id="c3884-2255">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2255">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="c3884-2256">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="c3884-2256">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="c3884-2257">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2257">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2258">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2258">Role</span></span>

* <span data-ttu-id="c3884-2259">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c3884-2259">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2260">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2260">Storage</span></span>

* <span data-ttu-id="c3884-2261">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="c3884-2261">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="c3884-2262">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="c3884-2262">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="c3884-2263">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="c3884-2263">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="c3884-2264">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="c3884-2264">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="c3884-2265">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2265">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2266">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2266">VM</span></span>

* <span data-ttu-id="c3884-2267">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="c3884-2267">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="c3884-2268">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c3884-2268">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="c3884-2269">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="c3884-2269">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="c3884-2270">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="c3884-2270">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="c3884-2271">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="c3884-2271">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="c3884-2272">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="c3884-2272">Added write accelerator support</span></span>
* <span data-ttu-id="c3884-2273">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c3884-2273">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="c3884-2274">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2274">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="c3884-2275">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="c3884-2275">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="c3884-2276">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2276">April 10, 2018</span></span>

<span data-ttu-id="c3884-2277">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="c3884-2277">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2278">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2278">ACR</span></span>

* <span data-ttu-id="c3884-2279">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="c3884-2279">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2280">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2280">ACS</span></span>

* <span data-ttu-id="c3884-2281">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="c3884-2281">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2282">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="c3884-2284">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="c3884-2284">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-2285">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2285">BatchAI</span></span>

* <span data-ttu-id="c3884-2286">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="c3884-2286">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="c3884-2287">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2287">Job level mounting</span></span>
  - <span data-ttu-id="c3884-2288">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="c3884-2288">Environment variables with secret values</span></span>
  - <span data-ttu-id="c3884-2289">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="c3884-2289">Performance counters settings</span></span>
  - <span data-ttu-id="c3884-2290">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2290">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="c3884-2291">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="c3884-2291">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="c3884-2292">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="c3884-2292">Usage and limits reporting</span></span>
  - <span data-ttu-id="c3884-2293">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="c3884-2293">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="c3884-2294">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="c3884-2294">Support for custom images</span></span>
  - <span data-ttu-id="c3884-2295">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="c3884-2295">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="c3884-2296">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2296">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="c3884-2297">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="c3884-2297">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="c3884-2298">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="c3884-2298">National clouds are supported</span></span>
* <span data-ttu-id="c3884-2299">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="c3884-2299">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="c3884-2300">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="c3884-2300">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="c3884-2301">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2301">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="c3884-2302">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="c3884-2302">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="c3884-2303">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="c3884-2303">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="c3884-2304">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="c3884-2304">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="c3884-2305">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2305">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="c3884-2306">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="c3884-2306">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="c3884-2307">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="c3884-2307">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="c3884-2308">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2308">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="c3884-2309">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2309">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="c3884-2310">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="c3884-2310">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="c3884-2311">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2311">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="c3884-2312">Facturation</span><span class="sxs-lookup"><span data-stu-id="c3884-2312">Billing</span></span>

* <span data-ttu-id="c3884-2313">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="c3884-2313">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-2314">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-2314">Consumption</span></span>

* <span data-ttu-id="c3884-2315">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="c3884-2315">Added `marketplace` commands</span></span>
* <span data-ttu-id="c3884-2316">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c3884-2316">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="c3884-2317">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="c3884-2317">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="c3884-2318">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="c3884-2318">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="c3884-2319">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c3884-2319">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="c3884-2320">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="c3884-2320">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2321">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2321">Container</span></span>

* <span data-ttu-id="c3884-2322">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="c3884-2322">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="c3884-2323">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="c3884-2323">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2324">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2324">Extension</span></span>

* <span data-ttu-id="c3884-2325">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="c3884-2325">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2326">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2326">Interactive</span></span>

* <span data-ttu-id="c3884-2327">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="c3884-2327">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="c3884-2328">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2328">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="c3884-2329">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="c3884-2329">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2330">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2330">Network</span></span>

* <span data-ttu-id="c3884-2331">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="c3884-2331">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="c3884-2332">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2332">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="c3884-2333">#4910</span><span class="sxs-lookup"><span data-stu-id="c3884-2333">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="c3884-2334">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c3884-2334">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="c3884-2335">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c3884-2335">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="c3884-2336">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2336">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="c3884-2337">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2337">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="c3884-2338">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="c3884-2338">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2339">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2339">Profile</span></span>

* <span data-ttu-id="c3884-2340">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2340">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="c3884-2341">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="c3884-2341">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-2342">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-2342">RDBMS</span></span>

* <span data-ttu-id="c3884-2343">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="c3884-2343">Added `georestore` command</span></span>
* <span data-ttu-id="c3884-2344">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2344">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2345">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2345">Resource</span></span>

* <span data-ttu-id="c3884-2346">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2346">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="c3884-2347">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2347">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2348">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2348">SQL</span></span>

* <span data-ttu-id="c3884-2349">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="c3884-2349">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2350">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2350">Storage</span></span>

* <span data-ttu-id="c3884-2351">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="c3884-2351">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2352">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2352">VM</span></span>

* <span data-ttu-id="c3884-2353">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2353">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="c3884-2354">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="c3884-2354">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="c3884-2356">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2356">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="c3884-2357">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="c3884-2357">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="c3884-2358">#5718</span><span class="sxs-lookup"><span data-stu-id="c3884-2358">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="c3884-2359">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="c3884-2359">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="c3884-2360">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2360">March 27, 2018</span></span>

<span data-ttu-id="c3884-2361">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="c3884-2361">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2362">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2362">Core</span></span>

* <span data-ttu-id="c3884-2363">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="c3884-2363">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2364">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2364">ACS</span></span>

* <span data-ttu-id="c3884-2365">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-2365">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2366">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2366">Appservice</span></span>

* <span data-ttu-id="c3884-2367">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2367">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="c3884-2368">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2368">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-2369">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-2369">Backup</span></span>

* <span data-ttu-id="c3884-2370">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="c3884-2370">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="c3884-2371">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-2371">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="c3884-2372">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3884-2372">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="c3884-2373">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2373">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2374">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2374">Container</span></span>

* <span data-ttu-id="c3884-2375">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="c3884-2375">Added `container exec` command.</span></span> <span data-ttu-id="c3884-2376">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="c3884-2376">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="c3884-2377">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2377">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2378">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2378">Extension</span></span>

* <span data-ttu-id="c3884-2379">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2379">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="c3884-2380">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="c3884-2380">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="c3884-2381">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2381">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2382">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2382">Interactive</span></span>

* <span data-ttu-id="c3884-2383">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2383">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="c3884-2384">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="c3884-2384">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="c3884-2385">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="c3884-2385">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="c3884-2386">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="c3884-2386">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="c3884-2387">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-2387">Lab</span></span>

* <span data-ttu-id="c3884-2388">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="c3884-2388">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2389">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2389">Monitor</span></span>

* <span data-ttu-id="c3884-2390">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c3884-2390">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="c3884-2391">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="c3884-2391">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="c3884-2392">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c3884-2392">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2393">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2393">Network</span></span>

* <span data-ttu-id="c3884-2394">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c3884-2394">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2395">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2395">Profile</span></span>

* <span data-ttu-id="c3884-2396">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="c3884-2396">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-2397">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-2397">RDBMS</span></span>

* <span data-ttu-id="c3884-2398">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="c3884-2398">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2399">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2399">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="c3884-2401">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2401">Role</span></span>

* <span data-ttu-id="c3884-2402">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2402">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="c3884-2403">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="c3884-2403">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="c3884-2404">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2404">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="c3884-2405">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2405">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="c3884-2406">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="c3884-2406">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2407">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2407">Storage</span></span>

* <span data-ttu-id="c3884-2408">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="c3884-2408">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="c3884-2409">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="c3884-2409">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2410">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2410">VM</span></span>

* <span data-ttu-id="c3884-2411">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="c3884-2411">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="c3884-2412">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2412">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="c3884-2413">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c3884-2413">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="c3884-2414">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="c3884-2414">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="c3884-2415">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2415">March 13, 2018</span></span>

<span data-ttu-id="c3884-2416">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="c3884-2416">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2417">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2417">ACR</span></span>

* <span data-ttu-id="c3884-2418">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-2418">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="c3884-2419">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="c3884-2419">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="c3884-2420">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="c3884-2420">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2421">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2421">ACS</span></span>

* <span data-ttu-id="c3884-2422">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="c3884-2422">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="c3884-2423">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="c3884-2423">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="c3884-2424">Advisor</span><span class="sxs-lookup"><span data-stu-id="c3884-2424">Advisor</span></span>

* <span data-ttu-id="c3884-2425">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2425">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="c3884-2426">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2426">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="c3884-2427">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="c3884-2427">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="c3884-2428">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2428">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="c3884-2429">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2429">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2430">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2430">Appservice</span></span>

* <span data-ttu-id="c3884-2431">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c3884-2431">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="c3884-2432">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2432">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c3884-2433">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c3884-2433">Eventhubs</span></span>

* <span data-ttu-id="c3884-2434">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2434">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2435">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2435">Extension</span></span>

* <span data-ttu-id="c3884-2436">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2436">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2437">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2437">Interactive</span></span>

* <span data-ttu-id="c3884-2438">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="c3884-2438">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="c3884-2439">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="c3884-2439">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="c3884-2440">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="c3884-2440">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="c3884-2441">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="c3884-2441">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2442">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2442">Monitor</span></span>

* <span data-ttu-id="c3884-2443">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="c3884-2443">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="c3884-2444">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="c3884-2444">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="c3884-2445">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="c3884-2445">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="c3884-2446">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-2446">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2447">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2447">Network</span></span>

* <span data-ttu-id="c3884-2448">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2448">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="c3884-2449">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3884-2449">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="c3884-2450">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="c3884-2450">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="c3884-2451">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="c3884-2451">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2452">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2452">Profile</span></span>

* <span data-ttu-id="c3884-2453">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="c3884-2453">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="c3884-2454">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="c3884-2454">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-2455">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-2455">RDBMS</span></span>

* <span data-ttu-id="c3884-2456">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2456">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="c3884-2457">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c3884-2457">Service Bus</span></span>

* <span data-ttu-id="c3884-2458">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2458">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2459">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2459">Storage</span></span>

* <span data-ttu-id="c3884-2460">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="c3884-2460">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="c3884-2461">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="c3884-2461">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2462">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2462">VM</span></span>

* <span data-ttu-id="c3884-2463">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="c3884-2463">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="c3884-2464">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="c3884-2464">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="c3884-2465">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="c3884-2465">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="c3884-2466">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="c3884-2466">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="c3884-2467">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2467">February 27, 2018</span></span>

<span data-ttu-id="c3884-2468">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="c3884-2468">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2469">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2469">Core</span></span>

* <span data-ttu-id="c3884-2470">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="c3884-2470">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="c3884-2471">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="c3884-2471">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="c3884-2472">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="c3884-2472">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2473">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2473">ACS</span></span>

* <span data-ttu-id="c3884-2474">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2474">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="c3884-2475">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="c3884-2475">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="c3884-2476">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c3884-2476">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="c3884-2477">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="c3884-2477">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2478">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2478">Appservice</span></span>

* <span data-ttu-id="c3884-2479">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="c3884-2479">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="c3884-2480">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="c3884-2480">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c3884-2481">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-2481">Cognitive Services</span></span>

* <span data-ttu-id="c3884-2482">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-2482">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-2483">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-2483">Consumption</span></span>

* <span data-ttu-id="c3884-2484">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="c3884-2484">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="c3884-2485">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="c3884-2485">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2486">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2486">Container</span></span>

* <span data-ttu-id="c3884-2487">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="c3884-2487">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2488">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2488">Network</span></span>

* <span data-ttu-id="c3884-2489">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="c3884-2489">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2490">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2490">Resource</span></span>

* <span data-ttu-id="c3884-2491">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="c3884-2491">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2492">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2492">Role</span></span>

* <span data-ttu-id="c3884-2493">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="c3884-2493">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2494">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2494">SQL</span></span>

* <span data-ttu-id="c3884-2495">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="c3884-2495">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2496">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2496">Storage</span></span>

* <span data-ttu-id="c3884-2497">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2497">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2498">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2498">VM</span></span>

* <span data-ttu-id="c3884-2499">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="c3884-2499">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="c3884-2500">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2500">February 13, 2018</span></span>

<span data-ttu-id="c3884-2501">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="c3884-2501">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2502">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2502">Core</span></span>

* <span data-ttu-id="c3884-2503">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="c3884-2503">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2504">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2504">ACS</span></span>

* <span data-ttu-id="c3884-2505">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="c3884-2505">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="c3884-2506">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2506">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="c3884-2507">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-2507">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="c3884-2508">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-2508">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="c3884-2509">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="c3884-2509">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="c3884-2510">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="c3884-2510">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="c3884-2511">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-2511">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="c3884-2512">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="c3884-2512">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2513">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2513">Appservice</span></span>

* <span data-ttu-id="c3884-2514">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="c3884-2514">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="c3884-2515">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="c3884-2515">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-2516">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-2516">CDN</span></span>

* <span data-ttu-id="c3884-2517">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2517">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2518">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2518">Container</span></span>

* <span data-ttu-id="c3884-2519">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="c3884-2519">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="c3884-2520">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2520">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-2521">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-2521">CosmosDB</span></span>

* <span data-ttu-id="c3884-2522">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c3884-2522">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2523">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2523">Extension</span></span>

* <span data-ttu-id="c3884-2524">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2524">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="c3884-2525">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2525">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="c3884-2526">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c3884-2526">Feedback</span></span>

* <span data-ttu-id="c3884-2527">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c3884-2527">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2528">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2528">Interactive</span></span>

* <span data-ttu-id="c3884-2529">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3884-2529">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="c3884-2530">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="c3884-2530">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-2531">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-2531">IoT</span></span>

* <span data-ttu-id="c3884-2532">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c3884-2532">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c3884-2533">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c3884-2533">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c3884-2534">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2534">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="c3884-2535">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="c3884-2535">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2536">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2536">Monitor</span></span>

* <span data-ttu-id="c3884-2537">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2537">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2538">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2538">Network</span></span>

* <span data-ttu-id="c3884-2539">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3884-2539">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="c3884-2540">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2540">Profile</span></span>

* <span data-ttu-id="c3884-2541">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c3884-2541">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2542">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2542">Resource</span></span>

* <span data-ttu-id="c3884-2543">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2543">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2544">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2544">Role</span></span>

* <span data-ttu-id="c3884-2545">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2545">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2546">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2546">SQL</span></span>

* <span data-ttu-id="c3884-2547">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="c3884-2547">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="c3884-2548">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="c3884-2548">Added `sql db rename`</span></span>
* <span data-ttu-id="c3884-2549">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="c3884-2549">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2550">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2550">Storage</span></span>

* <span data-ttu-id="c3884-2551">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="c3884-2551">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2552">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2552">VM</span></span>

* <span data-ttu-id="c3884-2553">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="c3884-2553">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="c3884-2554">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="c3884-2554">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="c3884-2555">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="c3884-2555">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="c3884-2556">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2556">January 31, 2018</span></span>

<span data-ttu-id="c3884-2557">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="c3884-2557">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2558">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2558">Core</span></span>

* <span data-ttu-id="c3884-2559">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="c3884-2559">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="c3884-2560">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-2560">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="c3884-2561">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="c3884-2561">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="c3884-2562">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="c3884-2562">Use `--verbose` to see</span></span>
* <span data-ttu-id="c3884-2563">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="c3884-2563">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2564">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2564">ACS</span></span>

* <span data-ttu-id="c3884-2565">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="c3884-2565">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="c3884-2566">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="c3884-2566">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2567">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2567">Appservice</span></span>

* <span data-ttu-id="c3884-2568">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="c3884-2568">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="c3884-2569">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="c3884-2569">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-2570">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-2570">CDN</span></span>

* <span data-ttu-id="c3884-2571">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2571">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-2572">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-2572">CosmosDB</span></span>

* <span data-ttu-id="c3884-2573">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="c3884-2573">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2574">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2574">Interactive</span></span>

* <span data-ttu-id="c3884-2575">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="c3884-2575">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2576">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2576">Network</span></span>

* <span data-ttu-id="c3884-2577">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2577">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="c3884-2578">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2578">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="c3884-2579">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2579">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="c3884-2580">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2580">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="c3884-2581">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="c3884-2581">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="c3884-2582">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="c3884-2582">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="c3884-2583">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="c3884-2583">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="c3884-2584">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="c3884-2584">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="c3884-2585">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c3884-2585">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="c3884-2586">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="c3884-2586">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2587">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2587">Profile</span></span>

* <span data-ttu-id="c3884-2588">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c3884-2588">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2589">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2589">Resource</span></span>

* <span data-ttu-id="c3884-2590">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="c3884-2590">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2591">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2591">Storage</span></span>

* <span data-ttu-id="c3884-2592">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="c3884-2592">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="c3884-2593">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="c3884-2593">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="c3884-2594">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-2594">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="c3884-2595">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2595">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="c3884-2596">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="c3884-2596">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2597">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2597">VM</span></span>

* <span data-ttu-id="c3884-2598">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="c3884-2598">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="c3884-2599">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="c3884-2599">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="c3884-2600">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="c3884-2600">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="c3884-2601">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2601">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="c3884-2602">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c3884-2602">January 17, 2018</span></span>

<span data-ttu-id="c3884-2603">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="c3884-2603">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2604">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2604">ACR</span></span>

* <span data-ttu-id="c3884-2605">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-2605">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="c3884-2606">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="c3884-2606">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2607">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2607">ACS</span></span>

* <span data-ttu-id="c3884-2608">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c3884-2608">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="c3884-2609">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="c3884-2609">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2610">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2610">Appservice</span></span>

* <span data-ttu-id="c3884-2611">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="c3884-2611">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="c3884-2612">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="c3884-2612">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="c3884-2613">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="c3884-2613">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-2614">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-2614">Backup</span></span>

* <span data-ttu-id="c3884-2615">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="c3884-2615">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="c3884-2616">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="c3884-2616">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="c3884-2617">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-2617">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="c3884-2618">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="c3884-2618">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="c3884-2619">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2619">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2620">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2620">Batch</span></span>

* <span data-ttu-id="c3884-2621">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="c3884-2621">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="c3884-2622">Cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-2622">Cloud</span></span>

* <span data-ttu-id="c3884-2623">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-2623">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-2624">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-2624">Consumption</span></span>

* <span data-ttu-id="c3884-2625">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="c3884-2625">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="c3884-2626">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c3884-2626">Event Grid</span></span>

* <span data-ttu-id="c3884-2627">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c3884-2627">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c3884-2628">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c3884-2628">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c3884-2629">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="c3884-2629">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="c3884-2630">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="c3884-2630">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="c3884-2631">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2631">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="c3884-2632">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2632">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="c3884-2633">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="c3884-2633">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="c3884-2634">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="c3884-2634">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-2635">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-2635">Interactive</span></span>

* <span data-ttu-id="c3884-2636">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="c3884-2636">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="c3884-2637">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="c3884-2637">Fixed errors on startup</span></span>
* <span data-ttu-id="c3884-2638">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="c3884-2638">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-2639">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-2639">IoT</span></span>

* <span data-ttu-id="c3884-2640">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="c3884-2640">Added support for device provisioning service</span></span>
* <span data-ttu-id="c3884-2641">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2641">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="c3884-2642">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-2642">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2643">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2643">Monitor</span></span>

* <span data-ttu-id="c3884-2644">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="c3884-2644">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="c3884-2645">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2645">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="c3884-2646">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="c3884-2646">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2647">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2647">Network</span></span>

* <span data-ttu-id="c3884-2648">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2648">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="c3884-2649">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2649">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2650">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2650">Profile</span></span>

* <span data-ttu-id="c3884-2651">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2651">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2652">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2652">Role</span></span>

* <span data-ttu-id="c3884-2653">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="c3884-2653">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c3884-2654">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c3884-2654">Service Fabric</span></span>

* <span data-ttu-id="c3884-2655">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="c3884-2655">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="c3884-2656">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-2656">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2657">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2657">VM</span></span>

* <span data-ttu-id="c3884-2658">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="c3884-2658">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="c3884-2659">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="c3884-2659">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="c3884-2660">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="c3884-2660">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="c3884-2661">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="c3884-2661">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="c3884-2662">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="c3884-2662">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="c3884-2663">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2663">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c3884-2664">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2664">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="c3884-2665">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="c3884-2665">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="c3884-2666">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2666">December 19, 2017</span></span>

<span data-ttu-id="c3884-2667">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="c3884-2667">Version 2.0.23</span></span>

* <span data-ttu-id="c3884-2668">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2668">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2669">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2669">Container</span></span>

* <span data-ttu-id="c3884-2670">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2670">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2671">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2671">Network</span></span>

* <span data-ttu-id="c3884-2672">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2672">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="c3884-2673">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2673">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2674">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2674">Storage</span></span>

* <span data-ttu-id="c3884-2675">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="c3884-2675">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2676">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2676">VM</span></span>

* <span data-ttu-id="c3884-2677">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="c3884-2677">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="c3884-2678">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2678">December 5, 2017</span></span>

<span data-ttu-id="c3884-2679">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="c3884-2679">Version 2.0.22</span></span>

* <span data-ttu-id="c3884-2680">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="c3884-2680">Removed `az component` commands.</span></span> <span data-ttu-id="c3884-2681">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="c3884-2681">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2682">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2682">Core</span></span>
* <span data-ttu-id="c3884-2683">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="c3884-2683">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="c3884-2684">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="c3884-2684">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2685">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2685">ACS</span></span>

* <span data-ttu-id="c3884-2686">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c3884-2686">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="c3884-2687">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2687">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="c3884-2688">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="c3884-2688">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="c3884-2689">Advisor</span><span class="sxs-lookup"><span data-stu-id="c3884-2689">Advisor</span></span>

* <span data-ttu-id="c3884-2690">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2690">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2691">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2691">Appservice</span></span>

* <span data-ttu-id="c3884-2692">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="c3884-2692">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="c3884-2693">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="c3884-2693">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="c3884-2694">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="c3884-2694">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="c3884-2695">Consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-2695">Consumption</span></span>

* <span data-ttu-id="c3884-2696">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="c3884-2696">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2697">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2697">Container</span></span>

* <span data-ttu-id="c3884-2698">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2698">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2699">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2699">Monitor</span></span>

* <span data-ttu-id="c3884-2700">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="c3884-2700">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2701">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2701">Resource</span></span>

* <span data-ttu-id="c3884-2702">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2702">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="c3884-2703">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-2703">Role</span></span>

* <span data-ttu-id="c3884-2704">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="c3884-2704">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="c3884-2705">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="c3884-2705">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="c3884-2706">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c3884-2706">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2707">SQL</span></span>

* <span data-ttu-id="c3884-2708">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="c3884-2708">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="c3884-2709">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2709">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2710">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2710">VM</span></span>

* <span data-ttu-id="c3884-2711">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="c3884-2711">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="c3884-2712">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2712">November 14, 2017</span></span>

<span data-ttu-id="c3884-2713">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="c3884-2713">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2714">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2714">ACR</span></span>

* <span data-ttu-id="c3884-2715">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="c3884-2715">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="c3884-2716">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2716">ACS</span></span>

* <span data-ttu-id="c3884-2717">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="c3884-2717">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="c3884-2718">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2718">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="c3884-2719">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="c3884-2719">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="c3884-2720">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-2720">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="c3884-2721">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c3884-2721">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2722">Appservice</span></span>

* <span data-ttu-id="c3884-2723">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="c3884-2723">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="c3884-2724">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c3884-2724">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="c3884-2725">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c3884-2725">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="c3884-2726">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="c3884-2726">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="c3884-2727">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="c3884-2727">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="c3884-2728">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="c3884-2728">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2729">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2729">Batch</span></span>

* <span data-ttu-id="c3884-2730">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="c3884-2730">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-2731">Batchai</span><span class="sxs-lookup"><span data-stu-id="c3884-2731">Batchai</span></span>

* <span data-ttu-id="c3884-2732">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2732">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="c3884-2733">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2733">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="c3884-2734">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="c3884-2734">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="c3884-2735">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2735">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="c3884-2736">Cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-2736">Cloud</span></span>

* <span data-ttu-id="c3884-2737">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="c3884-2737">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2738">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2738">Container</span></span>

* <span data-ttu-id="c3884-2739">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="c3884-2739">Added support to open multiple ports</span></span>
* <span data-ttu-id="c3884-2740">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c3884-2740">Added container group restart policy</span></span>
* <span data-ttu-id="c3884-2741">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="c3884-2741">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="c3884-2742">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="c3884-2742">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c3884-2743">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-2743">Data Lake Analytics</span></span>

* <span data-ttu-id="c3884-2744">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c3884-2744">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c3884-2745">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-2745">Data Lake Store</span></span>

* <span data-ttu-id="c3884-2746">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c3884-2746">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2747">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2747">Extension</span></span>

* <span data-ttu-id="c3884-2748">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="c3884-2748">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="c3884-2749">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="c3884-2749">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-2750">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-2750">IoT</span></span>

* <span data-ttu-id="c3884-2751">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="c3884-2751">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2752">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2752">Monitor</span></span>

* <span data-ttu-id="c3884-2753">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="c3884-2753">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2754">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2754">Network</span></span>

* <span data-ttu-id="c3884-2755">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="c3884-2755">Added support for CAA DNS records</span></span>
* <span data-ttu-id="c3884-2756">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2756">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="c3884-2757">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c3884-2757">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="c3884-2758">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c3884-2758">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="c3884-2759">Réservations</span><span class="sxs-lookup"><span data-stu-id="c3884-2759">Reservations</span></span>

* <span data-ttu-id="c3884-2760">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2760">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2761">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2761">Resource</span></span>

* <span data-ttu-id="c3884-2762">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-2762">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2763">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2763">SQL</span></span>

* <span data-ttu-id="c3884-2764">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2764">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2765">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2765">Storage</span></span>

* <span data-ttu-id="c3884-2766">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-2766">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="c3884-2767">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="c3884-2767">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="c3884-2768">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="c3884-2768">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="c3884-2769">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="c3884-2769">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="c3884-2770">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2770">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="c3884-2771">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="c3884-2771">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="c3884-2772">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2772">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2773">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2773">VM</span></span>

* <span data-ttu-id="c3884-2774">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="c3884-2774">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="c3884-2775">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="c3884-2775">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="c3884-2776">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="c3884-2776">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="c3884-2777">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="c3884-2777">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="c3884-2778">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c3884-2778">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c3884-2779">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2779">October 24, 2017</span></span>

<span data-ttu-id="c3884-2780">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c3884-2780">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2781">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2781">Core</span></span>

* <span data-ttu-id="c3884-2782">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c3884-2782">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-2783">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-2783">ACR</span></span>

* <span data-ttu-id="c3884-2784">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c3884-2784">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c3884-2785">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="c3884-2785">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c3884-2786">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="c3884-2786">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2787">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2787">ACS</span></span>

* <span data-ttu-id="c3884-2788">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="c3884-2788">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c3884-2789">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c3884-2789">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2790">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2790">Appservice</span></span>

* <span data-ttu-id="c3884-2791">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="c3884-2791">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c3884-2792">Composant</span><span class="sxs-lookup"><span data-stu-id="c3884-2792">Component</span></span>

* <span data-ttu-id="c3884-2793">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="c3884-2793">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-2794">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-2794">Monitor</span></span>

* <span data-ttu-id="c3884-2795">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="c3884-2795">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2796">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2796">Resource</span></span>

* <span data-ttu-id="c3884-2797">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c3884-2797">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c3884-2798">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="c3884-2798">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2799">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2799">VM</span></span>

* <span data-ttu-id="c3884-2800">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2800">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c3884-2801">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2801">October 9, 2017</span></span>

<span data-ttu-id="c3884-2802">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c3884-2802">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2803">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2803">Core</span></span>

* <span data-ttu-id="c3884-2804">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c3884-2804">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2805">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2805">Appservice</span></span>

* <span data-ttu-id="c3884-2806">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2806">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2807">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2807">Batch</span></span>

* <span data-ttu-id="c3884-2808">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-2808">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c3884-2809">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="c3884-2809">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c3884-2810">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2810">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c3884-2811">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="c3884-2811">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c3884-2812">Batchai</span><span class="sxs-lookup"><span data-stu-id="c3884-2812">Batchai</span></span>

* <span data-ttu-id="c3884-2813">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="c3884-2813">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-2814">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-2814">Keyvault</span></span>

* <span data-ttu-id="c3884-2815">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c3884-2815">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c3884-2816">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c3884-2816">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c3884-2817">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2817">Network</span></span>

* <span data-ttu-id="c3884-2818">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="c3884-2818">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c3884-2819">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c3884-2819">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2820">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2820">Resource</span></span>

* <span data-ttu-id="c3884-2821">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="c3884-2821">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c3884-2822">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-2822">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c3884-2823">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="c3884-2823">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c3884-2824">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-2824">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2825">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2825">Sql</span></span>

* <span data-ttu-id="c3884-2826">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="c3884-2826">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c3884-2827">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="c3884-2827">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c3884-2828">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="c3884-2828">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2829">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2829">Storage</span></span>

* <span data-ttu-id="c3884-2830">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="c3884-2830">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2831">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2831">Vm</span></span>

* <span data-ttu-id="c3884-2832">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="c3884-2832">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c3884-2833">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2833">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c3884-2834">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c3884-2834">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c3884-2835">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2835">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c3884-2836">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2836">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c3884-2837">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2837">September 22, 2017</span></span>

<span data-ttu-id="c3884-2838">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c3884-2838">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2839">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2839">Resource</span></span>

* <span data-ttu-id="c3884-2840">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="c3884-2840">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c3884-2841">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="c3884-2841">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c3884-2842">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2842">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c3884-2843">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c3884-2843">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2844">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2844">Network</span></span>

* <span data-ttu-id="c3884-2845">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c3884-2845">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c3884-2846">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="c3884-2846">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c3884-2847">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="c3884-2847">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c3884-2848">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2848">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c3884-2849">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2849">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c3884-2850">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2850">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c3884-2851">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2851">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2852">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2852">Storage</span></span>

* <span data-ttu-id="c3884-2853">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c3884-2853">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c3884-2854">Événement</span><span class="sxs-lookup"><span data-stu-id="c3884-2854">Eventgrid</span></span>

* <span data-ttu-id="c3884-2855">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="c3884-2855">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2856">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2856">SQL</span></span>

* <span data-ttu-id="c3884-2857">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="c3884-2857">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c3884-2858">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="c3884-2858">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c3884-2859">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2859">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-2860">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-2860">Keyvault</span></span>

* <span data-ttu-id="c3884-2861">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="c3884-2861">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2862">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2862">VM</span></span>

* <span data-ttu-id="c3884-2863">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2863">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c3884-2864">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="c3884-2864">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c3884-2865">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2865">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c3884-2866">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c3884-2866">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c3884-2867">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c3884-2867">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c3884-2868">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c3884-2868">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2869">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2869">ACS</span></span>

* <span data-ttu-id="c3884-2870">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2870">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2871">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2871">Appservice</span></span>

* <span data-ttu-id="c3884-2872">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2872">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c3884-2873">Backup</span><span class="sxs-lookup"><span data-stu-id="c3884-2873">Backup</span></span>

* <span data-ttu-id="c3884-2874">Préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2874">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c3884-2875">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2875">September 11, 2017</span></span>

<span data-ttu-id="c3884-2876">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c3884-2876">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c3884-2877">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-2877">Core</span></span>

* <span data-ttu-id="c3884-2878">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="c3884-2878">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c3884-2879">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="c3884-2879">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2880">Acs</span><span class="sxs-lookup"><span data-stu-id="c3884-2880">Acs</span></span>

* <span data-ttu-id="c3884-2881">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c3884-2881">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c3884-2882">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="c3884-2882">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2883">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2883">Appservice</span></span>

* <span data-ttu-id="c3884-2884">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="c3884-2884">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-2885">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-2885">CDN</span></span>

* <span data-ttu-id="c3884-2886">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2886">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="c3884-2887">Extension</span><span class="sxs-lookup"><span data-stu-id="c3884-2887">Extension</span></span>

* <span data-ttu-id="c3884-2888">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2888">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-2889">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-2889">Keyvault</span></span>

* <span data-ttu-id="c3884-2890">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-2890">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2891">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2891">Network</span></span>

* <span data-ttu-id="c3884-2892">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c3884-2892">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c3884-2893">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2893">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c3884-2894">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2894">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c3884-2895">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2895">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c3884-2896">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2896">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-2897">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-2897">Resource</span></span>

* <span data-ttu-id="c3884-2898">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2898">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c3884-2899">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2899">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c3884-2900">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="c3884-2900">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c3884-2901">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="c3884-2901">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-2902">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-2902">SQL</span></span>

* <span data-ttu-id="c3884-2903">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-2903">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2904">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2904">VM</span></span>

* <span data-ttu-id="c3884-2905">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="c3884-2905">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c3884-2906">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="c3884-2906">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c3884-2907">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2907">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c3884-2908">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="c3884-2908">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c3884-2909">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="c3884-2909">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c3884-2910">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2910">August 31, 2017</span></span>

<span data-ttu-id="c3884-2911">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c3884-2911">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-2912">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-2912">Keyvault</span></span>

* <span data-ttu-id="c3884-2913">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="c3884-2913">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c3884-2914">Sf</span><span class="sxs-lookup"><span data-stu-id="c3884-2914">Sf</span></span>

* <span data-ttu-id="c3884-2915">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c3884-2915">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2916">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2916">Storage</span></span>

* <span data-ttu-id="c3884-2917">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="c3884-2917">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c3884-2918">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="c3884-2918">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c3884-2919">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2919">August 28, 2017</span></span>

<span data-ttu-id="c3884-2920">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c3884-2920">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c3884-2921">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2921">CLI</span></span>

* <span data-ttu-id="c3884-2922">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="c3884-2922">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2923">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2923">ACS</span></span>

* <span data-ttu-id="c3884-2924">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c3884-2924">Corrected preview regions</span></span>
* <span data-ttu-id="c3884-2925">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-2925">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="c3884-2926">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2926">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2927">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2927">Appservice</span></span>

* <span data-ttu-id="c3884-2928">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2928">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c3884-2929">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-2929">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c3884-2930">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c3884-2930">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c3884-2931">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="c3884-2931">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c3884-2932">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-2932">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-2933">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-2933">IoT</span></span>

* <span data-ttu-id="c3884-2934">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="c3884-2934">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2935">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2935">Network</span></span>

* <span data-ttu-id="c3884-2936">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c3884-2936">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c3884-2937">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2937">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c3884-2938">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c3884-2938">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c3884-2939">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2939">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c3884-2940">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2940">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2941">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2941">Profile</span></span>

* <span data-ttu-id="c3884-2942">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2942">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c3884-2943">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c3884-2943">Service Fabric</span></span>

* <span data-ttu-id="c3884-2944">Préversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2944">Preview release</span></span>
* <span data-ttu-id="c3884-2945">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="c3884-2945">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c3884-2946">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="c3884-2946">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c3884-2947">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="c3884-2947">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2948">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2948">Storage</span></span>

* <span data-ttu-id="c3884-2949">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="c3884-2949">Enabled setting blob tier</span></span>
* <span data-ttu-id="c3884-2950">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="c3884-2950">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c3884-2951">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c3884-2951">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="c3884-2952">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="c3884-2952">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c3884-2953">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="c3884-2953">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c3884-2954">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="c3884-2954">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2955">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2955">VM</span></span>

* <span data-ttu-id="c3884-2956">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c3884-2956">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c3884-2957">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c3884-2957">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="c3884-2958">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2958">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="c3884-2959">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="c3884-2959">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c3884-2960">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="c3884-2960">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c3884-2961">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c3884-2961">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c3884-2962">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2962">August 15, 2017</span></span>

<span data-ttu-id="c3884-2963">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c3884-2963">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2964">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2964">ACS</span></span>

* <span data-ttu-id="c3884-2965">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="c3884-2965">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-2966">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-2966">Appservice</span></span>

* <span data-ttu-id="c3884-2967">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="c3884-2967">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c3884-2968">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c3884-2968">Event Grid</span></span>

* <span data-ttu-id="c3884-2969">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c3884-2969">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c3884-2970">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-2970">August 11, 2017</span></span>

<span data-ttu-id="c3884-2971">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c3884-2971">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-2972">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-2972">ACS</span></span>

* <span data-ttu-id="c3884-2973">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c3884-2973">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-2974">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-2974">Batch</span></span>

* <span data-ttu-id="c3884-2975">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c3884-2975">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c3884-2976">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2976">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c3884-2977">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="c3884-2977">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c3884-2978">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="c3884-2978">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c3884-2979">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="c3884-2979">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c3884-2980">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="c3884-2980">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c3884-2981">Composant</span><span class="sxs-lookup"><span data-stu-id="c3884-2981">Component</span></span>

* <span data-ttu-id="c3884-2982">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="c3884-2982">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c3884-2983">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-2983">Container</span></span>

* <span data-ttu-id="c3884-2984">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="c3884-2984">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c3884-2985">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-2985">Data Lake Store</span></span>

* <span data-ttu-id="c3884-2986">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="c3884-2986">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c3884-2987">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c3884-2987">Event Grid</span></span>

* <span data-ttu-id="c3884-2988">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c3884-2988">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c3884-2989">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-2989">Network</span></span>

* <span data-ttu-id="c3884-2990">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="c3884-2990">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c3884-2991">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c3884-2991">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c3884-2992">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="c3884-2992">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c3884-2993">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c3884-2993">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-2994">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-2994">Profile</span></span>

* <span data-ttu-id="c3884-2995">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="c3884-2995">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-2996">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-2996">Storage</span></span>

* <span data-ttu-id="c3884-2997">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c3884-2997">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-2998">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-2998">VM</span></span>

* <span data-ttu-id="c3884-2999">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="c3884-2999">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c3884-3000">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="c3884-3000">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c3884-3001">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="c3884-3001">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c3884-3002">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="c3884-3002">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c3884-3003">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="c3884-3003">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c3884-3004">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-3004">July 28, 2017</span></span>

<span data-ttu-id="c3884-3005">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c3884-3005">Version 2.0.12</span></span>

* <span data-ttu-id="c3884-3006">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="c3884-3006">Added container commands</span></span>
* <span data-ttu-id="c3884-3007">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="c3884-3007">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c3884-3008">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-3008">Core</span></span>

* <span data-ttu-id="c3884-3009">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="c3884-3009">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c3884-3010">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="c3884-3010">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c3884-3011">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c3884-3011">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c3884-3012">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c3884-3012">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c3884-3013">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="c3884-3013">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c3884-3014">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="c3884-3014">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c3884-3015">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="c3884-3015">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c3884-3016">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c3884-3016">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c3884-3017">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="c3884-3017">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c3884-3018">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c3884-3018">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c3884-3019">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="c3884-3019">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c3884-3020">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="c3884-3020">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c3884-3021">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-3021">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c3884-3022">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c3884-3022">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c3884-3023">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c3884-3023">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c3884-3024">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c3884-3024">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c3884-3025">ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-3025">ACR</span></span>

* <span data-ttu-id="c3884-3026">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c3884-3026">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c3884-3027">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c3884-3027">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c3884-3028">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="c3884-3028">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c3884-3029">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="c3884-3029">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c3884-3030">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="c3884-3030">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c3884-3031">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="c3884-3031">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-3032">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-3032">ACS</span></span>

* <span data-ttu-id="c3884-3033">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c3884-3033">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-3034">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-3034">Appservice</span></span>

* <span data-ttu-id="c3884-3035">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="c3884-3035">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c3884-3036">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="c3884-3036">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c3884-3037">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c3884-3037">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c3884-3038">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="c3884-3038">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c3884-3039">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="c3884-3039">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c3884-3040">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c3884-3040">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c3884-3041">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="c3884-3041">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c3884-3042">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="c3884-3042">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c3884-3043">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="c3884-3043">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c3884-3044">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c3884-3044">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c3884-3045">Batch</span><span class="sxs-lookup"><span data-stu-id="c3884-3045">Batch</span></span>

* <span data-ttu-id="c3884-3046">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="c3884-3046">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c3884-3047">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c3884-3047">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c3884-3048">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c3884-3048">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c3884-3049">CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-3049">CDN</span></span>

* <span data-ttu-id="c3884-3050">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c3884-3050">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="c3884-3051">Cloud</span><span class="sxs-lookup"><span data-stu-id="c3884-3051">Cloud</span></span>

* <span data-ttu-id="c3884-3052">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="c3884-3052">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c3884-3053">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c3884-3053">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c3884-3054">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="c3884-3054">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c3884-3055">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="c3884-3055">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c3884-3056">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c3884-3056">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-3057">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-3057">CosmosDB</span></span>

* <span data-ttu-id="c3884-3058">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="c3884-3058">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c3884-3059">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="c3884-3059">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c3884-3060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-3060">Data Lake Analytics</span></span>

* <span data-ttu-id="c3884-3061">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c3884-3061">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c3884-3062">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c3884-3062">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c3884-3063">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c3884-3063">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c3884-3064">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-3064">Data Lake Store</span></span>

* <span data-ttu-id="c3884-3065">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3065">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c3884-3066">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="c3884-3066">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c3884-3067">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c3884-3067">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c3884-3068">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-3068">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c3884-3069">Interactive</span><span class="sxs-lookup"><span data-stu-id="c3884-3069">Interactive</span></span>

* <span data-ttu-id="c3884-3070">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="c3884-3070">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c3884-3071">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="c3884-3071">Increased test coverage</span></span>
* <span data-ttu-id="c3884-3072">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="c3884-3072">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c3884-3073">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c3884-3073">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c3884-3074">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="c3884-3074">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c3884-3075">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="c3884-3075">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c3884-3076">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="c3884-3076">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c3884-3077">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="c3884-3077">Added `--progress` flag</span></span>
* <span data-ttu-id="c3884-3078">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="c3884-3078">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c3884-3079">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="c3884-3079">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c3884-3080">IoT</span><span class="sxs-lookup"><span data-stu-id="c3884-3080">IoT</span></span>

* <span data-ttu-id="c3884-3081">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="c3884-3081">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c3884-3082">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c3884-3082">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c3884-3083">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c3884-3083">Key vault</span></span>

* <span data-ttu-id="c3884-3084">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="c3884-3084">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c3884-3085">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c3884-3085">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c3884-3086">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c3884-3086">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c3884-3087">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c3884-3087">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c3884-3088">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c3884-3088">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c3884-3089">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="c3884-3089">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c3884-3090">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c3884-3090">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c3884-3091">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c3884-3091">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c3884-3092">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3092">Lab</span></span>

* <span data-ttu-id="c3884-3093">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c3884-3093">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c3884-3094">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c3884-3094">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-3095">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-3095">Monitor</span></span>

* <span data-ttu-id="c3884-3096">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="c3884-3096">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c3884-3097">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c3884-3097">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c3884-3098">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c3884-3098">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c3884-3099">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c3884-3099">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c3884-3100">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c3884-3100">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c3884-3101">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c3884-3101">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c3884-3102">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="c3884-3102">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c3884-3103">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="c3884-3103">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c3884-3104">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c3884-3104">`location` no longer required</span></span>
  * <span data-ttu-id="c3884-3105">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="c3884-3105">Add name and ID support for target</span></span>
  * <span data-ttu-id="c3884-3106">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-3106">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c3884-3107">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c3884-3107">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c3884-3108">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="c3884-3108">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c3884-3109">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="c3884-3109">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c3884-3110">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c3884-3110">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c3884-3111">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3111">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c3884-3112">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-3112">Network</span></span>

* <span data-ttu-id="c3884-3113">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c3884-3113">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c3884-3114">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3114">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c3884-3115">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="c3884-3115">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c3884-3116">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="c3884-3116">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c3884-3117">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3117">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c3884-3118">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c3884-3118">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c3884-3119">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c3884-3119">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c3884-3120">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c3884-3120">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c3884-3121">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c3884-3121">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c3884-3122">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c3884-3122">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c3884-3123">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3123">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c3884-3124">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c3884-3124">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c3884-3125">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c3884-3125">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c3884-3126">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3126">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c3884-3127">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3127">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c3884-3128">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3128">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c3884-3129">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="c3884-3129">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c3884-3130">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c3884-3130">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c3884-3131">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3131">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c3884-3132">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3132">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c3884-3133">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3133">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c3884-3134">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-3134">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c3884-3135">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c3884-3135">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c3884-3136">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c3884-3136">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c3884-3137">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c3884-3137">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c3884-3138">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c3884-3138">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c3884-3139">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c3884-3139">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-3140">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-3140">Profile</span></span>

* <span data-ttu-id="c3884-3141">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="c3884-3141">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c3884-3142">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c3884-3142">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c3884-3143">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="c3884-3143">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c3884-3144">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="c3884-3144">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c3884-3145">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="c3884-3145">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c3884-3146">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c3884-3146">RDBMS</span></span>

* <span data-ttu-id="c3884-3147">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="c3884-3147">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c3884-3148">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c3884-3148">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c3884-3149">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="c3884-3149">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c3884-3150">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c3884-3150">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-3151">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-3151">Resource</span></span>

* <span data-ttu-id="c3884-3152">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3152">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c3884-3153">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c3884-3153">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c3884-3154">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c3884-3154">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c3884-3155">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="c3884-3155">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c3884-3156">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="c3884-3156">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c3884-3157">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c3884-3157">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c3884-3158">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="c3884-3158">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c3884-3159">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c3884-3159">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c3884-3160">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-3160">Role</span></span>

* <span data-ttu-id="c3884-3161">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c3884-3161">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c3884-3162">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="c3884-3162">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c3884-3163">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="c3884-3163">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c3884-3164">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c3884-3164">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c3884-3165">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c3884-3165">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c3884-3166">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c3884-3166">Service Fabric</span></span>
* <span data-ttu-id="c3884-3167">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="c3884-3167">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c3884-3168">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c3884-3168">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c3884-3169">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c3884-3169">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-3170">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-3170">SQL</span></span>

* <span data-ttu-id="c3884-3171">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="c3884-3171">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c3884-3172">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c3884-3172">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c3884-3173">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c3884-3173">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-3174">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-3174">Storage</span></span>

* <span data-ttu-id="c3884-3175">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c3884-3175">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c3884-3176">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="c3884-3176">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c3884-3177">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="c3884-3177">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c3884-3178">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c3884-3178">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="c3884-3179">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="c3884-3179">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="c3884-3180">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c3884-3180">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-3181">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-3181">VM</span></span>

* <span data-ttu-id="c3884-3182">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-3182">Support configuring nsg</span></span>
* <span data-ttu-id="c3884-3183">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="c3884-3183">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c3884-3184">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="c3884-3184">Support managed service identities</span></span>
* <span data-ttu-id="c3884-3185">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="c3884-3185">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="c3884-3186">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="c3884-3186">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c3884-3187">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-3187">May 10, 2017</span></span>

<span data-ttu-id="c3884-3188">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c3884-3188">Version 2.0.6</span></span>

* <span data-ttu-id="c3884-3189">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c3884-3189">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c3884-3190">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c3884-3190">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c3884-3191">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-3191">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="c3884-3192">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c3884-3192">Include Cognitive Services module</span></span>
* <span data-ttu-id="c3884-3193">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c3884-3193">Include Service Fabric module</span></span>
* <span data-ttu-id="c3884-3194">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="c3884-3194">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="c3884-3195">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="c3884-3195">Add support for CDN commands</span></span>
* <span data-ttu-id="c3884-3196">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="c3884-3196">Remove Container module</span></span>
* <span data-ttu-id="c3884-3197">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c3884-3197">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c3884-3198">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c3884-3198">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c3884-3199">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-3199">Core</span></span>

* <span data-ttu-id="c3884-3200">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="c3884-3200">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="c3884-3201">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c3884-3201">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c3884-3202">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c3884-3202">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c3884-3203">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c3884-3203">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c3884-3204">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c3884-3204">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c3884-3205">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c3884-3205">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c3884-3206">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c3884-3206">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c3884-3207">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c3884-3207">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c3884-3208">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c3884-3208">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c3884-3209">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="c3884-3209">core: Improved performance</span></span>
* <span data-ttu-id="c3884-3210">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c3884-3210">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c3884-3211">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="c3884-3211">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-3212">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-3212">ACS</span></span>

* <span data-ttu-id="c3884-3213">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c3884-3213">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c3884-3214">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="c3884-3214">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c3884-3215">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="c3884-3215">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c3884-3216">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c3884-3216">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-3217">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-3217">AppService</span></span>

* <span data-ttu-id="c3884-3218">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c3884-3218">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c3884-3219">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="c3884-3219">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c3884-3220">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="c3884-3220">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c3884-3221">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="c3884-3221">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c3884-3222">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="c3884-3222">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c3884-3223">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c3884-3223">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c3884-3224">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="c3884-3224">support slot swap with preview</span></span>
* <span data-ttu-id="c3884-3225">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c3884-3225">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c3884-3226">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c3884-3226">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c3884-3227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c3884-3227">CosmosDB</span></span>

* <span data-ttu-id="c3884-3228">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c3884-3228">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="c3884-3229">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="c3884-3229">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c3884-3230">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="c3884-3230">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c3884-3231">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c3884-3231">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c3884-3232">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-3232">Data Lake Analytics</span></span>

* <span data-ttu-id="c3884-3233">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="c3884-3233">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="c3884-3234">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="c3884-3234">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c3884-3235">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c3884-3235">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c3884-3236">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="c3884-3236">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c3884-3237">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="c3884-3237">Table</span></span>
  * <span data-ttu-id="c3884-3238">Fonction table</span><span class="sxs-lookup"><span data-stu-id="c3884-3238">Table valued function</span></span>
  * <span data-ttu-id="c3884-3239">Affichage</span><span class="sxs-lookup"><span data-stu-id="c3884-3239">View</span></span>
  * <span data-ttu-id="c3884-3240">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="c3884-3240">Table Statistics.</span></span> <span data-ttu-id="c3884-3241">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="c3884-3241">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c3884-3242">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-3242">Data Lake Store</span></span>

* <span data-ttu-id="c3884-3243">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="c3884-3243">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="c3884-3244">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c3884-3244">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c3884-3245">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="c3884-3245">missed help for access show.</span></span> <span data-ttu-id="c3884-3246">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="c3884-3246">adding it.</span></span> <span data-ttu-id="c3884-3247">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c3884-3247">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c3884-3248">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c3884-3248">Find</span></span>

* <span data-ttu-id="c3884-3249">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="c3884-3249">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c3884-3250">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c3884-3250">KeyVault</span></span>

* <span data-ttu-id="c3884-3251">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="c3884-3251">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c3884-3252">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c3884-3252">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="c3884-3253">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="c3884-3253">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c3884-3254">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="c3884-3254">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="c3884-3255">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c3884-3255">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c3884-3256">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3256">Lab</span></span>

* <span data-ttu-id="c3884-3257">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3257">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="c3884-3258">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3258">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="c3884-3259">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3259">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="c3884-3260">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3260">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="c3884-3261">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="c3884-3261">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="c3884-3262">Moniteur</span><span class="sxs-lookup"><span data-stu-id="c3884-3262">Monitor</span></span>

* <span data-ttu-id="c3884-3263">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c3884-3263">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c3884-3264">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c3884-3264">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c3884-3265">Réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-3265">Network</span></span>

* <span data-ttu-id="c3884-3266">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="c3884-3266">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="c3884-3267">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3267">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="c3884-3268">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c3884-3268">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="c3884-3269">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c3884-3269">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="c3884-3270">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="c3884-3270">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="c3884-3271">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c3884-3271">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="c3884-3272">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c3884-3272">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="c3884-3273">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c3884-3273">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="c3884-3274">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="c3884-3274">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="c3884-3275">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="c3884-3275">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c3884-3276">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="c3884-3276">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="c3884-3277">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3277">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="c3884-3278">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-3278">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="c3884-3279">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="c3884-3279">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="c3884-3280">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c3884-3280">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="c3884-3281">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="c3884-3281">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="c3884-3282">Profil</span><span class="sxs-lookup"><span data-stu-id="c3884-3282">Profile</span></span>

* <span data-ttu-id="c3884-3283">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c3884-3283">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c3884-3284">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c3884-3284">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c3884-3285">Redis</span><span class="sxs-lookup"><span data-stu-id="c3884-3285">Redis</span></span>

* <span data-ttu-id="c3884-3286">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="c3884-3286">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c3884-3287">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="c3884-3287">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="c3884-3288">Ressource</span><span class="sxs-lookup"><span data-stu-id="c3884-3288">Resource</span></span>

* <span data-ttu-id="c3884-3289">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c3884-3289">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c3884-3290">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c3884-3290">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c3884-3291">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c3884-3291">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c3884-3292">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="c3884-3292">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c3884-3293">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c3884-3293">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c3884-3294">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="c3884-3294">Add docs for az lock update.</span></span> <span data-ttu-id="c3884-3295">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c3884-3295">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c3884-3296">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c3884-3296">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c3884-3297">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c3884-3297">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c3884-3298">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c3884-3298">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c3884-3299">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c3884-3299">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c3884-3300">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c3884-3300">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c3884-3301">Role</span><span class="sxs-lookup"><span data-stu-id="c3884-3301">Role</span></span>

* <span data-ttu-id="c3884-3302">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c3884-3302">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c3884-3303">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c3884-3303">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c3884-3304">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c3884-3304">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c3884-3305">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="c3884-3305">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c3884-3306">SQL</span><span class="sxs-lookup"><span data-stu-id="c3884-3306">SQL</span></span>

* <span data-ttu-id="c3884-3307">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="c3884-3307">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="c3884-3308">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c3884-3308">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c3884-3309">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-3309">Storage</span></span>

* <span data-ttu-id="c3884-3310">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="c3884-3310">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="c3884-3311">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c3884-3311">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c3884-3312">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="c3884-3312">Add support for large block blob upload</span></span>
* <span data-ttu-id="c3884-3313">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="c3884-3313">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-3314">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-3314">VM</span></span>

* <span data-ttu-id="c3884-3315">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="c3884-3315">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c3884-3316">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="c3884-3316">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c3884-3317">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c3884-3317">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c3884-3318">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c3884-3318">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c3884-3319">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="c3884-3319">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c3884-3320">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="c3884-3320">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c3884-3321">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c3884-3321">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c3884-3322">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-3322">April 3, 2017</span></span>

<span data-ttu-id="c3884-3323">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c3884-3323">Version 2.0.2</span></span>

<span data-ttu-id="c3884-3324">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="c3884-3324">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="c3884-3325">Core</span><span class="sxs-lookup"><span data-stu-id="c3884-3325">Core</span></span>

* <span data-ttu-id="c3884-3326">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-3326">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="c3884-3327">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c3884-3327">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c3884-3328">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c3884-3328">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c3884-3329">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c3884-3329">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c3884-3330">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c3884-3330">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c3884-3331">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="c3884-3331">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c3884-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c3884-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c3884-3333">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="c3884-3333">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c3884-3334">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="c3884-3334">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="c3884-3335">ACS</span><span class="sxs-lookup"><span data-stu-id="c3884-3335">ACS</span></span>

* <span data-ttu-id="c3884-3336">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c3884-3336">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c3884-3337">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="c3884-3337">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c3884-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c3884-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c3884-3339">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="c3884-3339">Add support for windows clusters.</span></span> <span data-ttu-id="c3884-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c3884-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c3884-3341">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="c3884-3341">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c3884-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c3884-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="c3884-3343">AppService</span><span class="sxs-lookup"><span data-stu-id="c3884-3343">AppService</span></span>

* <span data-ttu-id="c3884-3344">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c3884-3344">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c3884-3345">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c3884-3345">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c3884-3346">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c3884-3346">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c3884-3347">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c3884-3347">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="c3884-3348">DataLake</span><span class="sxs-lookup"><span data-stu-id="c3884-3348">DataLake</span></span>

* <span data-ttu-id="c3884-3349">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c3884-3349">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="c3884-3350">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c3884-3350">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="c3884-3351">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c3884-3351">DocuemntDB</span></span>

* <span data-ttu-id="c3884-3352">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c3884-3352">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c3884-3353">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c3884-3353">VM</span></span>

* <span data-ttu-id="c3884-3354">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c3884-3354">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c3884-3355">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c3884-3355">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c3884-3356">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c3884-3356">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c3884-3357">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c3884-3357">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c3884-3358">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c3884-3358">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c3884-3359">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="c3884-3359">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="c3884-3360">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c3884-3360">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c3884-3361">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="c3884-3361">February 27, 2017</span></span>

<span data-ttu-id="c3884-3362">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c3884-3362">Version 2.0.0</span></span>

<span data-ttu-id="c3884-3363">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="c3884-3363">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="c3884-3364">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c3884-3364">Container Service (acs)</span></span>
- <span data-ttu-id="c3884-3365">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="c3884-3365">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c3884-3366">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="c3884-3366">Networking</span></span>
- <span data-ttu-id="c3884-3367">Stockage</span><span class="sxs-lookup"><span data-stu-id="c3884-3367">Storage</span></span>

<span data-ttu-id="c3884-3368">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c3884-3368">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="c3884-3369">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c3884-3369">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="c3884-3370">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="c3884-3370">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="c3884-3371">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="c3884-3371">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="c3884-3372">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c3884-3372">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="c3884-3373">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="c3884-3373">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c3884-3374">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c3884-3374">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c3884-3375">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c3884-3375">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="c3884-3376">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c3884-3376">Provide feedback from the command line with the `az feedback` command</span></span>

