---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/05/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 727f9960ce60861bbe20a649606b807efb8d9cbc
ms.sourcegitcommit: f30b67f48b956bdc281f1a5fae96e10120ee3bba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/12/2019
ms.locfileid: "70937095"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="9fb94-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9fb94-103">Azure CLI release notes</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="9fb94-104">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-104">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-105">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-105">ACR</span></span>

* <span data-ttu-id="9fb94-106">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="9fb94-106">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="9fb94-107">AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-107">AKS</span></span>

* <span data-ttu-id="9fb94-108">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-108">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="9fb94-109">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-109">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="9fb94-110">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-110">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="9fb94-111">ARM</span><span class="sxs-lookup"><span data-stu-id="9fb94-111">ARM</span></span>

* <span data-ttu-id="9fb94-112">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="9fb94-112">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-113">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-113">Batch</span></span>

* <span data-ttu-id="9fb94-114">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-114">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="9fb94-115">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="9fb94-115">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="9fb94-116">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="9fb94-116">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="9fb94-117">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="9fb94-117">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="9fb94-118">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="9fb94-118">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="9fb94-119">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="9fb94-119">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="9fb94-120">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="9fb94-120">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-121">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-121">HDInsight</span></span>

* <span data-ttu-id="9fb94-122">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="9fb94-122">GA release</span></span>
* <span data-ttu-id="9fb94-123">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="9fb94-123">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fb94-124">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fb94-124">Key Vault</span></span>

* <span data-ttu-id="9fb94-125">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-125">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="9fb94-126">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-126">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-127">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-127">Network</span></span>

* <span data-ttu-id="9fb94-128">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="9fb94-128">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="9fb94-129">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-129">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="9fb94-130">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="9fb94-130">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="9fb94-131">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-131">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="9fb94-132">Stratégie</span><span class="sxs-lookup"><span data-stu-id="9fb94-132">Policy</span></span>

* <span data-ttu-id="9fb94-133">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="9fb94-133">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="9fb94-134">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-134">August 27, 2019</span></span>

<span data-ttu-id="9fb94-135">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="9fb94-135">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-136">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-136">ACR</span></span>

* <span data-ttu-id="9fb94-137">[CHANGEMENT CASSANT] Suppression du support pour la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="9fb94-137">[BREAKING CHNAGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="9fb94-138">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="9fb94-138">API Management</span></span>

* <span data-ttu-id="9fb94-139">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="9fb94-139">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-140">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-140">AppService</span></span>

* <span data-ttu-id="9fb94-141">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="9fb94-141">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="9fb94-142">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="9fb94-142">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-143">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-143">Keyvault</span></span>

* <span data-ttu-id="9fb94-144">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="9fb94-144">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-145">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-145">Network</span></span>

* <span data-ttu-id="9fb94-146">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="9fb94-146">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="9fb94-147">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="9fb94-147">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="9fb94-148">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="9fb94-148">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="9fb94-149">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-149">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="9fb94-150">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fb94-150">RBAC</span></span>

* <span data-ttu-id="9fb94-151">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="9fb94-151">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fb94-152">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-152">ServiceFabric</span></span>

* <span data-ttu-id="9fb94-153">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="9fb94-153">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="9fb94-154">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fb94-154">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="9fb94-155">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="9fb94-155">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="9fb94-156">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="9fb94-156">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="9fb94-157">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-157">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="9fb94-158">SignalR</span><span class="sxs-lookup"><span data-stu-id="9fb94-158">SignalR</span></span>

* <span data-ttu-id="9fb94-159">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-159">Added new commands:</span></span>
  * <span data-ttu-id="9fb94-160">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="9fb94-160">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="9fb94-161">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="9fb94-161">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="9fb94-162">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="9fb94-162">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="9fb94-163">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-163">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-164">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-164">Storage</span></span>

* <span data-ttu-id="9fb94-165">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="9fb94-165">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="9fb94-166">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-166">August 13, 2019</span></span>

<span data-ttu-id="9fb94-167">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="9fb94-167">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-168">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-168">AppService</span></span>

* <span data-ttu-id="9fb94-169">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="9fb94-169">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-170">BotService</span><span class="sxs-lookup"><span data-stu-id="9fb94-170">BotService</span></span>

* <span data-ttu-id="9fb94-171">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="9fb94-171">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="9fb94-172">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9fb94-172">CognitiveServices</span></span>

* <span data-ttu-id="9fb94-173">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-173">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fb94-174">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-174">Cosmos DB</span></span>

* <span data-ttu-id="9fb94-175">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="9fb94-175">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="9fb94-176">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-176">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-177">HDInsight</span></span>

<span data-ttu-id="9fb94-178">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="9fb94-178">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="9fb94-179">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-179">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="9fb94-180">Renommage de `--storage-default-container` en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="9fb94-180">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="9fb94-181">Renommage de `--storage-default-filesystem` en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="9fb94-181">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="9fb94-182">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="9fb94-182">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="9fb94-183">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-183">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="9fb94-184">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-184">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="9fb94-185">Renommage de `--application-type` en `--type`</span><span class="sxs-lookup"><span data-stu-id="9fb94-185">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="9fb94-186">Renommage de `--marketplace-identifier` en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="9fb94-186">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="9fb94-187">Renommage de `--https-endpoint-access-mode` en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="9fb94-187">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="9fb94-188">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="9fb94-188">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="9fb94-189">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-189">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="9fb94-190">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="9fb94-190">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="9fb94-191">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="9fb94-191">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="9fb94-192">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-192">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="9fb94-193">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="9fb94-193">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="9fb94-194">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="9fb94-194">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="9fb94-195">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="9fb94-195">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="9fb94-196">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-196">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="9fb94-197">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="9fb94-197">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="9fb94-198">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="9fb94-198">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="9fb94-199">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-199">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="9fb94-200">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="9fb94-200">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="9fb94-201">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-201">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-202">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-202">Interactive</span></span>

* <span data-ttu-id="9fb94-203">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="9fb94-203">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="9fb94-204">kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fb94-204">Kubernetes</span></span>

* <span data-ttu-id="9fb94-205">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="9fb94-205">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-206">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-206">Network</span></span>

* <span data-ttu-id="9fb94-207">Ajout de l’argument `--yes` `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-207">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-208">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-208">Profile</span></span>

* <span data-ttu-id="9fb94-209">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="9fb94-209">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fb94-210">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-210">ServiceFabric</span></span>

* <span data-ttu-id="9fb94-211">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="9fb94-211">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="9fb94-212">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="9fb94-212">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-213">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-213">Storage</span></span>

* <span data-ttu-id="9fb94-214">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-214">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="9fb94-215">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-215">July 30, 2019</span></span>

<span data-ttu-id="9fb94-216">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="9fb94-216">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-217">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-217">ACR</span></span>

* <span data-ttu-id="9fb94-218">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="9fb94-218">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="9fb94-219">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="9fb94-219">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-220">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-220">Appservice</span></span>

* <span data-ttu-id="9fb94-221">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="9fb94-221">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="9fb94-222">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="9fb94-222">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="9fb94-223">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="9fb94-223">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-224">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-224">Network</span></span>

* <span data-ttu-id="9fb94-225">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="9fb94-225">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="9fb94-226">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="9fb94-226">Fixes #9604.</span></span> <span data-ttu-id="9fb94-227">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9fb94-227">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="9fb94-228">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="9fb94-228">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="9fb94-229">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fb94-229">RBAC</span></span>

* <span data-ttu-id="9fb94-230">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-230">Added `user update` command</span></span>
* <span data-ttu-id="9fb94-231">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="9fb94-231">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="9fb94-232">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="9fb94-232">Use replacement argument `--id`</span></span>
* <span data-ttu-id="9fb94-233">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="9fb94-233">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-234">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-234">SQL</span></span>

* <span data-ttu-id="9fb94-235">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="9fb94-235">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-236">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-236">Storage</span></span>

* <span data-ttu-id="9fb94-237">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="9fb94-237">Added `storage remove` command</span></span>
* <span data-ttu-id="9fb94-238">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-238">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-239">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-239">VM</span></span>

* <span data-ttu-id="9fb94-240">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="9fb94-240">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="9fb94-241">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-241">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="9fb94-242">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-242">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="9fb94-243">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="9fb94-243">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="9fb94-244">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-244">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="9fb94-245">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-245">July 16, 2019</span></span>

<span data-ttu-id="9fb94-246">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="9fb94-246">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-247">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-247">Appservice</span></span>

* <span data-ttu-id="9fb94-248">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="9fb94-248">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="9fb94-249">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="9fb94-249">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="9fb94-250">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-250">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-251">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-251">Core</span></span>

* <span data-ttu-id="9fb94-252">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-252">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-253">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-253">Batch</span></span>

* <span data-ttu-id="9fb94-254">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-254">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="9fb94-255">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="9fb94-255">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="9fb94-256">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-256">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="9fb94-257">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-257">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fb94-258">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9fb94-258">Eventhubs</span></span>

* <span data-ttu-id="9fb94-259">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-259">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-260">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-260">RDBMS</span></span>

* <span data-ttu-id="9fb94-261">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="9fb94-261">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="9fb94-262">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-262">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="9fb94-263">Relais</span><span class="sxs-lookup"><span data-stu-id="9fb94-263">Relay</span></span>

* <span data-ttu-id="9fb94-264">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="9fb94-264">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="9fb94-265">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-265">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fb94-266">Servicebus</span><span class="sxs-lookup"><span data-stu-id="9fb94-266">Servicebus</span></span>

* <span data-ttu-id="9fb94-267">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-267">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-268">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-268">Storage</span></span>

* <span data-ttu-id="9fb94-269">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-269">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="9fb94-270">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="9fb94-270">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="9fb94-271">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-271">July 2, 2019</span></span>

<span data-ttu-id="9fb94-272">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="9fb94-272">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-273">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-273">Core</span></span>

* <span data-ttu-id="9fb94-274">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="9fb94-274">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="9fb94-275">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="9fb94-275">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="9fb94-276">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-276">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-277">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-277">ACR</span></span>

* <span data-ttu-id="9fb94-278">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="9fb94-278">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-279">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-279">Appservice</span></span>

* <span data-ttu-id="9fb94-280">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-280">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="9fb94-281">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="9fb94-281">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="9fb94-282">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="9fb94-282">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="9fb94-283">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="9fb94-283">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fb94-284">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-284">Cosmos DB</span></span>

* <span data-ttu-id="9fb94-285">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="9fb94-285">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="9fb94-286">DLS</span><span class="sxs-lookup"><span data-stu-id="9fb94-286">DLS</span></span>

* <span data-ttu-id="9fb94-287">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="9fb94-287">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="9fb94-288">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9fb94-288">Feedback</span></span>

* <span data-ttu-id="9fb94-289">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="9fb94-289">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-290">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-290">HDInsight</span></span>

* <span data-ttu-id="9fb94-291">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="9fb94-291">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="9fb94-292">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-292">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="9fb94-293">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="9fb94-293">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="9fb94-294">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="9fb94-294">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="9fb94-295">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="9fb94-295">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="9fb94-296">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-296">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="9fb94-297">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="9fb94-297">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="9fb94-298">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="9fb94-298">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="9fb94-299">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-299">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="9fb94-300">Services gérés</span><span class="sxs-lookup"><span data-stu-id="9fb94-300">Managed Services</span></span>

* <span data-ttu-id="9fb94-301">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-301">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-302">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-302">Profile</span></span>
* <span data-ttu-id="9fb94-303">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="9fb94-303">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="9fb94-304">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fb94-304">RBAC</span></span>

* <span data-ttu-id="9fb94-305">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9fb94-305">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="9fb94-306">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="9fb94-306">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="9fb94-307">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="9fb94-307">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="9fb94-308">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="9fb94-308">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-309">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-309">RDBMS</span></span>

* <span data-ttu-id="9fb94-310">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-310">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-311">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-311">SQL</span></span>

* <span data-ttu-id="9fb94-312">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-312">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-313">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-313">Storage</span></span>

* <span data-ttu-id="9fb94-314">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9fb94-314">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="9fb94-315">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9fb94-315">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="9fb94-316">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-316">VM</span></span>

* <span data-ttu-id="9fb94-317">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-317">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="9fb94-318">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-318">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="9fb94-319">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="9fb94-319">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="9fb94-320">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="9fb94-320">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="9fb94-321">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-321">June 18, 2019</span></span>

<span data-ttu-id="9fb94-322">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="9fb94-322">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-323">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-323">Core</span></span>

<span data-ttu-id="9fb94-324">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="9fb94-324">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="9fb94-325">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="9fb94-325">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="9fb94-326">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="9fb94-326">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="9fb94-327">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="9fb94-327">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="9fb94-328">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="9fb94-328">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="9fb94-329">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="9fb94-329">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="9fb94-330">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="9fb94-330">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-331">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-331">ACR</span></span>
* <span data-ttu-id="9fb94-332">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="9fb94-332">Added 'acr check-health' command</span></span>
* <span data-ttu-id="9fb94-333">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="9fb94-333">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-334">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-334">ACS</span></span>
* <span data-ttu-id="9fb94-335">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-335">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-336">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-336">AMS</span></span>
* <span data-ttu-id="9fb94-337">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="9fb94-337">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-338">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-338">AppService</span></span>
* <span data-ttu-id="9fb94-339">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="9fb94-339">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="9fb94-340">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fb94-340">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="9fb94-341">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="9fb94-341">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="9fb94-342">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-342">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="9fb94-343">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="9fb94-343">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="9fb94-344">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="9fb94-344">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-345">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-345">Batch</span></span>
* <span data-ttu-id="9fb94-346">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="9fb94-346">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-347">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-347">BatchAI</span></span>
* <span data-ttu-id="9fb94-348">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="9fb94-348">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-349">BotService</span><span class="sxs-lookup"><span data-stu-id="9fb94-349">BotService</span></span>
* <span data-ttu-id="9fb94-350">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="9fb94-350">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-351">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-351">CosmosDB</span></span>
* <span data-ttu-id="9fb94-352">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="9fb94-352">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="9fb94-353">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="9fb94-353">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="9fb94-354">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="9fb94-354">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="9fb94-355">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="9fb94-355">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fb94-356">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9fb94-356">EventGrid</span></span>
* <span data-ttu-id="9fb94-357">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="9fb94-357">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="9fb94-358">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="9fb94-358">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="9fb94-359">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="9fb94-359">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="9fb94-360">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="9fb94-360">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="9fb94-361">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-361">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-362">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-362">HDInsight</span></span>
* <span data-ttu-id="9fb94-363">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-363">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-364">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-364">IoT</span></span>
* <span data-ttu-id="9fb94-365">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="9fb94-365">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="9fb94-366">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="9fb94-366">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-367">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-367">Network</span></span>
* <span data-ttu-id="9fb94-368">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="9fb94-368">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="9fb94-369">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="9fb94-369">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="9fb94-370">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="9fb94-370">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="9fb94-371">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="9fb94-371">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-372">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-372">Resource</span></span>
* <span data-ttu-id="9fb94-373">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="9fb94-373">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="9fb94-374">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="9fb94-374">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fb94-375">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9fb94-375">ServiceBus</span></span>
* <span data-ttu-id="9fb94-376">Correction d’une erreur liée à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="9fb94-376">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-377">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-377">SQL</span></span>
* <span data-ttu-id="9fb94-378">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="9fb94-378">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="9fb94-379">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="9fb94-379">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="9fb94-380">SQLVm</span><span class="sxs-lookup"><span data-stu-id="9fb94-380">SQLVm</span></span>
* <span data-ttu-id="9fb94-381">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="9fb94-381">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="9fb94-382">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-382">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-383">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-383">Storage</span></span>
* <span data-ttu-id="9fb94-384">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9fb94-384">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="9fb94-385">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-385">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-386">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-386">VM</span></span>
* <span data-ttu-id="9fb94-387">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-387">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="9fb94-388">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-388">June 4, 2019</span></span>

<span data-ttu-id="9fb94-389">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="9fb94-389">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-390">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-390">Core</span></span>
* <span data-ttu-id="9fb94-391">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="9fb94-391">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-392">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-392">ACR</span></span>
* <span data-ttu-id="9fb94-393">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="9fb94-393">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-394">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-394">ACS</span></span>
* <span data-ttu-id="9fb94-395">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-395">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="9fb94-396">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="9fb94-396">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-397">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-397">Batch</span></span>
* <span data-ttu-id="9fb94-398">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="9fb94-398">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-399">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-399">IoT</span></span>
* <span data-ttu-id="9fb94-400">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-400">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-401">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-401">Network</span></span>
* <span data-ttu-id="9fb94-402">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="9fb94-402">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="9fb94-403">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-403">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="9fb94-404">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-404">Resource</span></span>
* <span data-ttu-id="9fb94-405">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="9fb94-405">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-406">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-406">Role</span></span>
* <span data-ttu-id="9fb94-407">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-407">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="9fb94-408">Calcul</span><span class="sxs-lookup"><span data-stu-id="9fb94-408">Compute</span></span>
* <span data-ttu-id="9fb94-409">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="9fb94-409">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="9fb94-410">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-410">May 21, 2019</span></span>

<span data-ttu-id="9fb94-411">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="9fb94-411">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-412">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-412">Core</span></span>
* <span data-ttu-id="9fb94-413">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="9fb94-413">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="9fb94-414">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="9fb94-414">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="9fb94-415">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="9fb94-415">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-416">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-416">ACR</span></span>
* <span data-ttu-id="9fb94-417">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="9fb94-417">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-418">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-418">ACS</span></span>
* <span data-ttu-id="9fb94-419">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="9fb94-419">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-420">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-420">AppService</span></span>
* <span data-ttu-id="9fb94-421">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="9fb94-421">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="9fb94-422">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="9fb94-422">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="9fb94-423">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="9fb94-423">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="9fb94-424">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="9fb94-424">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="9fb94-425">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fb94-425">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="9fb94-426">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="9fb94-426">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="9fb94-427">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-427">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-428">BotService</span><span class="sxs-lookup"><span data-stu-id="9fb94-428">BotService</span></span>
* <span data-ttu-id="9fb94-429">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-429">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="9fb94-430">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-430">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-431">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-431">Consumption</span></span>
* <span data-ttu-id="9fb94-432">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-432">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-433">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-433">IoT</span></span>
* <span data-ttu-id="9fb94-434">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="9fb94-434">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-435">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-435">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="9fb94-437">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="9fb94-437">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="9fb94-438">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="9fb94-438">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-439">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-439">RDBMS</span></span>
* <span data-ttu-id="9fb94-440">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="9fb94-440">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="9fb94-441">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fb94-441">RBAC</span></span>
* <span data-ttu-id="9fb94-442">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="9fb94-442">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-443">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-443">Storage</span></span>
* <span data-ttu-id="9fb94-444">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-444">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="9fb94-445">Calcul</span><span class="sxs-lookup"><span data-stu-id="9fb94-445">Compute</span></span>
* <span data-ttu-id="9fb94-446">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-446">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="9fb94-447">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="9fb94-447">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="9fb94-448">__Remarque__: il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="9fb94-448">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="9fb94-449">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-449">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="9fb94-450">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-450">May 6, 2019</span></span>

<span data-ttu-id="9fb94-451">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="9fb94-451">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-452">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-452">ACS</span></span>
* <span data-ttu-id="9fb94-453">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="9fb94-453">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="9fb94-454">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="9fb94-454">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="9fb94-455">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-455">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="9fb94-456">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-456">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-457">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-457">Appservice</span></span>
* <span data-ttu-id="9fb94-458">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="9fb94-458">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="9fb94-459">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="9fb94-459">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="9fb94-460">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fb94-460">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="9fb94-461">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="9fb94-461">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="9fb94-462">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fb94-462">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="9fb94-463">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="9fb94-463">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="9fb94-464">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="9fb94-464">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="9fb94-465">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="9fb94-465">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="9fb94-466">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-466">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="9fb94-467">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="9fb94-467">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-468">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-468">Batch</span></span>
* <span data-ttu-id="9fb94-469">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="9fb94-469">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-470">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fb94-470">Botservice</span></span>
* <span data-ttu-id="9fb94-471">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="9fb94-471">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="9fb94-472">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="9fb94-472">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="9fb94-473">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="9fb94-473">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="9fb94-474">__REMARQUE :__  `bot prepare-publish` utilise toujours l’ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-474">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="9fb94-475">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-475">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="9fb94-476">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-476">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="9fb94-477">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-477">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="9fb94-478">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="9fb94-478">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="9fb94-479">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="9fb94-479">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="9fb94-480">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="9fb94-480">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="9fb94-481">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="9fb94-481">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="9fb94-482">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="9fb94-482">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="9fb94-483">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="9fb94-483">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="9fb94-484">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="9fb94-484">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="9fb94-485">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-485">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="9fb94-486">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="9fb94-486">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="9fb94-487">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-487">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9fb94-488">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="9fb94-488">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="9fb94-489">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9fb94-489">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="9fb94-490">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-490">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9fb94-491">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="9fb94-491">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="9fb94-492">Configuration</span><span class="sxs-lookup"><span data-stu-id="9fb94-492">Configure</span></span>
* <span data-ttu-id="9fb94-493">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="9fb94-493">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fb94-494">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9fb94-494">Eventhubs</span></span>
* <span data-ttu-id="9fb94-495">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-495">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9fb94-496">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-496">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-497">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-497">Network</span></span>
* <span data-ttu-id="9fb94-498">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-498">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="9fb94-499">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9fb94-499">Policy Insights</span></span>
* <span data-ttu-id="9fb94-500">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-500">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-501">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-501">Role</span></span>
* <span data-ttu-id="9fb94-502">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-502">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fb94-503">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fb94-503">Service Bus</span></span>
* <span data-ttu-id="9fb94-504">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-504">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9fb94-505">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-505">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="9fb94-506">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="9fb94-506">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-507">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-507">SQL</span></span>
* <span data-ttu-id="9fb94-508">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-508">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-509">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-509">VM</span></span>
* <span data-ttu-id="9fb94-510">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="9fb94-510">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="9fb94-511">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="9fb94-511">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="9fb94-512">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-512">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="9fb94-513">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="9fb94-513">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="9fb94-514">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="9fb94-514">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="9fb94-515">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-515">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="9fb94-516">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-516">April 23, 2019</span></span>

<span data-ttu-id="9fb94-517">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="9fb94-517">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-518">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-518">ACS</span></span>
* <span data-ttu-id="9fb94-519">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="9fb94-519">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="9fb94-520">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="9fb94-520">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-521">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-521">AMS</span></span>
* <span data-ttu-id="9fb94-522">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="9fb94-522">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-523">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-523">AppService</span></span>
* <span data-ttu-id="9fb94-524">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="9fb94-524">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="9fb94-525">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="9fb94-525">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="9fb94-526">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="9fb94-526">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="9fb94-527">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="9fb94-527">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="9fb94-528">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="9fb94-528">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="9fb94-529">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-529">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="9fb94-530">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="9fb94-530">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="9fb94-531">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="9fb94-531">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="9fb94-532">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="9fb94-532">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9fb94-533">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="9fb94-533">Deployment Manager</span></span>
* <span data-ttu-id="9fb94-534">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="9fb94-534">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="9fb94-535">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-535">Lab</span></span>
* <span data-ttu-id="9fb94-536">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="9fb94-536">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-537">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-537">Network</span></span>
* <span data-ttu-id="9fb94-538">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="9fb94-538">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-539">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-539">Resource</span></span>
* <span data-ttu-id="9fb94-540">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="9fb94-540">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="9fb94-541">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="9fb94-541">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="9fb94-542">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-542">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="9fb94-543">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-543">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-544">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-544">SQL</span></span>
* <span data-ttu-id="9fb94-545">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="9fb94-545">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="9fb94-546">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-546">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="9fb94-547">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-547">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="9fb94-548">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-548">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-549">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-549">Storage</span></span>
* <span data-ttu-id="9fb94-550">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="9fb94-550">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-551">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-551">VM</span></span>
* <span data-ttu-id="9fb94-552">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="9fb94-552">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="9fb94-553">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="9fb94-553">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="9fb94-554">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="9fb94-554">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="9fb94-555">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-555">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-556">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-556">Core</span></span>
* <span data-ttu-id="9fb94-557">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="9fb94-557">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-558">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-558">ACR</span></span>
* <span data-ttu-id="9fb94-559">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="9fb94-559">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-560">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-560">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="9fb94-563">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-563">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="9fb94-564">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-564">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-565">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-565">AppService</span></span>
* <span data-ttu-id="9fb94-566">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fb94-566">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="9fb94-567">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-567">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="9fb94-568">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-568">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="9fb94-569">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9fb94-569">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="9fb94-570">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-570">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="9fb94-571">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="9fb94-571">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="9fb94-572">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="9fb94-572">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-573">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-573">CDN</span></span>
* <span data-ttu-id="9fb94-574">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="9fb94-574">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="9fb94-575">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9fb94-575">Feedback</span></span>
* <span data-ttu-id="9fb94-576">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="9fb94-576">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="9fb94-577">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="9fb94-577">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="9fb94-578">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="9fb94-578">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-579">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-579">Monitor</span></span>
* <span data-ttu-id="9fb94-580">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-580">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="9fb94-581">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-581">Network</span></span>
* <span data-ttu-id="9fb94-582">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="9fb94-582">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="9fb94-583">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-583">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="9fb94-584">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="9fb94-584">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="9fb94-585">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-585">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="9fb94-586">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="9fb94-586">PrivateDNS</span></span>
* <span data-ttu-id="9fb94-587">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="9fb94-587">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-588">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-588">Resource</span></span>
* <span data-ttu-id="9fb94-589">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-589">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-590">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-590">Role</span></span>
* <span data-ttu-id="9fb94-591">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-591">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="9fb94-592">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-592">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-593">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-593">SQL</span></span>
* <span data-ttu-id="9fb94-594">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="9fb94-594">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-595">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-595">Storage</span></span>
* <span data-ttu-id="9fb94-596">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-596">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="9fb94-597">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="9fb94-597">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="9fb94-598">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="9fb94-598">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="9fb94-599">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="9fb94-599">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="9fb94-600">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-600">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="9fb94-601">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-601">Core</span></span>
* <span data-ttu-id="9fb94-602">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="9fb94-602">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="9fb94-603">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="9fb94-603">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="9fb94-604">Cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-604">Cloud</span></span>
* <span data-ttu-id="9fb94-605">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="9fb94-605">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-606">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-606">ACR</span></span>
* <span data-ttu-id="9fb94-607">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="9fb94-607">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="9fb94-608">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-608">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="9fb94-609">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="9fb94-609">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="9fb94-610">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="9fb94-610">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-611">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-611">AppService</span></span>
* <span data-ttu-id="9fb94-612">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="9fb94-612">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="9fb94-613">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="9fb94-613">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="9fb94-614">Service BOT</span><span class="sxs-lookup"><span data-stu-id="9fb94-614">BOT Service</span></span>
* <span data-ttu-id="9fb94-615">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="9fb94-615">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="9fb94-616">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="9fb94-616">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="9fb94-617">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="9fb94-617">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="9fb94-618">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9fb94-618">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-619">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-619">CDN</span></span>
* <span data-ttu-id="9fb94-620">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-620">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="9fb94-621">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-621">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="9fb94-622">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="9fb94-622">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9fb94-623">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="9fb94-623">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-624">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9fb94-624">Cosmosdb</span></span>
* <span data-ttu-id="9fb94-625">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="9fb94-625">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="9fb94-626">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-626">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-627">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-627">Interactive</span></span>
* <span data-ttu-id="9fb94-628">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="9fb94-628">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-629">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-629">Monitor</span></span>
* <span data-ttu-id="9fb94-630">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-630">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-631">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-631">Network</span></span>
* <span data-ttu-id="9fb94-632">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="9fb94-632">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-633">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-633">Profile</span></span>
* <span data-ttu-id="9fb94-634">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="9fb94-634">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="9fb94-635">Postgres</span><span class="sxs-lookup"><span data-stu-id="9fb94-635">Postgres</span></span> 
* <span data-ttu-id="9fb94-636">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="9fb94-636">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="9fb94-637">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="9fb94-637">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-638">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-638">Resource</span></span>
* <span data-ttu-id="9fb94-639">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-639">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="9fb94-640">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="9fb94-640">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="9fb94-641">Graph</span><span class="sxs-lookup"><span data-stu-id="9fb94-641">Graph</span></span>
* <span data-ttu-id="9fb94-642">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="9fb94-642">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="9fb94-643">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="9fb94-643">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="9fb94-644">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="9fb94-644">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="9fb94-645">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-645">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="9fb94-646">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="9fb94-646">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-647">storage</span><span class="sxs-lookup"><span data-stu-id="9fb94-647">storage</span></span>
* <span data-ttu-id="9fb94-648">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="9fb94-648">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="9fb94-649">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="9fb94-649">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="9fb94-650">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="9fb94-650">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="9fb94-651">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="9fb94-651">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-652">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-652">VM</span></span>
* <span data-ttu-id="9fb94-653">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-653">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="9fb94-654">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-654">March 12, 2019</span></span>

<span data-ttu-id="9fb94-655">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="9fb94-655">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-656">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-656">Core</span></span>

* <span data-ttu-id="9fb94-657">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="9fb94-657">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-658">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-658">ACR</span></span>

* <span data-ttu-id="9fb94-659">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="9fb94-659">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-660">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-660">ACS</span></span>

* <span data-ttu-id="9fb94-661">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="9fb94-661">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="9fb94-662">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-662">AppService</span></span>

* <span data-ttu-id="9fb94-663">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="9fb94-663">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="9fb94-664">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-664">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="9fb94-665">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-665">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="9fb94-666">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-666">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-667">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fb94-667">Botservice</span></span>

* <span data-ttu-id="9fb94-668">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9fb94-668">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9fb94-669">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="9fb94-669">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9fb94-670">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-670">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="9fb94-671">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="9fb94-671">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-672">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-672">Container</span></span>

* <span data-ttu-id="9fb94-673">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-673">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="9fb94-674">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9fb94-674">EventHub</span></span>

* <span data-ttu-id="9fb94-675">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="9fb94-675">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="9fb94-676">Rechercher</span><span class="sxs-lookup"><span data-stu-id="9fb94-676">Find</span></span>

* <span data-ttu-id="9fb94-677">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="9fb94-677">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-678">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-678">HDInsight</span></span>

* <span data-ttu-id="9fb94-679">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="9fb94-679">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-680">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-680">Network</span></span>

* <span data-ttu-id="9fb94-681">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="9fb94-681">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-682">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fb94-682">Rdbms</span></span>

* <span data-ttu-id="9fb94-683">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="9fb94-683">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-684">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-684">Role</span></span>

* <span data-ttu-id="9fb94-685">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="9fb94-685">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="9fb94-686">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="9fb94-686">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fb94-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-687">Service Fabric</span></span>

* <span data-ttu-id="9fb94-688">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="9fb94-688">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="9fb94-689">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-689">February 26, 2019</span></span>

<span data-ttu-id="9fb94-690">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="9fb94-690">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-691">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-691">Core</span></span>

* <span data-ttu-id="9fb94-692">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="9fb94-692">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-693">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-693">ACR</span></span>

* <span data-ttu-id="9fb94-694">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-694">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="9fb94-695">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="9fb94-695">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-696">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-696">ACS</span></span>

* <span data-ttu-id="9fb94-697">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="9fb94-697">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-698">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-698">AppService</span></span>

* <span data-ttu-id="9fb94-699">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="9fb94-699">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-700">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-700">Batch</span></span>
* <span data-ttu-id="9fb94-701">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="9fb94-701">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="9fb94-702">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="9fb94-702">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="9fb94-703">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="9fb94-703">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="9fb94-704">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="9fb94-704">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="9fb94-705">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="9fb94-705">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="9fb94-706">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="9fb94-706">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-707">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-707">CosmosDB</span></span>

* <span data-ttu-id="9fb94-708">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-708">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="9fb94-709">Kusto</span><span class="sxs-lookup"><span data-stu-id="9fb94-709">Kusto</span></span>

* <span data-ttu-id="9fb94-710">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="9fb94-710">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-711">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-711">Network</span></span>

* <span data-ttu-id="9fb94-712">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-712">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="9fb94-713">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="9fb94-713">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="9fb94-714">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="9fb94-714">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="9fb94-715">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-715">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="9fb94-716">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-716">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="9fb94-717">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-717">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="9fb94-718">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="9fb94-718">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-719">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-719">Resource</span></span>

* <span data-ttu-id="9fb94-720">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-720">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="9fb94-721">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-721">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="9fb94-722">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-722">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="9fb94-723">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-723">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="9fb94-724">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-724">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-725">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-725">Role</span></span>

* <span data-ttu-id="9fb94-726">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-726">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-727">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-727">VM</span></span>

* <span data-ttu-id="9fb94-728">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="9fb94-728">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="9fb94-729">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-729">February 12, 2019</span></span>

<span data-ttu-id="9fb94-730">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="9fb94-730">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-731">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-731">Core</span></span>

* <span data-ttu-id="9fb94-732">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="9fb94-732">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="9fb94-733">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="9fb94-733">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-734">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-734">ACR</span></span>
* <span data-ttu-id="9fb94-735">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="9fb94-735">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="9fb94-736">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-736">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-737">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-737">ACS</span></span>
* <span data-ttu-id="9fb94-738">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-738">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="9fb94-739">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="9fb94-739">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="9fb94-740">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9fb94-740">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-741">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-741">AMS</span></span>
* <span data-ttu-id="9fb94-742">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-742">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="9fb94-743">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-743">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-744">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-744">Appservice</span></span>
* <span data-ttu-id="9fb94-745">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-745">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="9fb94-746">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="9fb94-746">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="9fb94-747">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-747">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="9fb94-748">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="9fb94-748">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="9fb94-749">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="9fb94-749">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-750">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fb94-750">Botservice</span></span>
* <span data-ttu-id="9fb94-751">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="9fb94-751">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="9fb94-752">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="9fb94-752">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="9fb94-753">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-753">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="9fb94-754">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="9fb94-754">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="9fb94-755">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="9fb94-755">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="9fb94-756">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="9fb94-756">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="9fb94-757">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="9fb94-757">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="9fb94-758">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="9fb94-758">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="9fb94-759">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="9fb94-759">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="9fb94-760">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="9fb94-760">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fb94-761">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fb94-761">Key Vault</span></span>
* <span data-ttu-id="9fb94-762">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="9fb94-762">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-763">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-763">Monitor</span></span>
* <span data-ttu-id="9fb94-764">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="9fb94-764">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-765">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-765">Network</span></span>
* <span data-ttu-id="9fb94-766">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="9fb94-766">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="9fb94-767">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9fb94-767">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="9fb94-768">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-768">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="9fb94-769">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-769">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9fb94-770">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9fb94-770">Policy Insights</span></span>
* <span data-ttu-id="9fb94-771">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="9fb94-771">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-772">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-772">RDBMS</span></span>
* <span data-ttu-id="9fb94-773">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-773">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="9fb94-774">Redis</span><span class="sxs-lookup"><span data-stu-id="9fb94-774">Redis</span></span>
* <span data-ttu-id="9fb94-775">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="9fb94-775">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="9fb94-776">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="9fb94-776">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="9fb94-777">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="9fb94-777">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="9fb94-778">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="9fb94-778">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="9fb94-779">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="9fb94-779">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="9fb94-780">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="9fb94-780">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="9fb94-781">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="9fb94-781">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-782">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-782">Role</span></span>
* <span data-ttu-id="9fb94-783">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="9fb94-783">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="9fb94-784">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-784">SQL VM</span></span>
* <span data-ttu-id="9fb94-785">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="9fb94-785">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-786">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-786">VM</span></span>
* <span data-ttu-id="9fb94-787">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="9fb94-787">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="9fb94-788">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-788">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="9fb94-789">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="9fb94-789">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="9fb94-790">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="9fb94-790">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="9fb94-791">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-791">January 31, 2019</span></span>

<span data-ttu-id="9fb94-792">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="9fb94-792">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-793">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-793">Core</span></span>

* <span data-ttu-id="9fb94-794">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="9fb94-794">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="9fb94-795">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-795">January 28, 2019</span></span>

<span data-ttu-id="9fb94-796">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="9fb94-796">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-797">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-797">ACR</span></span>
* <span data-ttu-id="9fb94-798">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="9fb94-798">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-799">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-799">ACS</span></span>
* <span data-ttu-id="9fb94-800">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="9fb94-800">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9fb94-801">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="9fb94-801">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="9fb94-802">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="9fb94-802">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-803">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-803">AMS</span></span>
* <span data-ttu-id="9fb94-804">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="9fb94-804">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="9fb94-805">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="9fb94-805">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-806">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-806">Appservice</span></span>
* <span data-ttu-id="9fb94-807">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-807">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="9fb94-808">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="9fb94-808">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="9fb94-809">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="9fb94-809">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-810">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-810">Container</span></span>
* <span data-ttu-id="9fb94-811">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="9fb94-811">Added `container start` command</span></span>
* <span data-ttu-id="9fb94-812">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-812">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fb94-813">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9fb94-813">EventGrid</span></span>
* <span data-ttu-id="9fb94-814">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-814">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="9fb94-815">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="9fb94-815">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="9fb94-816">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="9fb94-816">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="9fb94-817">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="9fb94-817">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="9fb94-818">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="9fb94-818">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-819">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-819">HDInsight</span></span>
* <span data-ttu-id="9fb94-820">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-820">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="9fb94-821">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="9fb94-821">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="9fb94-822">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-822">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="9fb94-823">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-823">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="9fb94-824">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="9fb94-824">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="9fb94-825">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-825">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-826">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-826">IoT</span></span>
* <span data-ttu-id="9fb94-827">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="9fb94-827">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="9fb94-828">Kusto</span><span class="sxs-lookup"><span data-stu-id="9fb94-828">Kusto</span></span>
* <span data-ttu-id="9fb94-829">Préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-829">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-830">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-830">Monitor</span></span>
* <span data-ttu-id="9fb94-831">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-831">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-832">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-832">Profile</span></span>
* <span data-ttu-id="9fb94-833">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="9fb94-833">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-834">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-834">Network</span></span>
* <span data-ttu-id="9fb94-835">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="9fb94-835">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="9fb94-836">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="9fb94-836">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-837">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-837">Resource</span></span>
* <span data-ttu-id="9fb94-838">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-838">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="9fb94-839">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-839">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="9fb94-840">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-840">SQL Virtual Machine</span></span>
* <span data-ttu-id="9fb94-841">Préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-841">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-842">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-842">Storage</span></span>
* <span data-ttu-id="9fb94-843">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="9fb94-843">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="9fb94-844">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="9fb94-844">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-845">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-845">VM</span></span>
* <span data-ttu-id="9fb94-846">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="9fb94-846">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="9fb94-847">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9fb94-847">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="9fb94-848">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="9fb94-848">January 15, 2019</span></span>

<span data-ttu-id="9fb94-849">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="9fb94-849">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-850">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-850">ACR</span></span>
* <span data-ttu-id="9fb94-851">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-851">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="9fb94-852">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="9fb94-852">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="9fb94-853">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-853">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="9fb94-854">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-854">ACS</span></span>
* <span data-ttu-id="9fb94-855">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="9fb94-855">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-856">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-856">Appservice</span></span>
* <span data-ttu-id="9fb94-857">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="9fb94-857">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="9fb94-858">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-858">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="9fb94-859">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="9fb94-859">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="9fb94-860">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="9fb94-860">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-861">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fb94-861">Botservice</span></span>
* <span data-ttu-id="9fb94-862">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-862">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="9fb94-863">Configuration</span><span class="sxs-lookup"><span data-stu-id="9fb94-863">Configure</span></span>
* <span data-ttu-id="9fb94-864">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="9fb94-864">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-865">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-865">CosmosDB</span></span>
* <span data-ttu-id="9fb94-866">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="9fb94-866">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-867">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-867">HDInsight</span></span>
* <span data-ttu-id="9fb94-868">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="9fb94-868">Added commands for managing applications</span></span>
* <span data-ttu-id="9fb94-869">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="9fb94-869">Added commands for managing script actions</span></span>
* <span data-ttu-id="9fb94-870">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="9fb94-870">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="9fb94-871">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="9fb94-871">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="9fb94-872">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-872">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-873">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-873">Network</span></span>
* <span data-ttu-id="9fb94-874">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-874">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="9fb94-875">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="9fb94-875">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="9fb94-876">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-876">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="9fb94-877">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-877">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-878">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-878">Role</span></span>
* <span data-ttu-id="9fb94-879">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-879">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="9fb94-880">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="9fb94-880">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="9fb94-881">Sécurité</span><span class="sxs-lookup"><span data-stu-id="9fb94-881">Security</span></span>
* <span data-ttu-id="9fb94-882">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-882">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-883">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-883">Storage</span></span>
* <span data-ttu-id="9fb94-884">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="9fb94-884">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="9fb94-885">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="9fb94-885">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="9fb94-886">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-886">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="9fb94-887">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-887">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="9fb94-888">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-888">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-889">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-889">VM</span></span>
* <span data-ttu-id="9fb94-890">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="9fb94-890">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="9fb94-891">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-891">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fb94-892">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="9fb94-892">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="9fb94-893">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-893">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="9fb94-894">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-894">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="9fb94-895">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="9fb94-895">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="9fb94-896">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-896">December 20, 2018</span></span>

<span data-ttu-id="9fb94-897">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="9fb94-897">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="9fb94-898">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-898">Appservice</span></span>
* <span data-ttu-id="9fb94-899">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fb94-899">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="9fb94-900">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="9fb94-900">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="9fb94-901">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-901">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9fb94-902">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9fb94-902">IoTCentral</span></span>
* <span data-ttu-id="9fb94-903">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="9fb94-903">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-904">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-904">Role</span></span>
* <span data-ttu-id="9fb94-905">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="9fb94-905">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-906">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-906">SQL</span></span>
* <span data-ttu-id="9fb94-907">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="9fb94-907">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-908">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-908">VM</span></span>
* <span data-ttu-id="9fb94-909">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-909">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="9fb94-910">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-910">December 18, 2018</span></span>

<span data-ttu-id="9fb94-911">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="9fb94-911">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="9fb94-912">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-912">ACR</span></span>
* <span data-ttu-id="9fb94-913">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="9fb94-913">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="9fb94-914">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="9fb94-914">Condensed the table layout for task list</span></span>
* <span data-ttu-id="9fb94-915">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9fb94-915">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-916">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-916">ACS</span></span>
* <span data-ttu-id="9fb94-917">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="9fb94-917">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9fb94-918">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-918">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="9fb94-919">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-919">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="9fb94-920">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="9fb94-920">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="9fb94-921">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-921">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="9fb94-922">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="9fb94-922">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-923">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-923">Appservice</span></span>
* <span data-ttu-id="9fb94-924">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="9fb94-924">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="9fb94-925">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fb94-925">Botservice</span></span>
* <span data-ttu-id="9fb94-926">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-926">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="9fb94-927">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="9fb94-927">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="9fb94-928">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="9fb94-928">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="9fb94-929">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="9fb94-929">Reduced Kudu network calls</span></span>
* <span data-ttu-id="9fb94-930">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="9fb94-930">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-931">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-931">Consumption</span></span>
* <span data-ttu-id="9fb94-932">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="9fb94-932">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-933">CosmosDB</span></span>
* <span data-ttu-id="9fb94-934">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="9fb94-934">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="9fb94-935">Cartes</span><span class="sxs-lookup"><span data-stu-id="9fb94-935">Maps</span></span>
* <span data-ttu-id="9fb94-936">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-936">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-937">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-937">Network</span></span>
* <span data-ttu-id="9fb94-938">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="9fb94-938">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="9fb94-939">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-939">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-940">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-940">Resource</span></span>
* <span data-ttu-id="9fb94-941">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-941">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="9fb94-942">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-942">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-943">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-943">Storage</span></span>
*  <span data-ttu-id="9fb94-944">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-944">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-945">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-945">VM</span></span>
* <span data-ttu-id="9fb94-946">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="9fb94-946">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="9fb94-947">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-947">December 4, 2018</span></span>

<span data-ttu-id="9fb94-948">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="9fb94-948">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="9fb94-949">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-949">Core</span></span>
* <span data-ttu-id="9fb94-950">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="9fb94-950">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="9fb94-951">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="9fb94-951">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-952">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-952">Appservice</span></span>
* <span data-ttu-id="9fb94-953">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="9fb94-953">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="9fb94-954">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="9fb94-954">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-955">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-955">Network</span></span>
* <span data-ttu-id="9fb94-956">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="9fb94-956">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-957">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-957">Role</span></span>
* <span data-ttu-id="9fb94-958">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="9fb94-958">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="9fb94-959">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-959">VM</span></span>
* <span data-ttu-id="9fb94-960">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="9fb94-960">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="9fb94-961">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="9fb94-961">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="9fb94-962">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="9fb94-962">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="9fb94-963">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="9fb94-963">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="9fb94-964">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-964">November 20, 2018</span></span>

<span data-ttu-id="9fb94-965">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="9fb94-965">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="9fb94-966">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-966">Core</span></span>
* <span data-ttu-id="9fb94-967">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="9fb94-967">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-968">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-968">ACR</span></span>
* <span data-ttu-id="9fb94-969">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="9fb94-969">Added context token to task step</span></span>
* <span data-ttu-id="9fb94-970">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="9fb94-970">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="9fb94-971">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9fb94-971">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-972">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-972">Appservice</span></span>
* <span data-ttu-id="9fb94-973">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="9fb94-973">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="9fb94-974">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-974">Updated the default `node_version`.</span></span> <span data-ttu-id="9fb94-975">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="9fb94-975">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="9fb94-976">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-976">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="9fb94-977">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="9fb94-977">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9fb94-978">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9fb94-978">IotCentral</span></span>
* <span data-ttu-id="9fb94-979">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fb94-979">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-980">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-980">KeyVault</span></span>
* <span data-ttu-id="9fb94-981">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="9fb94-981">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-982">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-982">Network</span></span>
* <span data-ttu-id="9fb94-983">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="9fb94-983">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="9fb94-984">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-984">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="9fb94-985">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-985">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="9fb94-986">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="9fb94-986">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-987">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fb94-987">Rdbms</span></span>
* <span data-ttu-id="9fb94-988">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="9fb94-988">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="9fb94-989">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="9fb94-989">Rbac</span></span>
* <span data-ttu-id="9fb94-990">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-990">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="9fb94-991">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-991">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="9fb94-992">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-992">Storage</span></span>
* <span data-ttu-id="9fb94-993">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-993">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="9fb94-994">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-994">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="9fb94-995">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="9fb94-995">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="9fb94-996">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="9fb94-996">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-997">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-997">VM</span></span>
* <span data-ttu-id="9fb94-998">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="9fb94-998">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="9fb94-999">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="9fb94-999">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="9fb94-1000">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1000">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="9fb94-1001">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1001">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="9fb94-1002">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1002">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="9fb94-1003">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1003">Added `snapshot wait` command</span></span>
* <span data-ttu-id="9fb94-1004">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1004">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="9fb94-1005">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1005">November 6, 2018</span></span>

<span data-ttu-id="9fb94-1006">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="9fb94-1006">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1007">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1007">Core</span></span>
* <span data-ttu-id="9fb94-1008">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="9fb94-1008">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1009">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1009">ACR</span></span>
* <span data-ttu-id="9fb94-1010">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="9fb94-1010">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="9fb94-1011">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="9fb94-1011">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1012">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1012">ACS</span></span>
* <span data-ttu-id="9fb94-1013">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1013">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="9fb94-1014">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fb94-1014">Advisor</span></span>
* <span data-ttu-id="9fb94-1015">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1015">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-1016">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1016">AMS</span></span>
* <span data-ttu-id="9fb94-1017">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1017">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="9fb94-1018">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1018">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="9fb94-1019">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1019">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="9fb94-1020">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="9fb94-1020">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="9fb94-1021">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1021">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="9fb94-1022">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1022">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="9fb94-1023">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1023">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="9fb94-1024">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1024">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="9fb94-1025">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1025">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="9fb94-1026">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1026">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="9fb94-1027">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1027">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="9fb94-1028">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1028">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="9fb94-1029">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="9fb94-1029">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="9fb94-1030">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1030">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="9fb94-1031">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1031">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="9fb94-1032">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="9fb94-1032">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="9fb94-1033">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1033">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1034">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1034">AppService</span></span>
* <span data-ttu-id="9fb94-1035">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1035">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="9fb94-1036">Configuration</span><span class="sxs-lookup"><span data-stu-id="9fb94-1036">Configure</span></span>
* <span data-ttu-id="9fb94-1037">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1037">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1038">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1038">Container</span></span>
* <span data-ttu-id="9fb94-1039">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="9fb94-1039">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="9fb94-1040">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9fb94-1040">EventHub</span></span>
* <span data-ttu-id="9fb94-1041">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1041">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1042">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1042">Interactive</span></span>
* <span data-ttu-id="9fb94-1043">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="9fb94-1043">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1044">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1044">Monitor</span></span>
* <span data-ttu-id="9fb94-1045">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1045">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1046">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1046">Network</span></span>
* <span data-ttu-id="9fb94-1047">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1047">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="9fb94-1048">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1048">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="9fb94-1049">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1049">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="9fb94-1050">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1050">Profile</span></span>
* <span data-ttu-id="9fb94-1051">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="9fb94-1051">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1052">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1052">RDBMS</span></span>
* <span data-ttu-id="9fb94-1053">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="9fb94-1053">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1054">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1054">Resource</span></span>
* <span data-ttu-id="9fb94-1055">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1055">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1056">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1056">Role</span></span>
* <span data-ttu-id="9fb94-1057">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="9fb94-1057">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="9fb94-1058">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1058">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="9fb94-1059">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="9fb94-1059">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1060">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1060">Storage</span></span>
* <span data-ttu-id="9fb94-1061">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1061">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1062">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1062">VM</span></span>
* <span data-ttu-id="9fb94-1063">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="9fb94-1063">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="9fb94-1064">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1064">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="9fb94-1065">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="9fb94-1065">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="9fb94-1066">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="9fb94-1066">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="9fb94-1067">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="9fb94-1067">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="9fb94-1068">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1068">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="9fb94-1069">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1069">October 23, 2018</span></span>

<span data-ttu-id="9fb94-1070">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="9fb94-1070">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1071">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1071">Core</span></span>
* <span data-ttu-id="9fb94-1072">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1072">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="9fb94-1073">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1073">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1074">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1074">ACR</span></span>
* <span data-ttu-id="9fb94-1075">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="9fb94-1075">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-1076">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-1076">CDN</span></span>
* <span data-ttu-id="9fb94-1077">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1077">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9fb94-1078">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1078">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1079">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1079">Container</span></span>
* <span data-ttu-id="9fb94-1080">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="9fb94-1080">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="9fb94-1081">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1081">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="9fb94-1082">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="9fb94-1082">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="9fb94-1083">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1083">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="9fb94-1084">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="9fb94-1084">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="9fb94-1085">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="9fb94-1085">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="9fb94-1086">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1086">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-1087">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-1087">CosmosDB</span></span>
* <span data-ttu-id="9fb94-1088">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1088">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1089">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1089">Interactive</span></span>
* <span data-ttu-id="9fb94-1090">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="9fb94-1090">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="9fb94-1091">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fb94-1091">IoT Central</span></span>
* <span data-ttu-id="9fb94-1092">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="9fb94-1092">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="9fb94-1093">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="9fb94-1093">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1094">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1094">Monitor</span></span>
* <span data-ttu-id="9fb94-1095">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1095">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="9fb94-1096">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1096">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="9fb94-1097">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="9fb94-1097">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9fb94-1098">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="9fb94-1098">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="9fb94-1099">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1099">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="9fb94-1100">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1100">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="9fb94-1101">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1101">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="9fb94-1102">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="9fb94-1102">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9fb94-1103">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="9fb94-1103">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="9fb94-1104">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1104">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1105">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1105">Network</span></span>
* <span data-ttu-id="9fb94-1106">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1106">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="9fb94-1107">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1107">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fb94-1108">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9fb94-1108">ServiceBus</span></span>
* <span data-ttu-id="9fb94-1109">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fb94-1109">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1110">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1110">SQL</span></span>
* <span data-ttu-id="9fb94-1111">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-1111">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1112">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1112">Storage</span></span>
* <span data-ttu-id="9fb94-1113">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="9fb94-1113">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="9fb94-1114">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1114">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1115">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1115">VM</span></span>
* <span data-ttu-id="9fb94-1116">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1116">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fb94-1117">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1117">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="9fb94-1118">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1118">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="9fb94-1119">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1119">October 16, 2018</span></span>

<span data-ttu-id="9fb94-1120">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="9fb94-1120">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1121">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1121">VM</span></span>
* <span data-ttu-id="9fb94-1122">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9fb94-1122">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="9fb94-1123">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1123">October 9, 2018</span></span>

<span data-ttu-id="9fb94-1124">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="9fb94-1124">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1125">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1125">Core</span></span>
* <span data-ttu-id="9fb94-1126">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1126">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1127">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1127">ACR</span></span>
* <span data-ttu-id="9fb94-1128">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="9fb94-1128">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1129">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1129">ACS</span></span>
* <span data-ttu-id="9fb94-1130">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="9fb94-1130">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="9fb94-1131">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="9fb94-1131">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="9fb94-1132">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1132">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="9fb94-1133">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1133">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1134">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1134">Container</span></span>
* <span data-ttu-id="9fb94-1135">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="9fb94-1135">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="9fb94-1136">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-1136">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="9fb94-1137">Event Hub</span><span class="sxs-lookup"><span data-stu-id="9fb94-1137">Event Hub</span></span>
* <span data-ttu-id="9fb94-1138">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1138">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="9fb94-1139">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1139">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="9fb94-1140">Extensions</span><span class="sxs-lookup"><span data-stu-id="9fb94-1140">Extensions</span></span>
* <span data-ttu-id="9fb94-1141">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1141">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fb94-1142">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fb94-1142">HDInsight</span></span>
* <span data-ttu-id="9fb94-1143">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1143">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-1144">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1144">IoT</span></span>
* <span data-ttu-id="9fb94-1145">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="9fb94-1145">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-1146">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-1146">KeyVault</span></span>
* <span data-ttu-id="9fb94-1147">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="9fb94-1147">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1148">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1148">Network</span></span>
* <span data-ttu-id="9fb94-1149">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1149">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="9fb94-1150">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="9fb94-1150">See #6052</span></span>
* <span data-ttu-id="9fb94-1151">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1151">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="9fb94-1152">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="9fb94-1152">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="9fb94-1153">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1153">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="9fb94-1154">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1154">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="9fb94-1155">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1155">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="9fb94-1156">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1156">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1157">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1157">Role</span></span>
* <span data-ttu-id="9fb94-1158">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1158">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="9fb94-1159">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1159">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="9fb94-1160">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="9fb94-1160">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="9fb94-1161">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1161">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fb94-1162">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fb94-1162">Service Bus</span></span>
* <span data-ttu-id="9fb94-1163">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1163">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1164">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1164">VM</span></span>
* <span data-ttu-id="9fb94-1165">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1165">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="9fb94-1166">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1166">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="9fb94-1167">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1167">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="9fb94-1168">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1168">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="9fb94-1169">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1169">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="9fb94-1170">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="9fb94-1170">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="9fb94-1171">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1171">September 21, 2018</span></span>

<span data-ttu-id="9fb94-1172">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="9fb94-1172">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1173">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1173">ACR</span></span>
* <span data-ttu-id="9fb94-1174">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1174">Added ACR Task commands</span></span>
* <span data-ttu-id="9fb94-1175">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1175">Added quick run command</span></span>
* <span data-ttu-id="9fb94-1176">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1176">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="9fb94-1177">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1177">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="9fb94-1178">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1178">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="9fb94-1179">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="9fb94-1179">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1180">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1180">ACS</span></span>
* <span data-ttu-id="9fb94-1181">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1181">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="9fb94-1182">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="9fb94-1182">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1183">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1183">AppService</span></span>

* <span data-ttu-id="9fb94-1184">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1184">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="9fb94-1185">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="9fb94-1185">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="9fb94-1186">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="9fb94-1186">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="9fb94-1187">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1187">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-1188">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1188">Batch</span></span>
* <span data-ttu-id="9fb94-1189">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="9fb94-1189">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="9fb94-1190">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1190">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="9fb94-1191">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1191">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="9fb94-1192">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1192">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fb94-1193">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1193">Batch AI</span></span> 
* <span data-ttu-id="9fb94-1194">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1194">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fb94-1195">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1195">Cognitive Services</span></span>
* <span data-ttu-id="9fb94-1196">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1196">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="9fb94-1197">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1197">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="9fb94-1198">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1198">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="9fb94-1199">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1199">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="9fb94-1200">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1200">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="9fb94-1201">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1201">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1202">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1202">Container</span></span>
* <span data-ttu-id="9fb94-1203">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="9fb94-1203">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="9fb94-1204">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1204">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="9fb94-1205">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-1205">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="9fb94-1206">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1206">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="9fb94-1207">DataLake</span><span class="sxs-lookup"><span data-stu-id="9fb94-1207">Datalake</span></span>
* <span data-ttu-id="9fb94-1208">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-1208">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="9fb94-1209">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="9fb94-1209">Interactive Shell</span></span>
* <span data-ttu-id="9fb94-1210">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1210">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="9fb94-1211">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1211">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-1212">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1212">IoT</span></span>
* <span data-ttu-id="9fb94-1213">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1213">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fb94-1214">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fb94-1214">Key Vault</span></span>
* <span data-ttu-id="9fb94-1215">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="9fb94-1215">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1216">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1216">Network</span></span>
* <span data-ttu-id="9fb94-1217">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1217">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="9fb94-1218">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1218">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="9fb94-1219">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="9fb94-1219">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="9fb94-1220">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1220">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="9fb94-1221">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1221">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="9fb94-1222">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1222">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="9fb94-1223">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1223">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="9fb94-1224">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1224">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="9fb94-1225">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1225">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="9fb94-1226">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1226">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="9fb94-1227">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1227">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="9fb94-1228">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1228">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="9fb94-1229">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1229">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="9fb94-1230">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1230">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="9fb94-1231">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1231">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="9fb94-1232">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="9fb94-1232">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="9fb94-1233">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1233">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="9fb94-1234">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1234">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1235">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1235">RDBMS</span></span>
* <span data-ttu-id="9fb94-1236">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-1236">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="9fb94-1237">Réservation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1237">Reservation</span></span>
* <span data-ttu-id="9fb94-1238">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1238">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="9fb94-1239">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1239">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="9fb94-1240">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="9fb94-1240">Manage App</span></span>
* <span data-ttu-id="9fb94-1241">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1241">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="9fb94-1242">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="9fb94-1242">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1243">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1243">Role</span></span>
* <span data-ttu-id="9fb94-1244">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1244">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="9fb94-1245">SignalR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1245">SignalR</span></span>
* <span data-ttu-id="9fb94-1246">Première version</span><span class="sxs-lookup"><span data-stu-id="9fb94-1246">First release</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1247">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1247">Storage</span></span>
* <span data-ttu-id="9fb94-1248">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="9fb94-1248">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="9fb94-1249">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="9fb94-1249">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1250">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1250">VM</span></span>
* <span data-ttu-id="9fb94-1251">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1251">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="9fb94-1252">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1252">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="9fb94-1253">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1253">August 28, 2018</span></span>

<span data-ttu-id="9fb94-1254">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="9fb94-1254">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1255">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1255">Core</span></span>

* <span data-ttu-id="9fb94-1256">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1256">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="9fb94-1257">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fb94-1257">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1258">ACR</span></span>

* <span data-ttu-id="9fb94-1259">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="9fb94-1259">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="9fb94-1260">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1260">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1261">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1261">ACS</span></span>

* <span data-ttu-id="9fb94-1262">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1262">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="9fb94-1263">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="9fb94-1263">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1264">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1264">AppService</span></span>

* <span data-ttu-id="9fb94-1265">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="9fb94-1265">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="9fb94-1266">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="9fb94-1266">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="9fb94-1267">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1267">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="9fb94-1268">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9fb94-1268">Backup</span></span>

* <span data-ttu-id="9fb94-1269">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1269">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="9fb94-1270">Service de robot</span><span class="sxs-lookup"><span data-stu-id="9fb94-1270">Bot Service</span></span>

* <span data-ttu-id="9fb94-1271">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1271">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fb94-1272">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1272">Cognitive Services</span></span>

* <span data-ttu-id="9fb94-1273">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1273">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-1274">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1274">IoT</span></span>

* <span data-ttu-id="9fb94-1275">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1275">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1276">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1276">Monitor</span></span>

* <span data-ttu-id="9fb94-1277">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="9fb94-1277">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="9fb94-1278">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1278">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1279">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1279">Network</span></span>

* <span data-ttu-id="9fb94-1280">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1280">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1281">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1281">Resource</span></span>

* <span data-ttu-id="9fb94-1282">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1282">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1283">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1283">Storage</span></span>

* <span data-ttu-id="9fb94-1284">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1284">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1285">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1285">VM</span></span>

* <span data-ttu-id="9fb94-1286">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1286">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="9fb94-1287">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1287">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="9fb94-1288">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1288">Auguest 14, 2018</span></span>

<span data-ttu-id="9fb94-1289">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="9fb94-1289">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1290">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1290">Core</span></span>

* <span data-ttu-id="9fb94-1291">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1291">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="9fb94-1292">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="9fb94-1292">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="9fb94-1293">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1293">Telemetry</span></span>

* <span data-ttu-id="9fb94-1294">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1294">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1295">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1295">ACR</span></span>

* <span data-ttu-id="9fb94-1296">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1296">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="9fb94-1297">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1297">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1298">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1298">ACS</span></span>

* <span data-ttu-id="9fb94-1299">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-1299">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="9fb94-1300">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1300">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="9fb94-1301">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1301">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="9fb94-1302">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1302">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="9fb94-1303">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="9fb94-1303">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="9fb94-1304">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1304">AppService</span></span>

* <span data-ttu-id="9fb94-1305">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1305">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="9fb94-1306">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="9fb94-1306">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-1307">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1307">BatchAI</span></span>

* <span data-ttu-id="9fb94-1308">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="9fb94-1308">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="9fb94-1309">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1309">Container</span></span>

* <span data-ttu-id="9fb94-1310">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1310">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="9fb94-1311">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1311">IoT</span></span>

* <span data-ttu-id="9fb94-1312">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="9fb94-1312">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="9fb94-1313">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1313">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="9fb94-1314">Iot Central</span><span class="sxs-lookup"><span data-stu-id="9fb94-1314">Iot Central</span></span>

* <span data-ttu-id="9fb94-1315">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fb94-1315">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-1316">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-1316">KeyVault</span></span>


* <span data-ttu-id="9fb94-1317">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1317">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="9fb94-1318">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1318">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="9fb94-1319">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="9fb94-1319">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="9fb94-1320">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1320">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="9fb94-1321">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1321">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="9fb94-1322">Relais</span><span class="sxs-lookup"><span data-stu-id="9fb94-1322">Relay</span></span>

* <span data-ttu-id="9fb94-1323">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1323">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1324">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1324">Sql</span></span>

* <span data-ttu-id="9fb94-1325">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1325">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1326">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1326">Storage</span></span>

* <span data-ttu-id="9fb94-1327">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="9fb94-1327">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="9fb94-1328">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1328">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="9fb94-1329">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1329">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="9fb94-1330">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="9fb94-1330">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="9fb94-1331">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1331">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1332">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1332">VM</span></span>

* <span data-ttu-id="9fb94-1333">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1333">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="9fb94-1334">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1334">July 31, 2018</span></span>

<span data-ttu-id="9fb94-1335">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="9fb94-1335">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1336">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1336">ACR</span></span>

* <span data-ttu-id="9fb94-1337">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1337">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="9fb94-1338">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1338">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1339">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1339">ACS</span></span>

* <span data-ttu-id="9fb94-1340">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1340">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-1341">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1341">Batch</span></span>

* <span data-ttu-id="9fb94-1342">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fb94-1342">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1343">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1343">Container</span></span>

* <span data-ttu-id="9fb94-1344">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="9fb94-1344">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1345">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1345">Network</span></span>

* <span data-ttu-id="9fb94-1346">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fb94-1346">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="9fb94-1347">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1347">Resource</span></span>

* <span data-ttu-id="9fb94-1348">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1348">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="9fb94-1349">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1349">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1350">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1350">Role</span></span>

* <span data-ttu-id="9fb94-1351">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-1351">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="9fb94-1352">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1352">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="9fb94-1353">Recherche</span><span class="sxs-lookup"><span data-stu-id="9fb94-1353">Search</span></span>

* <span data-ttu-id="9fb94-1354">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="9fb94-1354">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fb94-1355">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fb94-1355">Service Bus</span></span>

* <span data-ttu-id="9fb94-1356">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="9fb94-1356">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="9fb94-1357">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1357">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="9fb94-1358">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1358">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="9fb94-1359">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1359">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1360">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1360">Storage</span></span>

* <span data-ttu-id="9fb94-1361">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="9fb94-1361">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="9fb94-1362">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1362">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1363">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1363">VM</span></span>

* <span data-ttu-id="9fb94-1364">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1364">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="9fb94-1365">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1365">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="9fb94-1366">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="9fb94-1366">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="9fb94-1367">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="9fb94-1367">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="9fb94-1368">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1368">July 18, 2018</span></span>

<span data-ttu-id="9fb94-1369">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="9fb94-1369">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1370">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1370">Core</span></span>

* <span data-ttu-id="9fb94-1371">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-1371">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="9fb94-1372">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="9fb94-1372">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="9fb94-1373">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="9fb94-1373">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1374">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1374">ACR</span></span>

* <span data-ttu-id="9fb94-1375">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1375">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="9fb94-1376">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1376">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="9fb94-1377">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1377">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="9fb94-1378">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="9fb94-1378">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1379">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1379">ACS</span></span>

* <span data-ttu-id="9fb94-1380">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="9fb94-1380">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1381">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1381">AppService</span></span>

* <span data-ttu-id="9fb94-1382">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="9fb94-1382">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-1383">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1383">Batch</span></span>

* <span data-ttu-id="9fb94-1384">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fb94-1384">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="9fb94-1385">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-1385">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fb94-1386">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1386">Batch AI</span></span>

* <span data-ttu-id="9fb94-1387">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1387">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1388">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1388">Container</span></span>

* <span data-ttu-id="9fb94-1389">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="9fb94-1389">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="9fb94-1390">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="9fb94-1390">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1391">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1391">Network</span></span>

* <span data-ttu-id="9fb94-1392">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1392">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="9fb94-1393">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1393">Added `network nic wait`</span></span>
* <span data-ttu-id="9fb94-1394">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1394">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="9fb94-1395">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1395">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="9fb94-1396">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1396">Resource</span></span>

* <span data-ttu-id="9fb94-1397">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1397">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="9fb94-1398">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1398">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="9fb94-1399">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1399">Added `deployment wait` command</span></span>
* <span data-ttu-id="9fb94-1400">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="9fb94-1400">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1401">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1401">SQL</span></span>

* <span data-ttu-id="9fb94-1402">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1402">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="9fb94-1403">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1403">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="9fb94-1404">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1404">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1405">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1405">Storage</span></span>

* <span data-ttu-id="9fb94-1406">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="9fb94-1406">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1407">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1407">VM</span></span>

* <span data-ttu-id="9fb94-1408">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1408">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="9fb94-1409">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1409">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="9fb94-1410">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1410">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9fb94-1411">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1411">July 3, 2018</span></span>

<span data-ttu-id="9fb94-1412">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="9fb94-1412">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="9fb94-1413">AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1413">AKS</span></span>

* <span data-ttu-id="9fb94-1414">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1414">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9fb94-1415">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1415">July 3, 2018</span></span>

<span data-ttu-id="9fb94-1416">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="9fb94-1416">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1417">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1417">Core</span></span>

* <span data-ttu-id="9fb94-1418">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1418">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1419">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1419">ACR</span></span>

* <span data-ttu-id="9fb94-1420">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="9fb94-1420">Added polling build status</span></span>
* <span data-ttu-id="9fb94-1421">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-1421">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="9fb94-1422">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1422">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1423">ACS</span></span>

* <span data-ttu-id="9fb94-1424">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1424">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="9fb94-1425">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1425">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="9fb94-1426">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1426">Updated options for `aks browse` command.</span></span> <span data-ttu-id="9fb94-1427">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1427">Added `--listen-port` support</span></span>
* <span data-ttu-id="9fb94-1428">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1428">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="9fb94-1429">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="9fb94-1429">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="9fb94-1430">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="9fb94-1430">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1431">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1431">AppService</span></span>

* <span data-ttu-id="9fb94-1432">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1432">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="9fb94-1433">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="9fb94-1433">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="9fb94-1434">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9fb94-1434">Backup</span></span>

* <span data-ttu-id="9fb94-1435">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="9fb94-1435">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-1436">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1436">BatchAI</span></span>

* <span data-ttu-id="9fb94-1437">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1437">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="9fb94-1438">Cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-1438">Cloud</span></span>

* <span data-ttu-id="9fb94-1439">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-1439">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1440">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1440">Container</span></span>

* <span data-ttu-id="9fb94-1441">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="9fb94-1441">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="9fb94-1442">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1442">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="9fb94-1443">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="9fb94-1443">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1444">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1444">Extension</span></span>

* <span data-ttu-id="9fb94-1445">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1445">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1446">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1446">Network</span></span>

* <span data-ttu-id="9fb94-1447">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="9fb94-1447">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1448">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fb94-1448">Rdbms</span></span>

* <span data-ttu-id="9fb94-1449">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1449">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1450">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1450">Resource</span></span>

* <span data-ttu-id="9fb94-1451">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1451">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1452">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1452">VM</span></span>

* <span data-ttu-id="9fb94-1453">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="9fb94-1453">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="9fb94-1454">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1454">June 25, 2018</span></span>

<span data-ttu-id="9fb94-1455">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="9fb94-1455">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="9fb94-1456">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1456">CLI</span></span>

* <span data-ttu-id="9fb94-1457">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1457">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="9fb94-1458">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1458">June 19, 2018</span></span>

<span data-ttu-id="9fb94-1459">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="9fb94-1459">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1460">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1460">Core</span></span>

* <span data-ttu-id="9fb94-1461">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1461">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1462">ACR</span></span>

* <span data-ttu-id="9fb94-1463">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="9fb94-1463">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="9fb94-1464">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1464">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1465">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1465">ACS</span></span>

* <span data-ttu-id="9fb94-1466">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1466">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="9fb94-1467">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1467">Added `--update` support</span></span>
* <span data-ttu-id="9fb94-1468">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1468">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="9fb94-1469">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1469">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="9fb94-1470">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1470">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="9fb94-1471">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1471">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="9fb94-1472">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1472">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="9fb94-1473">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1473">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1474">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1474">AppService</span></span>

* <span data-ttu-id="9fb94-1475">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1475">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="9fb94-1476">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1476">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-1477">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1477">Batch</span></span>

* <span data-ttu-id="9fb94-1478">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1478">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fb94-1479">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1479">Batch AI</span></span>

* <span data-ttu-id="9fb94-1480">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1480">Added support for workspaces.</span></span> <span data-ttu-id="9fb94-1481">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1481">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="9fb94-1482">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1482">Added support for experiments.</span></span> <span data-ttu-id="9fb94-1483">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1483">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="9fb94-1484">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="9fb94-1484">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="9fb94-1485">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1485">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="9fb94-1486">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1486">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="9fb94-1487">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1487">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="9fb94-1488">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-1488">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="9fb94-1489">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="9fb94-1489">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="9fb94-1490">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1490">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="9fb94-1491">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1491">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="9fb94-1492">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1492">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="9fb94-1493">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1493">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="9fb94-1494">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1494">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="9fb94-1495">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1495">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="9fb94-1496">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1496">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="9fb94-1497">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1497">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="9fb94-1498">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1498">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="9fb94-1499">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1499">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9fb94-1500">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1500">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9fb94-1501">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1501">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="9fb94-1502">Cartes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1502">Maps</span></span>

* <span data-ttu-id="9fb94-1503">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1503">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1504">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1504">Network</span></span>

* <span data-ttu-id="9fb94-1505">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1505">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="9fb94-1506">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1506">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="9fb94-1507">#6502</span><span class="sxs-lookup"><span data-stu-id="9fb94-1507">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="9fb94-1508">Réservations</span><span class="sxs-lookup"><span data-stu-id="9fb94-1508">Reservations</span></span>

* <span data-ttu-id="9fb94-1509">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1509">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="9fb94-1510">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1510">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="9fb94-1511">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1511">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="9fb94-1512">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1512">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="9fb94-1513">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1513">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="9fb94-1514">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1514">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1515">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1515">Role</span></span>

* <span data-ttu-id="9fb94-1516">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1516">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1517">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1517">SQL</span></span>

* <span data-ttu-id="9fb94-1518">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1518">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1519">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1519">Storage</span></span>

* <span data-ttu-id="9fb94-1520">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="9fb94-1520">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1521">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1521">VM</span></span>

* <span data-ttu-id="9fb94-1522">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1522">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="9fb94-1523">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1523">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="9fb94-1524">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1524">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9fb94-1525">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1525">June 13, 2018</span></span>

<span data-ttu-id="9fb94-1526">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="9fb94-1526">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1527">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1527">Core</span></span>

* <span data-ttu-id="9fb94-1528">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1528">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9fb94-1529">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1529">June 13, 2018</span></span>

<span data-ttu-id="9fb94-1530">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="9fb94-1530">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="9fb94-1531">AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1531">AKS</span></span>

* <span data-ttu-id="9fb94-1532">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1532">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="9fb94-1533">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb94-1533">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="9fb94-1534">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1534">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="9fb94-1535">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1535">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="9fb94-1536">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1536">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1537">AppService</span></span>

* <span data-ttu-id="9fb94-1538">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="9fb94-1538">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9fb94-1539">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1539">June 5, 2018</span></span>

<span data-ttu-id="9fb94-1540">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="9fb94-1540">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1541">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1541">Interactive</span></span>

* <span data-ttu-id="9fb94-1542">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="9fb94-1542">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9fb94-1543">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1543">June 5, 2018</span></span>

<span data-ttu-id="9fb94-1544">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="9fb94-1544">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1545">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1545">Core</span></span>

* <span data-ttu-id="9fb94-1546">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="9fb94-1546">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="9fb94-1547">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1547">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1548">ACR</span></span>

* <span data-ttu-id="9fb94-1549">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="9fb94-1549">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="9fb94-1550">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1550">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="9fb94-1551">AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1551">AKS</span></span>

* <span data-ttu-id="9fb94-1552">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1552">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-1553">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1553">Batch</span></span>

* <span data-ttu-id="9fb94-1554">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="9fb94-1554">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-1555">IOT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1555">IOT</span></span>

* <span data-ttu-id="9fb94-1556">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="9fb94-1556">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1557">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1557">Network</span></span>

* <span data-ttu-id="9fb94-1558">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="9fb94-1558">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9fb94-1559">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9fb94-1559">Policy Insights</span></span>

* <span data-ttu-id="9fb94-1560">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1560">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="9fb94-1561">ARM</span><span class="sxs-lookup"><span data-stu-id="9fb94-1561">ARM</span></span>

* <span data-ttu-id="9fb94-1562">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1562">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1563">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1563">SQL</span></span>

* <span data-ttu-id="9fb94-1564">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1564">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="9fb94-1565">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1565">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="9fb94-1566">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1566">Storage</span></span>

* <span data-ttu-id="9fb94-1567">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="9fb94-1567">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1568">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1568">VM</span></span>

* <span data-ttu-id="9fb94-1569">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1569">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="9fb94-1570">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1570">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="9fb94-1571">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1571">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="9fb94-1572">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1572">May 22, 2018</span></span>

<span data-ttu-id="9fb94-1573">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="9fb94-1573">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1574">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1574">Core</span></span>

* <span data-ttu-id="9fb94-1575">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="9fb94-1575">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1576">ACS</span></span>

* <span data-ttu-id="9fb94-1577">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1577">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="9fb94-1578">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1578">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1579">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1579">AppService</span></span>

* <span data-ttu-id="9fb94-1580">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="9fb94-1580">Improved generic update commands</span></span>
* <span data-ttu-id="9fb94-1581">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1581">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1582">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1582">Container</span></span>

* <span data-ttu-id="9fb94-1583">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="9fb94-1583">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="9fb94-1584">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1584">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1585">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1585">Extension</span></span>

* <span data-ttu-id="9fb94-1586">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="9fb94-1586">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1587">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1587">Interactive</span></span>

* <span data-ttu-id="9fb94-1588">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1588">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="9fb94-1589">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="9fb94-1589">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-1590">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-1590">KeyVault</span></span>

* <span data-ttu-id="9fb94-1591">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="9fb94-1591">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1592">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1592">Network</span></span>

* <span data-ttu-id="9fb94-1593">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1593">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="9fb94-1594">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1594">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1595">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1595">SQL</span></span>

* <span data-ttu-id="9fb94-1596">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1596">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="9fb94-1597">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1597">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="9fb94-1598">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1598">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="9fb94-1599">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="9fb94-1599">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="9fb94-1600">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1600">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="9fb94-1601">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1601">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="9fb94-1602">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1602">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="9fb94-1603">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1603">`edition`.</span></span> <span data-ttu-id="9fb94-1604">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1604">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="9fb94-1605">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1605">`elasticPoolName`.</span></span> <span data-ttu-id="9fb94-1606">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1606">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="9fb94-1607">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1607">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="9fb94-1608">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1608">`edition`.</span></span> <span data-ttu-id="9fb94-1609">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1609">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="9fb94-1610">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1610">`dtu`.</span></span> <span data-ttu-id="9fb94-1611">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1611">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="9fb94-1612">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1612">`databaseDtuMin`.</span></span> <span data-ttu-id="9fb94-1613">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1613">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="9fb94-1614">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1614">`databaseDtuMax`.</span></span> <span data-ttu-id="9fb94-1615">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1615">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="9fb94-1616">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1616">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="9fb94-1617">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1617">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1618">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1618">Storage</span></span>

* <span data-ttu-id="9fb94-1619">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1619">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="9fb94-1620">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1620">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1621">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1621">VM</span></span>

* <span data-ttu-id="9fb94-1622">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1622">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="9fb94-1623">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1623">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="9fb94-1624">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1624">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="9fb94-1625">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1625">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="9fb94-1626">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1626">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="9fb94-1627">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1627">May 7, 2018</span></span>

<span data-ttu-id="9fb94-1628">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="9fb94-1628">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1629">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1629">Core</span></span>

* <span data-ttu-id="9fb94-1630">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="9fb94-1630">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="9fb94-1631">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="9fb94-1631">Added limited support for positional arguments</span></span>
* <span data-ttu-id="9fb94-1632">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1632">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="9fb94-1633">#5591</span><span class="sxs-lookup"><span data-stu-id="9fb94-1633">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="9fb94-1634">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1634">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="9fb94-1635">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="9fb94-1635">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="9fb94-1636">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1636">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="9fb94-1637">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1637">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="9fb94-1638">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1638">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1639">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1639">ACR</span></span>

* <span data-ttu-id="9fb94-1640">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1640">Added ACR Build commands</span></span>
* <span data-ttu-id="9fb94-1641">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="9fb94-1641">Improved resource not found error messages</span></span>
* <span data-ttu-id="9fb94-1642">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1642">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="9fb94-1643">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1643">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="9fb94-1644">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="9fb94-1644">Improved repository commands error messages</span></span>
* <span data-ttu-id="9fb94-1645">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1645">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1646">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1646">ACS</span></span>

* <span data-ttu-id="9fb94-1647">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-1647">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="9fb94-1648">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="9fb94-1648">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="9fb94-1649">AMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1649">AMS</span></span>

* <span data-ttu-id="9fb94-1650">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1650">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1651">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1651">Appservice</span></span>

* <span data-ttu-id="9fb94-1652">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="9fb94-1652">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="9fb94-1653">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1653">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="9fb94-1654">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="9fb94-1654">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="9fb94-1655">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1655">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fb94-1656">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1656">Batch AI</span></span>

* <span data-ttu-id="9fb94-1657">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="9fb94-1657">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fb94-1658">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1658">Cognitive Services</span></span>

* <span data-ttu-id="9fb94-1659">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1659">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-1660">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1660">Consumption</span></span>

* <span data-ttu-id="9fb94-1661">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="9fb94-1661">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1662">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1662">Container</span></span>

* <span data-ttu-id="9fb94-1663">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="9fb94-1663">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fb94-1664">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-1664">Cosmos DB</span></span>

* <span data-ttu-id="9fb94-1665">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fb94-1665">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="9fb94-1666">DMS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1666">DMS</span></span>

* <span data-ttu-id="9fb94-1667">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="9fb94-1667">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1668">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1668">Extension</span></span>

* <span data-ttu-id="9fb94-1669">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1669">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1670">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1670">Interactive</span></span>

* <span data-ttu-id="9fb94-1671">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="9fb94-1671">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="9fb94-1672">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="9fb94-1672">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="9fb94-1673">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1673">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="9fb94-1674">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1674">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="9fb94-1675">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-1675">Lab</span></span>

* <span data-ttu-id="9fb94-1676">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="9fb94-1676">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1677">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1677">Network</span></span>

* <span data-ttu-id="9fb94-1678">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1678">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="9fb94-1679">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1679">Profile</span></span>

* <span data-ttu-id="9fb94-1680">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1680">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="9fb94-1681">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1681">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="9fb94-1682">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1682">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="9fb94-1683">Redis</span><span class="sxs-lookup"><span data-stu-id="9fb94-1683">Redis</span></span>

* <span data-ttu-id="9fb94-1684">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1684">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="9fb94-1685">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1685">Deprecated `redis list-all`.</span></span> <span data-ttu-id="9fb94-1686">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1686">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="9fb94-1687">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1687">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="9fb94-1688">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1688">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1689">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1689">Role</span></span>

* <span data-ttu-id="9fb94-1690">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1690">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1691">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1691">Storage</span></span>

* <span data-ttu-id="9fb94-1692">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1692">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="9fb94-1693">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="9fb94-1693">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="9fb94-1694">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1694">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="9fb94-1695">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1695">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="9fb94-1696">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1696">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1697">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1697">VM</span></span>

* <span data-ttu-id="9fb94-1698">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1698">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="9fb94-1699">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1699">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="9fb94-1700">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1700">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="9fb94-1701">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1701">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="9fb94-1702">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1702">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="9fb94-1703">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="9fb94-1703">Added write accelerator support</span></span>
* <span data-ttu-id="9fb94-1704">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1704">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="9fb94-1705">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1705">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="9fb94-1706">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="9fb94-1706">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="9fb94-1707">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1707">April 10, 2018</span></span>

<span data-ttu-id="9fb94-1708">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="9fb94-1708">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1709">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1709">ACR</span></span>

* <span data-ttu-id="9fb94-1710">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="9fb94-1710">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1711">ACS</span></span>

* <span data-ttu-id="9fb94-1712">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="9fb94-1712">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1713">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1713">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="9fb94-1715">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="9fb94-1715">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-1716">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1716">BatchAI</span></span>

* <span data-ttu-id="9fb94-1717">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="9fb94-1717">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="9fb94-1718">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-1718">Job level mounting</span></span>
  - <span data-ttu-id="9fb94-1719">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="9fb94-1719">Environment variables with secret values</span></span>
  - <span data-ttu-id="9fb94-1720">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="9fb94-1720">Performance counters settings</span></span>
  - <span data-ttu-id="9fb94-1721">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-1721">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="9fb94-1722">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="9fb94-1722">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="9fb94-1723">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="9fb94-1723">Usage and limits reporting</span></span>
  - <span data-ttu-id="9fb94-1724">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1724">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="9fb94-1725">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1725">Support for custom images</span></span>
  - <span data-ttu-id="9fb94-1726">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="9fb94-1726">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="9fb94-1727">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-1727">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="9fb94-1728">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="9fb94-1728">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="9fb94-1729">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="9fb94-1729">National clouds are supported</span></span>
* <span data-ttu-id="9fb94-1730">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="9fb94-1730">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="9fb94-1731">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1731">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="9fb94-1732">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1732">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="9fb94-1733">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1733">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="9fb94-1734">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1734">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="9fb94-1735">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1735">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="9fb94-1736">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1736">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="9fb94-1737">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1737">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="9fb94-1738">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="9fb94-1738">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="9fb94-1739">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1739">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="9fb94-1740">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1740">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="9fb94-1741">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1741">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="9fb94-1742">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1742">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="9fb94-1743">Facturation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1743">Billing</span></span>

* <span data-ttu-id="9fb94-1744">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="9fb94-1744">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-1745">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1745">Consumption</span></span>

* <span data-ttu-id="9fb94-1746">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1746">Added `marketplace` commands</span></span>
* <span data-ttu-id="9fb94-1747">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1747">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="9fb94-1748">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1748">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="9fb94-1749">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1749">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="9fb94-1750">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1750">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="9fb94-1751">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1751">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1752">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1752">Container</span></span>

* <span data-ttu-id="9fb94-1753">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1753">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="9fb94-1754">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="9fb94-1754">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1755">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1755">Extension</span></span>

* <span data-ttu-id="9fb94-1756">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1756">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1757">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1757">Interactive</span></span>

* <span data-ttu-id="9fb94-1758">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="9fb94-1758">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="9fb94-1759">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1759">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="9fb94-1760">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1760">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1761">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1761">Network</span></span>

* <span data-ttu-id="9fb94-1762">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="9fb94-1762">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="9fb94-1763">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1763">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="9fb94-1764">#4910</span><span class="sxs-lookup"><span data-stu-id="9fb94-1764">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="9fb94-1765">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1765">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="9fb94-1766">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1766">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="9fb94-1767">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1767">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="9fb94-1768">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1768">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="9fb94-1769">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1769">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-1770">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1770">Profile</span></span>

* <span data-ttu-id="9fb94-1771">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1771">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="9fb94-1772">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1772">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1773">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1773">RDBMS</span></span>

* <span data-ttu-id="9fb94-1774">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1774">Added `georestore` command</span></span>
* <span data-ttu-id="9fb94-1775">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1775">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1776">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1776">Resource</span></span>

* <span data-ttu-id="9fb94-1777">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1777">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="9fb94-1778">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1778">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1779">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1779">SQL</span></span>

* <span data-ttu-id="9fb94-1780">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1780">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1781">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1781">Storage</span></span>

* <span data-ttu-id="9fb94-1782">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1782">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1783">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1783">VM</span></span>

* <span data-ttu-id="9fb94-1784">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1784">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="9fb94-1785">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1785">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="9fb94-1787">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1787">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="9fb94-1788">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1788">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="9fb94-1789">#5718</span><span class="sxs-lookup"><span data-stu-id="9fb94-1789">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="9fb94-1790">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="9fb94-1790">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="9fb94-1791">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1791">March 27, 2018</span></span>

<span data-ttu-id="9fb94-1792">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="9fb94-1792">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1793">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1793">Core</span></span>

* <span data-ttu-id="9fb94-1794">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1794">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1795">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1795">ACS</span></span>

* <span data-ttu-id="9fb94-1796">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fb94-1796">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1797">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1797">Appservice</span></span>

* <span data-ttu-id="9fb94-1798">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1798">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="9fb94-1799">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1799">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9fb94-1800">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9fb94-1800">Backup</span></span>

* <span data-ttu-id="9fb94-1801">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1801">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="9fb94-1802">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1802">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="9fb94-1803">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1803">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="9fb94-1804">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1804">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1805">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1805">Container</span></span>

* <span data-ttu-id="9fb94-1806">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1806">Added `container exec` command.</span></span> <span data-ttu-id="9fb94-1807">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1807">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="9fb94-1808">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1808">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1809">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1809">Extension</span></span>

* <span data-ttu-id="9fb94-1810">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-1810">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="9fb94-1811">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1811">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="9fb94-1812">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1812">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1813">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1813">Interactive</span></span>

* <span data-ttu-id="9fb94-1814">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-1814">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="9fb94-1815">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1815">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="9fb94-1816">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="9fb94-1816">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="9fb94-1817">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="9fb94-1817">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="9fb94-1818">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-1818">Lab</span></span>

* <span data-ttu-id="9fb94-1819">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1819">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1820">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1820">Monitor</span></span>

* <span data-ttu-id="9fb94-1821">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1821">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="9fb94-1822">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="9fb94-1822">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="9fb94-1823">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1823">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1824">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1824">Network</span></span>

* <span data-ttu-id="9fb94-1825">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1825">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-1826">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1826">Profile</span></span>

* <span data-ttu-id="9fb94-1827">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1827">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1828">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1828">RDBMS</span></span>

* <span data-ttu-id="9fb94-1829">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="9fb94-1829">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1830">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1830">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="9fb94-1832">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1832">Role</span></span>

* <span data-ttu-id="9fb94-1833">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1833">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="9fb94-1834">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="9fb94-1834">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="9fb94-1835">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1835">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="9fb94-1836">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1836">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="9fb94-1837">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1837">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1838">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1838">Storage</span></span>

* <span data-ttu-id="9fb94-1839">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="9fb94-1839">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="9fb94-1840">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="9fb94-1840">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1841">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1841">VM</span></span>

* <span data-ttu-id="9fb94-1842">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="9fb94-1842">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="9fb94-1843">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1843">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="9fb94-1844">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1844">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="9fb94-1845">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1845">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="9fb94-1846">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1846">March 13, 2018</span></span>

<span data-ttu-id="9fb94-1847">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="9fb94-1847">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-1848">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1848">ACR</span></span>

* <span data-ttu-id="9fb94-1849">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1849">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="9fb94-1850">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1850">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="9fb94-1851">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="9fb94-1851">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1852">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1852">ACS</span></span>

* <span data-ttu-id="9fb94-1853">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="9fb94-1853">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="9fb94-1854">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="9fb94-1854">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="9fb94-1855">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fb94-1855">Advisor</span></span>

* <span data-ttu-id="9fb94-1856">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1856">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="9fb94-1857">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1857">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="9fb94-1858">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1858">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="9fb94-1859">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1859">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="9fb94-1860">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1860">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1861">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1861">Appservice</span></span>

* <span data-ttu-id="9fb94-1862">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="9fb94-1862">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="9fb94-1863">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1863">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fb94-1864">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1864">Eventhubs</span></span>

* <span data-ttu-id="9fb94-1865">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1865">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1866">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1866">Extension</span></span>

* <span data-ttu-id="9fb94-1867">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-1867">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1868">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1868">Interactive</span></span>

* <span data-ttu-id="9fb94-1869">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="9fb94-1869">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="9fb94-1870">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="9fb94-1870">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="9fb94-1871">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="9fb94-1871">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="9fb94-1872">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="9fb94-1872">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1873">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1873">Monitor</span></span>

* <span data-ttu-id="9fb94-1874">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1874">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="9fb94-1875">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1875">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="9fb94-1876">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1876">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="9fb94-1877">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1877">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1878">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1878">Network</span></span>

* <span data-ttu-id="9fb94-1879">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1879">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="9fb94-1880">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1880">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="9fb94-1881">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1881">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="9fb94-1882">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1882">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-1883">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1883">Profile</span></span>

* <span data-ttu-id="9fb94-1884">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1884">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="9fb94-1885">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1885">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-1886">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-1886">RDBMS</span></span>

* <span data-ttu-id="9fb94-1887">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-1887">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fb94-1888">Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fb94-1888">Service Bus</span></span>

* <span data-ttu-id="9fb94-1889">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-1889">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1890">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1890">Storage</span></span>

* <span data-ttu-id="9fb94-1891">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="9fb94-1891">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="9fb94-1892">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="9fb94-1892">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1893">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1893">VM</span></span>

* <span data-ttu-id="9fb94-1894">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="9fb94-1894">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="9fb94-1895">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="9fb94-1895">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="9fb94-1896">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1896">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="9fb94-1897">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="9fb94-1897">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="9fb94-1898">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1898">February 27, 2018</span></span>

<span data-ttu-id="9fb94-1899">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="9fb94-1899">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1900">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1900">Core</span></span>

* <span data-ttu-id="9fb94-1901">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="9fb94-1901">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="9fb94-1902">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="9fb94-1902">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="9fb94-1903">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1903">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1904">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1904">ACS</span></span>

* <span data-ttu-id="9fb94-1905">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-1905">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="9fb94-1906">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1906">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="9fb94-1907">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1907">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="9fb94-1908">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1908">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1909">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1909">Appservice</span></span>

* <span data-ttu-id="9fb94-1910">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="9fb94-1910">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="9fb94-1911">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="9fb94-1911">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fb94-1912">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1912">Cognitive Services</span></span>

* <span data-ttu-id="9fb94-1913">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-1913">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-1914">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1914">Consumption</span></span>

* <span data-ttu-id="9fb94-1915">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="9fb94-1915">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="9fb94-1916">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="9fb94-1916">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1917">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1917">Container</span></span>

* <span data-ttu-id="9fb94-1918">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1918">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1919">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1919">Network</span></span>

* <span data-ttu-id="9fb94-1920">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1920">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1921">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1921">Resource</span></span>

* <span data-ttu-id="9fb94-1922">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="9fb94-1922">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1923">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1923">Role</span></span>

* <span data-ttu-id="9fb94-1924">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="9fb94-1924">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1925">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1925">SQL</span></span>

* <span data-ttu-id="9fb94-1926">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="9fb94-1926">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1927">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1927">Storage</span></span>

* <span data-ttu-id="9fb94-1928">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1928">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1929">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1929">VM</span></span>

* <span data-ttu-id="9fb94-1930">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="9fb94-1930">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="9fb94-1931">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1931">February 13, 2018</span></span>

<span data-ttu-id="9fb94-1932">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="9fb94-1932">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1933">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1933">Core</span></span>

* <span data-ttu-id="9fb94-1934">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1934">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1935">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1935">ACS</span></span>

* <span data-ttu-id="9fb94-1936">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="9fb94-1936">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="9fb94-1937">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1937">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="9fb94-1938">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1938">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="9fb94-1939">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1939">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="9fb94-1940">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="9fb94-1940">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="9fb94-1941">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1941">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="9fb94-1942">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fb94-1942">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="9fb94-1943">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1943">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1944">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1944">Appservice</span></span>

* <span data-ttu-id="9fb94-1945">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="9fb94-1945">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="9fb94-1946">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1946">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-1947">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-1947">CDN</span></span>

* <span data-ttu-id="9fb94-1948">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1948">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-1949">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1949">Container</span></span>

* <span data-ttu-id="9fb94-1950">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="9fb94-1950">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="9fb94-1951">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-1951">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-1952">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-1952">CosmosDB</span></span>

* <span data-ttu-id="9fb94-1953">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="9fb94-1953">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-1954">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-1954">Extension</span></span>

* <span data-ttu-id="9fb94-1955">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1955">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="9fb94-1956">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1956">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="9fb94-1957">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9fb94-1957">Feedback</span></span>

* <span data-ttu-id="9fb94-1958">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="9fb94-1958">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-1959">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-1959">Interactive</span></span>

* <span data-ttu-id="9fb94-1960">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fb94-1960">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="9fb94-1961">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="9fb94-1961">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-1962">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-1962">IoT</span></span>

* <span data-ttu-id="9fb94-1963">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9fb94-1963">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9fb94-1964">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="9fb94-1964">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9fb94-1965">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1965">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="9fb94-1966">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="9fb94-1966">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-1967">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-1967">Monitor</span></span>

* <span data-ttu-id="9fb94-1968">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1968">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-1969">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-1969">Network</span></span>

* <span data-ttu-id="9fb94-1970">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="9fb94-1970">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="9fb94-1971">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-1971">Profile</span></span>

* <span data-ttu-id="9fb94-1972">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="9fb94-1972">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-1973">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-1973">Resource</span></span>

* <span data-ttu-id="9fb94-1974">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1974">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-1975">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-1975">Role</span></span>

* <span data-ttu-id="9fb94-1976">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1976">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-1977">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-1977">SQL</span></span>

* <span data-ttu-id="9fb94-1978">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1978">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="9fb94-1979">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1979">Added `sql db rename`</span></span>
* <span data-ttu-id="9fb94-1980">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="9fb94-1980">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-1981">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-1981">Storage</span></span>

* <span data-ttu-id="9fb94-1982">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="9fb94-1982">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-1983">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-1983">VM</span></span>

* <span data-ttu-id="9fb94-1984">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="9fb94-1984">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="9fb94-1985">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1985">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="9fb94-1986">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="9fb94-1986">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="9fb94-1987">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-1987">January 31, 2018</span></span>

<span data-ttu-id="9fb94-1988">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="9fb94-1988">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-1989">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-1989">Core</span></span>

* <span data-ttu-id="9fb94-1990">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="9fb94-1990">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="9fb94-1991">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-1991">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="9fb94-1992">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="9fb94-1992">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="9fb94-1993">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="9fb94-1993">Use `--verbose` to see</span></span>
* <span data-ttu-id="9fb94-1994">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="9fb94-1994">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-1995">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-1995">ACS</span></span>

* <span data-ttu-id="9fb94-1996">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1996">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="9fb94-1997">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="9fb94-1997">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-1998">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-1998">Appservice</span></span>

* <span data-ttu-id="9fb94-1999">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="9fb94-1999">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="9fb94-2000">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="9fb94-2000">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-2001">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2001">CDN</span></span>

* <span data-ttu-id="9fb94-2002">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2002">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-2003">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-2003">CosmosDB</span></span>

* <span data-ttu-id="9fb94-2004">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2004">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-2005">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-2005">Interactive</span></span>

* <span data-ttu-id="9fb94-2006">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="9fb94-2006">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2007">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2007">Network</span></span>

* <span data-ttu-id="9fb94-2008">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2008">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="9fb94-2009">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2009">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="9fb94-2010">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2010">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="9fb94-2011">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2011">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="9fb94-2012">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2012">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="9fb94-2013">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2013">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="9fb94-2014">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2014">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="9fb94-2015">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2015">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="9fb94-2016">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2016">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="9fb94-2017">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2017">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2018">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2018">Profile</span></span>

* <span data-ttu-id="9fb94-2019">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="9fb94-2019">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2020">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2020">Resource</span></span>

* <span data-ttu-id="9fb94-2021">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="9fb94-2021">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2022">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2022">Storage</span></span>

* <span data-ttu-id="9fb94-2023">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="9fb94-2023">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="9fb94-2024">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2024">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="9fb94-2025">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2025">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="9fb94-2026">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2026">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="9fb94-2027">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="9fb94-2027">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2028">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2028">VM</span></span>

* <span data-ttu-id="9fb94-2029">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="9fb94-2029">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="9fb94-2030">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2030">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="9fb94-2031">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="9fb94-2031">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="9fb94-2032">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2032">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="9fb94-2033">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="9fb94-2033">January 17, 2018</span></span>

<span data-ttu-id="9fb94-2034">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="9fb94-2034">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-2035">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2035">ACR</span></span>

* <span data-ttu-id="9fb94-2036">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-2036">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="9fb94-2037">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="9fb94-2037">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2038">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2038">ACS</span></span>

* <span data-ttu-id="9fb94-2039">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2039">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="9fb94-2040">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2040">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2041">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2041">Appservice</span></span>

* <span data-ttu-id="9fb94-2042">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="9fb94-2042">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="9fb94-2043">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2043">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="9fb94-2044">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2044">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="9fb94-2045">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9fb94-2045">Backup</span></span>

* <span data-ttu-id="9fb94-2046">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="9fb94-2046">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="9fb94-2047">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2047">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="9fb94-2048">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-2048">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="9fb94-2049">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="9fb94-2049">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="9fb94-2050">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2050">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-2051">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2051">Batch</span></span>

* <span data-ttu-id="9fb94-2052">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="9fb94-2052">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="9fb94-2053">Cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-2053">Cloud</span></span>

* <span data-ttu-id="9fb94-2054">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-2054">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-2055">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2055">Consumption</span></span>

* <span data-ttu-id="9fb94-2056">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2056">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fb94-2057">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fb94-2057">Event Grid</span></span>

* <span data-ttu-id="9fb94-2058">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2058">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9fb94-2059">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2059">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9fb94-2060">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2060">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="9fb94-2061">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="9fb94-2061">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="9fb94-2062">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2062">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="9fb94-2063">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2063">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="9fb94-2064">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2064">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="9fb94-2065">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="9fb94-2065">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-2066">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-2066">Interactive</span></span>

* <span data-ttu-id="9fb94-2067">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="9fb94-2067">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="9fb94-2068">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2068">Fixed errors on startup</span></span>
* <span data-ttu-id="9fb94-2069">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="9fb94-2069">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-2070">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-2070">IoT</span></span>

* <span data-ttu-id="9fb94-2071">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="9fb94-2071">Added support for device provisioning service</span></span>
* <span data-ttu-id="9fb94-2072">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2072">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="9fb94-2073">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-2073">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2074">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2074">Monitor</span></span>

* <span data-ttu-id="9fb94-2075">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2075">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="9fb94-2076">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2076">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="9fb94-2077">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="9fb94-2077">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2078">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2078">Network</span></span>

* <span data-ttu-id="9fb94-2079">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2079">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="9fb94-2080">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2080">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2081">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2081">Profile</span></span>

* <span data-ttu-id="9fb94-2082">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-2082">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-2083">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-2083">Role</span></span>

* <span data-ttu-id="9fb94-2084">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="9fb94-2084">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fb94-2085">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-2085">Service Fabric</span></span>

* <span data-ttu-id="9fb94-2086">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="9fb94-2086">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="9fb94-2087">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2087">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2088">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2088">VM</span></span>

* <span data-ttu-id="9fb94-2089">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2089">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="9fb94-2090">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2090">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="9fb94-2091">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="9fb94-2091">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="9fb94-2092">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2092">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="9fb94-2093">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="9fb94-2093">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="9fb94-2094">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2094">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fb94-2095">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2095">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fb94-2096">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2096">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="9fb94-2097">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2097">December 19, 2017</span></span>

<span data-ttu-id="9fb94-2098">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="9fb94-2098">Version 2.0.23</span></span>

* <span data-ttu-id="9fb94-2099">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-2099">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-2100">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2100">Container</span></span>

* <span data-ttu-id="9fb94-2101">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2101">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2102">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2102">Network</span></span>

* <span data-ttu-id="9fb94-2103">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2103">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="9fb94-2104">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2104">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2105">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2105">Storage</span></span>

* <span data-ttu-id="9fb94-2106">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="9fb94-2106">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2107">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2107">VM</span></span>

* <span data-ttu-id="9fb94-2108">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2108">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="9fb94-2109">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2109">December 5, 2017</span></span>

<span data-ttu-id="9fb94-2110">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="9fb94-2110">Version 2.0.22</span></span>

* <span data-ttu-id="9fb94-2111">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2111">Removed `az component` commands.</span></span> <span data-ttu-id="9fb94-2112">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="9fb94-2112">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-2113">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2113">Core</span></span>
* <span data-ttu-id="9fb94-2114">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="9fb94-2114">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="9fb94-2115">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="9fb94-2115">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2116">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2116">ACS</span></span>

* <span data-ttu-id="9fb94-2117">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2117">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="9fb94-2118">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2118">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="9fb94-2119">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="9fb94-2119">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="9fb94-2120">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fb94-2120">Advisor</span></span>

* <span data-ttu-id="9fb94-2121">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-2121">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2122">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2122">Appservice</span></span>

* <span data-ttu-id="9fb94-2123">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2123">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="9fb94-2124">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2124">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="9fb94-2125">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2125">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="9fb94-2126">Consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2126">Consumption</span></span>

* <span data-ttu-id="9fb94-2127">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="9fb94-2127">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-2128">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2128">Container</span></span>

* <span data-ttu-id="9fb94-2129">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2129">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2130">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2130">Monitor</span></span>

* <span data-ttu-id="9fb94-2131">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="9fb94-2131">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2132">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2132">Resource</span></span>

* <span data-ttu-id="9fb94-2133">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2133">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-2134">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-2134">Role</span></span>

* <span data-ttu-id="9fb94-2135">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2135">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="9fb94-2136">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2136">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="9fb94-2137">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2137">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2138">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2138">SQL</span></span>

* <span data-ttu-id="9fb94-2139">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2139">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="9fb94-2140">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2140">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2141">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2141">VM</span></span>

* <span data-ttu-id="9fb94-2142">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2142">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="9fb94-2143">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2143">November 14, 2017</span></span>

<span data-ttu-id="9fb94-2144">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="9fb94-2144">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-2145">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2145">ACR</span></span>

* <span data-ttu-id="9fb94-2146">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="9fb94-2146">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="9fb94-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2147">ACS</span></span>

* <span data-ttu-id="9fb94-2148">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2148">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="9fb94-2149">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2149">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="9fb94-2150">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2150">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="9fb94-2151">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-2151">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="9fb94-2152">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="9fb94-2152">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2153">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2153">Appservice</span></span>

* <span data-ttu-id="9fb94-2154">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="9fb94-2154">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="9fb94-2155">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2155">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="9fb94-2156">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2156">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="9fb94-2157">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2157">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="9fb94-2158">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="9fb94-2158">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="9fb94-2159">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2159">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-2160">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2160">Batch</span></span>

* <span data-ttu-id="9fb94-2161">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2161">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-2162">Batchai</span><span class="sxs-lookup"><span data-stu-id="9fb94-2162">Batchai</span></span>

* <span data-ttu-id="9fb94-2163">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2163">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="9fb94-2164">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2164">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="9fb94-2165">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2165">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="9fb94-2166">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2166">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="9fb94-2167">Cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-2167">Cloud</span></span>

* <span data-ttu-id="9fb94-2168">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="9fb94-2168">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-2169">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2169">Container</span></span>

* <span data-ttu-id="9fb94-2170">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="9fb94-2170">Added support to open multiple ports</span></span>
* <span data-ttu-id="9fb94-2171">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="9fb94-2171">Added container group restart policy</span></span>
* <span data-ttu-id="9fb94-2172">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="9fb94-2172">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="9fb94-2173">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="9fb94-2173">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fb94-2174">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-2174">Data Lake Analytics</span></span>

* <span data-ttu-id="9fb94-2175">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="9fb94-2175">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fb94-2176">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2176">Data Lake Store</span></span>

* <span data-ttu-id="9fb94-2177">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="9fb94-2177">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-2178">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-2178">Extension</span></span>

* <span data-ttu-id="9fb94-2179">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="9fb94-2179">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="9fb94-2180">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="9fb94-2180">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-2181">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-2181">IoT</span></span>

* <span data-ttu-id="9fb94-2182">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2182">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2183">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2183">Monitor</span></span>

* <span data-ttu-id="9fb94-2184">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2184">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2185">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2185">Network</span></span>

* <span data-ttu-id="9fb94-2186">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="9fb94-2186">Added support for CAA DNS records</span></span>
* <span data-ttu-id="9fb94-2187">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2187">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="9fb94-2188">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-2188">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="9fb94-2189">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2189">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="9fb94-2190">Réservations</span><span class="sxs-lookup"><span data-stu-id="9fb94-2190">Reservations</span></span>

* <span data-ttu-id="9fb94-2191">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-2191">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2192">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2192">Resource</span></span>

* <span data-ttu-id="9fb94-2193">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="9fb94-2193">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2194">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2194">SQL</span></span>

* <span data-ttu-id="9fb94-2195">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2195">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2196">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2196">Storage</span></span>

* <span data-ttu-id="9fb94-2197">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2197">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="9fb94-2198">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="9fb94-2198">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="9fb94-2199">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2199">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="9fb94-2200">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2200">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="9fb94-2201">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2201">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="9fb94-2202">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2202">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="9fb94-2203">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2203">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2204">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2204">VM</span></span>

* <span data-ttu-id="9fb94-2205">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2205">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="9fb94-2206">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2206">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="9fb94-2207">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="9fb94-2207">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="9fb94-2208">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2208">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="9fb94-2209">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2209">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="9fb94-2210">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2210">October 24, 2017</span></span>

<span data-ttu-id="9fb94-2211">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="9fb94-2211">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-2212">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2212">Core</span></span>

* <span data-ttu-id="9fb94-2213">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2213">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-2214">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2214">ACR</span></span>

* <span data-ttu-id="9fb94-2215">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2215">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="9fb94-2216">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="9fb94-2216">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="9fb94-2217">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="9fb94-2217">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2218">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2218">ACS</span></span>

* <span data-ttu-id="9fb94-2219">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2219">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="9fb94-2220">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2220">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2221">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2221">Appservice</span></span>

* <span data-ttu-id="9fb94-2222">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="9fb94-2222">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="9fb94-2223">Composant</span><span class="sxs-lookup"><span data-stu-id="9fb94-2223">Component</span></span>

* <span data-ttu-id="9fb94-2224">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2224">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2225">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2225">Monitor</span></span>

* <span data-ttu-id="9fb94-2226">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2226">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2227">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2227">Resource</span></span>

* <span data-ttu-id="9fb94-2228">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2228">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="9fb94-2229">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="9fb94-2229">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2230">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2230">VM</span></span>

* <span data-ttu-id="9fb94-2231">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2231">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="9fb94-2232">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2232">October 9, 2017</span></span>

<span data-ttu-id="9fb94-2233">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="9fb94-2233">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-2234">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2234">Core</span></span>

* <span data-ttu-id="9fb94-2235">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fb94-2235">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2236">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2236">Appservice</span></span>

* <span data-ttu-id="9fb94-2237">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2237">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-2238">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2238">Batch</span></span>

* <span data-ttu-id="9fb94-2239">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="9fb94-2239">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="9fb94-2240">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="9fb94-2240">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="9fb94-2241">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2241">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="9fb94-2242">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="9fb94-2242">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="9fb94-2243">Batchai</span><span class="sxs-lookup"><span data-stu-id="9fb94-2243">Batchai</span></span>

* <span data-ttu-id="9fb94-2244">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fb94-2244">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-2245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-2245">Keyvault</span></span>

* <span data-ttu-id="9fb94-2246">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2246">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="9fb94-2247">(#4448)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2247">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="9fb94-2248">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2248">Network</span></span>

* <span data-ttu-id="9fb94-2249">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="9fb94-2249">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="9fb94-2250">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2250">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2251">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2251">Resource</span></span>

* <span data-ttu-id="9fb94-2252">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2252">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="9fb94-2253">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2253">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="9fb94-2254">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2254">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="9fb94-2255">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="9fb94-2255">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2256">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2256">Sql</span></span>

* <span data-ttu-id="9fb94-2257">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="9fb94-2257">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="9fb94-2258">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="9fb94-2258">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="9fb94-2259">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="9fb94-2259">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2260">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2260">Storage</span></span>

* <span data-ttu-id="9fb94-2261">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="9fb94-2261">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2262">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2262">Vm</span></span>

* <span data-ttu-id="9fb94-2263">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2263">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="9fb94-2264">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2264">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="9fb94-2265">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2265">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="9fb94-2266">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2266">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="9fb94-2267">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2267">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="9fb94-2268">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2268">September 22, 2017</span></span>

<span data-ttu-id="9fb94-2269">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="9fb94-2269">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2270">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2270">Resource</span></span>

* <span data-ttu-id="9fb94-2271">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2271">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="9fb94-2272">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="9fb94-2272">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="9fb94-2273">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2273">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="9fb94-2274">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2274">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2275">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2275">Network</span></span>

* <span data-ttu-id="9fb94-2276">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2276">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="9fb94-2277">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2277">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="9fb94-2278">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2278">Added `asg` application security group commands</span></span>
* <span data-ttu-id="9fb94-2279">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2279">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="9fb94-2280">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2280">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9fb94-2281">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2281">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="9fb94-2282">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2282">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2283">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2283">Storage</span></span>

* <span data-ttu-id="9fb94-2284">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2284">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fb94-2285">Événement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2285">Eventgrid</span></span>

* <span data-ttu-id="9fb94-2286">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2286">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2287">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2287">SQL</span></span>

* <span data-ttu-id="9fb94-2288">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2288">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="9fb94-2289">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2289">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="9fb94-2290">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2290">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-2291">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-2291">Keyvault</span></span>

* <span data-ttu-id="9fb94-2292">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="9fb94-2292">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2293">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2293">VM</span></span>

* <span data-ttu-id="9fb94-2294">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2294">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="9fb94-2295">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="9fb94-2295">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="9fb94-2296">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2296">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="9fb94-2297">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2297">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="9fb94-2298">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2298">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="9fb94-2299">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2299">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2300">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2300">ACS</span></span>

* <span data-ttu-id="9fb94-2301">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-2301">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2302">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2302">Appservice</span></span>

* <span data-ttu-id="9fb94-2303">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2303">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9fb94-2304">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="9fb94-2304">Backup</span></span>

* <span data-ttu-id="9fb94-2305">Préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-2305">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="9fb94-2306">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2306">September 11, 2017</span></span>

<span data-ttu-id="9fb94-2307">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="9fb94-2307">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="9fb94-2308">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2308">Core</span></span>

* <span data-ttu-id="9fb94-2309">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="9fb94-2309">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="9fb94-2310">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="9fb94-2310">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2311">Acs</span><span class="sxs-lookup"><span data-stu-id="9fb94-2311">Acs</span></span>

* <span data-ttu-id="9fb94-2312">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2312">Added `acs list-locations` command</span></span>
* <span data-ttu-id="9fb94-2313">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="9fb94-2313">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2314">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2314">Appservice</span></span>

* <span data-ttu-id="9fb94-2315">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="9fb94-2315">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-2316">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2316">CDN</span></span>

* <span data-ttu-id="9fb94-2317">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2317">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="9fb94-2318">Extension</span><span class="sxs-lookup"><span data-stu-id="9fb94-2318">Extension</span></span>

* <span data-ttu-id="9fb94-2319">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-2319">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-2320">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-2320">Keyvault</span></span>

* <span data-ttu-id="9fb94-2321">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2321">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2322">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2322">Network</span></span>

* <span data-ttu-id="9fb94-2323">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2323">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9fb94-2324">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2324">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="9fb94-2325">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2325">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="9fb94-2326">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2326">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9fb94-2327">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2327">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2328">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2328">Resource</span></span>

* <span data-ttu-id="9fb94-2329">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2329">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="9fb94-2330">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2330">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="9fb94-2331">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="9fb94-2331">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="9fb94-2332">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="9fb94-2332">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2333">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2333">SQL</span></span>

* <span data-ttu-id="9fb94-2334">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2334">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2335">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2335">VM</span></span>

* <span data-ttu-id="9fb94-2336">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="9fb94-2336">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="9fb94-2337">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="9fb94-2337">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="9fb94-2338">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2338">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="9fb94-2339">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="9fb94-2339">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="9fb94-2340">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="9fb94-2340">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="9fb94-2341">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2341">August 31, 2017</span></span>

<span data-ttu-id="9fb94-2342">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="9fb94-2342">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-2343">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-2343">Keyvault</span></span>

* <span data-ttu-id="9fb94-2344">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2344">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="9fb94-2345">Sf</span><span class="sxs-lookup"><span data-stu-id="9fb94-2345">Sf</span></span>

* <span data-ttu-id="9fb94-2346">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2346">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2347">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2347">Storage</span></span>

* <span data-ttu-id="9fb94-2348">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="9fb94-2348">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="9fb94-2349">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2349">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="9fb94-2350">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2350">August 28, 2017</span></span>

<span data-ttu-id="9fb94-2351">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="9fb94-2351">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="9fb94-2352">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-2352">CLI</span></span>

* <span data-ttu-id="9fb94-2353">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2353">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2354">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2354">ACS</span></span>

* <span data-ttu-id="9fb94-2355">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="9fb94-2355">Corrected preview regions</span></span>
* <span data-ttu-id="9fb94-2356">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2356">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="9fb94-2357">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2357">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2358">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2358">Appservice</span></span>

* <span data-ttu-id="9fb94-2359">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2359">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="9fb94-2360">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2360">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="9fb94-2361">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2361">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="9fb94-2362">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2362">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="9fb94-2363">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2363">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-2364">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-2364">IoT</span></span>

* <span data-ttu-id="9fb94-2365">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2365">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2366">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2366">Network</span></span>

* <span data-ttu-id="9fb94-2367">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2367">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9fb94-2368">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2368">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="9fb94-2369">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2369">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9fb94-2370">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2370">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9fb94-2371">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2371">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2372">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2372">Profile</span></span>

* <span data-ttu-id="9fb94-2373">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2373">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fb94-2374">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-2374">Service Fabric</span></span>

* <span data-ttu-id="9fb94-2375">Préversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-2375">Preview release</span></span>
* <span data-ttu-id="9fb94-2376">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-2376">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="9fb94-2377">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="9fb94-2377">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="9fb94-2378">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2378">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2379">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2379">Storage</span></span>

* <span data-ttu-id="9fb94-2380">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="9fb94-2380">Enabled setting blob tier</span></span>
* <span data-ttu-id="9fb94-2381">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="9fb94-2381">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="9fb94-2382">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2382">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="9fb94-2383">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="9fb94-2383">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="9fb94-2384">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2384">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="9fb94-2385">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2385">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2386">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2386">VM</span></span>

* <span data-ttu-id="9fb94-2387">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2387">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="9fb94-2388">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="9fb94-2388">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="9fb94-2389">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2389">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fb94-2390">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="9fb94-2390">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="9fb94-2391">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="9fb94-2391">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="9fb94-2392">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2392">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="9fb94-2393">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2393">August 15, 2017</span></span>

<span data-ttu-id="9fb94-2394">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="9fb94-2394">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2395">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2395">ACS</span></span>

* <span data-ttu-id="9fb94-2396">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2396">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2397">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2397">Appservice</span></span>

* <span data-ttu-id="9fb94-2398">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="9fb94-2398">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fb94-2399">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fb94-2399">Event Grid</span></span>

* <span data-ttu-id="9fb94-2400">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2400">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="9fb94-2401">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2401">August 11, 2017</span></span>

<span data-ttu-id="9fb94-2402">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="9fb94-2402">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2403">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2403">ACS</span></span>

* <span data-ttu-id="9fb94-2404">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="9fb94-2404">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-2405">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2405">Batch</span></span>

* <span data-ttu-id="9fb94-2406">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="9fb94-2406">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="9fb94-2407">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-2407">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="9fb94-2408">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="9fb94-2408">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="9fb94-2409">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="9fb94-2409">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="9fb94-2410">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="9fb94-2410">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="9fb94-2411">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="9fb94-2411">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="9fb94-2412">Composant</span><span class="sxs-lookup"><span data-stu-id="9fb94-2412">Component</span></span>

* <span data-ttu-id="9fb94-2413">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2413">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="9fb94-2414">Conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2414">Container</span></span>

* <span data-ttu-id="9fb94-2415">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2415">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="9fb94-2416">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2416">Data Lake Store</span></span>

* <span data-ttu-id="9fb94-2417">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="9fb94-2417">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fb94-2418">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fb94-2418">Event Grid</span></span>

* <span data-ttu-id="9fb94-2419">Version initiale</span><span class="sxs-lookup"><span data-stu-id="9fb94-2419">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2420">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2420">Network</span></span>

* <span data-ttu-id="9fb94-2421">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="9fb94-2421">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="9fb94-2422">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2422">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="9fb94-2423">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2423">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="9fb94-2424">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2424">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2425">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2425">Profile</span></span>

* <span data-ttu-id="9fb94-2426">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2426">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2427">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2427">Storage</span></span>

* <span data-ttu-id="9fb94-2428">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="9fb94-2428">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2429">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2429">VM</span></span>

* <span data-ttu-id="9fb94-2430">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="9fb94-2430">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="9fb94-2431">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2431">Exposed `list-skus` command</span></span>
* <span data-ttu-id="9fb94-2432">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2432">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="9fb94-2433">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="9fb94-2433">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="9fb94-2434">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2434">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="9fb94-2435">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2435">July 28, 2017</span></span>

<span data-ttu-id="9fb94-2436">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="9fb94-2436">Version 2.0.12</span></span>

* <span data-ttu-id="9fb94-2437">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2437">Added container commands</span></span>
* <span data-ttu-id="9fb94-2438">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="9fb94-2438">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="9fb94-2439">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2439">Core</span></span>

* <span data-ttu-id="9fb94-2440">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="9fb94-2440">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="9fb94-2441">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2441">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="9fb94-2442">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2442">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="9fb94-2443">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2443">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="9fb94-2444">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="9fb94-2444">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="9fb94-2445">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2445">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="9fb94-2446">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2446">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9fb94-2447">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2447">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="9fb94-2448">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2448">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="9fb94-2449">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2449">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="9fb94-2450">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="9fb94-2450">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="9fb94-2451">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2451">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="9fb94-2452">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-2452">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="9fb94-2453">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="9fb94-2453">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="9fb94-2454">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fb94-2454">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="9fb94-2455">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2455">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="9fb94-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2456">ACR</span></span>

* <span data-ttu-id="9fb94-2457">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2457">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="9fb94-2458">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2458">Support SKU update for managed registries</span></span>
* <span data-ttu-id="9fb94-2459">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2459">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="9fb94-2460">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="9fb94-2460">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="9fb94-2461">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="9fb94-2461">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="9fb94-2462">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="9fb94-2462">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2463">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2463">ACS</span></span>

* <span data-ttu-id="9fb94-2464">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="9fb94-2464">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2465">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2465">Appservice</span></span>

* <span data-ttu-id="9fb94-2466">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="9fb94-2466">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="9fb94-2467">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2467">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="9fb94-2468">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2468">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="9fb94-2469">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2469">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="9fb94-2470">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2470">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="9fb94-2471">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2471">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="9fb94-2472">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2472">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="9fb94-2473">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2473">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="9fb94-2474">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2474">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="9fb94-2475">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2475">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="9fb94-2476">Batch</span><span class="sxs-lookup"><span data-stu-id="9fb94-2476">Batch</span></span>

* <span data-ttu-id="9fb94-2477">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="9fb94-2477">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="9fb94-2478">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2478">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="9fb94-2479">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2479">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="9fb94-2480">CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2480">CDN</span></span>

* <span data-ttu-id="9fb94-2481">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-2481">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="9fb94-2482">Cloud</span><span class="sxs-lookup"><span data-stu-id="9fb94-2482">Cloud</span></span>

* <span data-ttu-id="9fb94-2483">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="9fb94-2483">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="9fb94-2484">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2484">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="9fb94-2485">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="9fb94-2485">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="9fb94-2486">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="9fb94-2486">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="9fb94-2487">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2487">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-2488">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-2488">CosmosDB</span></span>

* <span data-ttu-id="9fb94-2489">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2489">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="9fb94-2490">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="9fb94-2490">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fb94-2491">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-2491">Data Lake Analytics</span></span>

* <span data-ttu-id="9fb94-2492">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2492">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="9fb94-2493">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2493">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="9fb94-2494">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2494">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fb94-2495">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2495">Data Lake Store</span></span>

* <span data-ttu-id="9fb94-2496">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2496">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="9fb94-2497">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="9fb94-2497">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="9fb94-2498">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2498">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="9fb94-2499">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2499">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="9fb94-2500">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fb94-2500">Interactive</span></span>

* <span data-ttu-id="9fb94-2501">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="9fb94-2501">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="9fb94-2502">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="9fb94-2502">Increased test coverage</span></span>
* <span data-ttu-id="9fb94-2503">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="9fb94-2503">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="9fb94-2504">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2504">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="9fb94-2505">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2505">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="9fb94-2506">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2506">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="9fb94-2507">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2507">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9fb94-2508">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2508">Added `--progress` flag</span></span>
* <span data-ttu-id="9fb94-2509">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="9fb94-2509">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="9fb94-2510">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2510">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="9fb94-2511">IoT</span><span class="sxs-lookup"><span data-stu-id="9fb94-2511">IoT</span></span>

* <span data-ttu-id="9fb94-2512">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2512">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="9fb94-2513">(#3934)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2513">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fb94-2514">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2514">Key vault</span></span>

* <span data-ttu-id="9fb94-2515">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2515">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="9fb94-2516">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2516">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="9fb94-2517">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2517">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9fb94-2518">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2518">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9fb94-2519">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2519">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="9fb94-2520">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2520">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="9fb94-2521">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2521">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="9fb94-2522">(#3307)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2522">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="9fb94-2523">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2523">Lab</span></span>

* <span data-ttu-id="9fb94-2524">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2524">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="9fb94-2525">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2525">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2526">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2526">Monitor</span></span>

* <span data-ttu-id="9fb94-2527">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2527">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="9fb94-2528">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2528">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="9fb94-2529">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2529">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="9fb94-2530">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2530">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="9fb94-2531">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2531">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="9fb94-2532">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="9fb94-2532">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="9fb94-2533">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="9fb94-2533">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="9fb94-2534">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2534">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="9fb94-2535">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2535">`location` no longer required</span></span>
  * <span data-ttu-id="9fb94-2536">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="9fb94-2536">Add name and ID support for target</span></span>
  * <span data-ttu-id="9fb94-2537">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2537">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="9fb94-2538">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2538">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="9fb94-2539">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="9fb94-2539">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="9fb94-2540">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="9fb94-2540">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="9fb94-2541">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2541">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="9fb94-2542">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2542">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2543">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2543">Network</span></span>

* <span data-ttu-id="9fb94-2544">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2544">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="9fb94-2545">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2545">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="9fb94-2546">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="9fb94-2546">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="9fb94-2547">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="9fb94-2547">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="9fb94-2548">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2548">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="9fb94-2549">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2549">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="9fb94-2550">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2550">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="9fb94-2551">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2551">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="9fb94-2552">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2552">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="9fb94-2553">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2553">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="9fb94-2554">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2554">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="9fb94-2555">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2555">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="9fb94-2556">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2556">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="9fb94-2557">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2557">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="9fb94-2558">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2558">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="9fb94-2559">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2559">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="9fb94-2560">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="9fb94-2560">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="9fb94-2561">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2561">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="9fb94-2562">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2562">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="9fb94-2563">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2563">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="9fb94-2564">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2564">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="9fb94-2565">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2565">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="9fb94-2566">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2566">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="9fb94-2567">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9fb94-2567">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="9fb94-2568">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9fb94-2568">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="9fb94-2569">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9fb94-2569">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="9fb94-2570">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="9fb94-2570">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2571">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2571">Profile</span></span>

* <span data-ttu-id="9fb94-2572">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2572">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="9fb94-2573">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2573">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="9fb94-2574">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="9fb94-2574">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="9fb94-2575">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2575">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="9fb94-2576">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="9fb94-2576">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fb94-2577">SGBDR</span><span class="sxs-lookup"><span data-stu-id="9fb94-2577">RDBMS</span></span>

* <span data-ttu-id="9fb94-2578">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2578">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="9fb94-2579">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2579">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="9fb94-2580">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2580">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="9fb94-2581">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2581">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2582">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2582">Resource</span></span>

* <span data-ttu-id="9fb94-2583">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2583">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="9fb94-2584">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2584">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="9fb94-2585">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2585">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="9fb94-2586">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="9fb94-2586">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="9fb94-2587">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2587">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="9fb94-2588">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2588">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="9fb94-2589">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2589">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="9fb94-2590">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="9fb94-2590">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-2591">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-2591">Role</span></span>

* <span data-ttu-id="9fb94-2592">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2592">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="9fb94-2593">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2593">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="9fb94-2594">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="9fb94-2594">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="9fb94-2595">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2595">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="9fb94-2596">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2596">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fb94-2597">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-2597">Service Fabric</span></span>
* <span data-ttu-id="9fb94-2598">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2598">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="9fb94-2599">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2599">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="9fb94-2600">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2600">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2601">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2601">SQL</span></span>

* <span data-ttu-id="9fb94-2602">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2602">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="9fb94-2603">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2603">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="9fb94-2604">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2604">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2605">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2605">Storage</span></span>

* <span data-ttu-id="9fb94-2606">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2606">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="9fb94-2607">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="9fb94-2607">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="9fb94-2608">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2608">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="9fb94-2609">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2609">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="9fb94-2610">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2610">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="9fb94-2611">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2611">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2612">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2612">VM</span></span>

* <span data-ttu-id="9fb94-2613">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2613">Support configuring nsg</span></span>
* <span data-ttu-id="9fb94-2614">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2614">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="9fb94-2615">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="9fb94-2615">Support managed service identities</span></span>
* <span data-ttu-id="9fb94-2616">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2616">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="9fb94-2617">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="9fb94-2617">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="9fb94-2618">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2618">May 10, 2017</span></span>

<span data-ttu-id="9fb94-2619">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="9fb94-2619">Version 2.0.6</span></span>

* <span data-ttu-id="9fb94-2620">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9fb94-2620">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="9fb94-2621">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2621">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="9fb94-2622">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2622">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="9fb94-2623">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fb94-2623">Include Cognitive Services module</span></span>
* <span data-ttu-id="9fb94-2624">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fb94-2624">Include Service Fabric module</span></span>
* <span data-ttu-id="9fb94-2625">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2625">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="9fb94-2626">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2626">Add support for CDN commands</span></span>
* <span data-ttu-id="9fb94-2627">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="9fb94-2627">Remove Container module</span></span>
* <span data-ttu-id="9fb94-2628">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2628">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="9fb94-2629">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2629">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="9fb94-2630">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2630">Core</span></span>

* <span data-ttu-id="9fb94-2631">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2631">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="9fb94-2632">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2632">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="9fb94-2633">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2633">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="9fb94-2634">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2634">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="9fb94-2635">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2635">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="9fb94-2636">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2636">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="9fb94-2637">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2637">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="9fb94-2638">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2638">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="9fb94-2639">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2639">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="9fb94-2640">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="9fb94-2640">core: Improved performance</span></span>
* <span data-ttu-id="9fb94-2641">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="9fb94-2641">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="9fb94-2642">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="9fb94-2642">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2643">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2643">ACS</span></span>

* <span data-ttu-id="9fb94-2644">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="9fb94-2644">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="9fb94-2645">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="9fb94-2645">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="9fb94-2646">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="9fb94-2646">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="9fb94-2647">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2647">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2648">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2648">AppService</span></span>

* <span data-ttu-id="9fb94-2649">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2649">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="9fb94-2650">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2650">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="9fb94-2651">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2651">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="9fb94-2652">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="9fb94-2652">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="9fb94-2653">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2653">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="9fb94-2654">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2654">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="9fb94-2655">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="9fb94-2655">support slot swap with preview</span></span>
* <span data-ttu-id="9fb94-2656">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2656">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="9fb94-2657">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2657">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fb94-2658">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-2658">CosmosDB</span></span>

* <span data-ttu-id="9fb94-2659">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9fb94-2659">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="9fb94-2660">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="9fb94-2660">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="9fb94-2661">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="9fb94-2661">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="9fb94-2662">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="9fb94-2662">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fb94-2663">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-2663">Data Lake Analytics</span></span>

* <span data-ttu-id="9fb94-2664">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2664">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="9fb94-2665">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2665">Add support for new catalog item type: package.</span></span> <span data-ttu-id="9fb94-2666">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2666">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="9fb94-2667">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2667">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="9fb94-2668">Table</span><span class="sxs-lookup"><span data-stu-id="9fb94-2668">Table</span></span>
  * <span data-ttu-id="9fb94-2669">Fonction table</span><span class="sxs-lookup"><span data-stu-id="9fb94-2669">Table valued function</span></span>
  * <span data-ttu-id="9fb94-2670">Affichage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2670">View</span></span>
  * <span data-ttu-id="9fb94-2671">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2671">Table Statistics.</span></span> <span data-ttu-id="9fb94-2672">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="9fb94-2672">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fb94-2673">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2673">Data Lake Store</span></span>

* <span data-ttu-id="9fb94-2674">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="9fb94-2674">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="9fb94-2675">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2675">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="9fb94-2676">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2676">missed help for access show.</span></span> <span data-ttu-id="9fb94-2677">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2677">adding it.</span></span> <span data-ttu-id="9fb94-2678">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2678">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="9fb94-2679">Rechercher</span><span class="sxs-lookup"><span data-stu-id="9fb94-2679">Find</span></span>

* <span data-ttu-id="9fb94-2680">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="9fb94-2680">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fb94-2681">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fb94-2681">KeyVault</span></span>

* <span data-ttu-id="9fb94-2682">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="9fb94-2682">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="9fb94-2683">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="9fb94-2683">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="9fb94-2684">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="9fb94-2684">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="9fb94-2685">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-2685">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="9fb94-2686">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2686">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="9fb94-2687">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2687">Lab</span></span>

* <span data-ttu-id="9fb94-2688">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2688">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="9fb94-2689">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2689">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="9fb94-2690">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2690">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="9fb94-2691">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2691">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="9fb94-2692">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="9fb94-2692">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="9fb94-2693">Surveiller</span><span class="sxs-lookup"><span data-stu-id="9fb94-2693">Monitor</span></span>

* <span data-ttu-id="9fb94-2694">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2694">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="9fb94-2695">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2695">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="9fb94-2696">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2696">Network</span></span>

* <span data-ttu-id="9fb94-2697">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2697">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="9fb94-2698">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2698">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="9fb94-2699">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9fb94-2699">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="9fb94-2700">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9fb94-2700">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="9fb94-2701">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9fb94-2701">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="9fb94-2702">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9fb94-2702">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="9fb94-2703">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2703">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="9fb94-2704">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="9fb94-2704">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="9fb94-2705">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2705">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="9fb94-2706">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="9fb94-2706">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="9fb94-2707">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2707">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="9fb94-2708">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2708">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="9fb94-2709">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2709">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="9fb94-2710">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="9fb94-2710">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="9fb94-2711">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="9fb94-2711">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="9fb94-2712">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="9fb94-2712">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="9fb94-2713">Profil</span><span class="sxs-lookup"><span data-stu-id="9fb94-2713">Profile</span></span>

* <span data-ttu-id="9fb94-2714">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2714">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="9fb94-2715">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2715">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="9fb94-2716">Redis</span><span class="sxs-lookup"><span data-stu-id="9fb94-2716">Redis</span></span>

* <span data-ttu-id="9fb94-2717">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="9fb94-2717">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="9fb94-2718">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="9fb94-2718">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="9fb94-2719">Ressource</span><span class="sxs-lookup"><span data-stu-id="9fb94-2719">Resource</span></span>

* <span data-ttu-id="9fb94-2720">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2720">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="9fb94-2721">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2721">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="9fb94-2722">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2722">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="9fb94-2723">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2723">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="9fb94-2724">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2724">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="9fb94-2725">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2725">Add docs for az lock update.</span></span> <span data-ttu-id="9fb94-2726">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2726">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="9fb94-2727">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2727">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="9fb94-2728">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2728">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="9fb94-2729">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2729">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="9fb94-2730">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2730">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="9fb94-2731">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2731">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="9fb94-2732">Role</span><span class="sxs-lookup"><span data-stu-id="9fb94-2732">Role</span></span>

* <span data-ttu-id="9fb94-2733">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2733">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="9fb94-2734">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2734">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="9fb94-2735">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2735">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="9fb94-2736">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="9fb94-2736">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="9fb94-2737">SQL</span><span class="sxs-lookup"><span data-stu-id="9fb94-2737">SQL</span></span>

* <span data-ttu-id="9fb94-2738">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="9fb94-2738">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="9fb94-2739">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2739">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="9fb94-2740">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2740">Storage</span></span>

* <span data-ttu-id="9fb94-2741">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="9fb94-2741">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="9fb94-2742">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="9fb94-2742">Add support for incremental blob copy</span></span>
* <span data-ttu-id="9fb94-2743">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="9fb94-2743">Add support for large block blob upload</span></span>
* <span data-ttu-id="9fb94-2744">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="9fb94-2744">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2745">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2745">VM</span></span>

* <span data-ttu-id="9fb94-2746">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="9fb94-2746">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="9fb94-2747">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2747">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="9fb94-2748">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="9fb94-2748">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="9fb94-2749">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="9fb94-2749">az vm/vmss disk</span></span>
  3. <span data-ttu-id="9fb94-2750">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="9fb94-2750">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="9fb94-2751">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="9fb94-2751">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="9fb94-2752">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2752">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="9fb94-2753">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2753">April 3, 2017</span></span>

<span data-ttu-id="9fb94-2754">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="9fb94-2754">Version 2.0.2</span></span>

<span data-ttu-id="9fb94-2755">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="9fb94-2755">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="9fb94-2756">Core</span><span class="sxs-lookup"><span data-stu-id="9fb94-2756">Core</span></span>

* <span data-ttu-id="9fb94-2757">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2757">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="9fb94-2758">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2758">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="9fb94-2759">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2759">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="9fb94-2760">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2760">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9fb94-2761">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2761">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="9fb94-2762">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2762">Add prompting for missing template parameters.</span></span> <span data-ttu-id="9fb94-2763">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2763">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="9fb94-2764">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="9fb94-2764">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="9fb94-2765">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="9fb94-2765">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="9fb94-2766">ACS</span><span class="sxs-lookup"><span data-stu-id="9fb94-2766">ACS</span></span>

* <span data-ttu-id="9fb94-2767">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2767">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="9fb94-2768">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2768">Add support for ssh key password prompting.</span></span> <span data-ttu-id="9fb94-2769">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2769">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="9fb94-2770">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2770">Add support for windows clusters.</span></span> <span data-ttu-id="9fb94-2771">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2771">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="9fb94-2772">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2772">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="9fb94-2773">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2773">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="9fb94-2774">AppService</span><span class="sxs-lookup"><span data-stu-id="9fb94-2774">AppService</span></span>

* <span data-ttu-id="9fb94-2775">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2775">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="9fb94-2776">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2776">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="9fb94-2777">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2777">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="9fb94-2778">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2778">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="9fb94-2779">DataLake</span><span class="sxs-lookup"><span data-stu-id="9fb94-2779">DataLake</span></span>

* <span data-ttu-id="9fb94-2780">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fb94-2780">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="9fb94-2781">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fb94-2781">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="9fb94-2782">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="9fb94-2782">DocuemntDB</span></span>

* <span data-ttu-id="9fb94-2783">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2783">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="9fb94-2784">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="9fb94-2784">VM</span></span>

* <span data-ttu-id="9fb94-2785">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2785">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="9fb94-2786">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2786">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="9fb94-2787">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2787">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="9fb94-2788">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2788">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9fb94-2789">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2789">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="9fb94-2790">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2790">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="9fb94-2791">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="9fb94-2791">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="9fb94-2792">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="9fb94-2792">February 27, 2017</span></span>

<span data-ttu-id="9fb94-2793">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="9fb94-2793">Version 2.0.0</span></span>

<span data-ttu-id="9fb94-2794">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2794">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="9fb94-2795">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2795">Container Service (acs)</span></span>
- <span data-ttu-id="9fb94-2796">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2796">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="9fb94-2797">Réseau</span><span class="sxs-lookup"><span data-stu-id="9fb94-2797">Networking</span></span>
- <span data-ttu-id="9fb94-2798">Stockage</span><span class="sxs-lookup"><span data-stu-id="9fb94-2798">Storage</span></span>

<span data-ttu-id="9fb94-2799">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2799">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="9fb94-2800">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2800">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="9fb94-2801">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2801">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="9fb94-2802">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2802">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="9fb94-2803">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="9fb94-2803">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="9fb94-2804">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="9fb94-2804">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="9fb94-2805">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="9fb94-2805">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="9fb94-2806">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="9fb94-2806">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="9fb94-2807">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9fb94-2807">Provide feedback from the command line with the `az feedback` command</span></span>

