---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/30/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: efb17acb25b2268496efe313cac0a8189a78930a
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2020
ms.locfileid: "82591422"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="88779-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="88779-103">Azure CLI release notes</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="88779-104">30 avril 2020</span><span class="sxs-lookup"><span data-stu-id="88779-104">April 30, 2020</span></span>

<span data-ttu-id="88779-105">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="88779-105">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="88779-106">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-106">ACR</span></span>

* <span data-ttu-id="88779-107">`az acr check-health`: Correction de « DOCKER_PULL_ERROR » sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-107">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="88779-108">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-108">Compute</span></span>

* <span data-ttu-id="88779-109">`az vm list-ip-addresses`: Gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="88779-109">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="88779-110">Correction d’un bogue de vm create si endpoint_vm_image_alias_doc n’est pas défini dans le profil cloud</span><span class="sxs-lookup"><span data-stu-id="88779-110">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="88779-111">`az vmss create`: Ajout de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="88779-111">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-112">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-112">Cosmos DB</span></span>

* <span data-ttu-id="88779-113">`az cosmosdb create/update` : ajout de la prise en charge de add --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="88779-113">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="88779-114">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-114">Extension</span></span>

* <span data-ttu-id="88779-115">Correction du chargement des métadonnées incorrectes pour l’extension du type de roulette</span><span class="sxs-lookup"><span data-stu-id="88779-115">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-116">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-116">Packaging</span></span>

* <span data-ttu-id="88779-117">Ajout du script az pour Git Bash/Cygwin sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-117">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="88779-118">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-118">SQL</span></span>

* <span data-ttu-id="88779-119">`az sql instance-pool`: Ajout d’un groupe de commandes pour les pools d’instances</span><span class="sxs-lookup"><span data-stu-id="88779-119">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="88779-120">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-120">Storage</span></span>

* <span data-ttu-id="88779-121">Mise à niveau du package azure-multiapi-storage vers 0.3.0</span><span class="sxs-lookup"><span data-stu-id="88779-121">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="88779-122">Prise en charge de GZRS pour la création et la mise à jour de comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-122">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="88779-123">`az storage account failover`: Ajout de la prise en charge du basculement de comptes de stockage grs/gzrs</span><span class="sxs-lookup"><span data-stu-id="88779-123">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="88779-124">`az storage blob upload`: Ajout du paramètre --encryption-scope pour prendre en charge la spécification des informations d’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="88779-124">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="88779-125">28 avril 2020</span><span class="sxs-lookup"><span data-stu-id="88779-125">April 28, 2020</span></span>

<span data-ttu-id="88779-126">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="88779-126">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="88779-127">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-127">ACS</span></span>

* <span data-ttu-id="88779-128">[CHANGEMENT CASSANT] du paramètre az openshift create: remove --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="88779-128">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="88779-129">`az openshift create` : Ajout d’indicateurs pour prendre en charge un cluster privé.</span><span class="sxs-lookup"><span data-stu-id="88779-129">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="88779-130">`az openshift` : Mise à niveau vers la version d’API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="88779-130">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="88779-131">`az openshift` : Ajout de la commande `update`.</span><span class="sxs-lookup"><span data-stu-id="88779-131">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="88779-132">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-132">AKS</span></span>

* <span data-ttu-id="88779-133">`az aks create`: Ajout de la prise en charge de Windows</span><span class="sxs-lookup"><span data-stu-id="88779-133">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-134">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-134">AppService</span></span>

* <span data-ttu-id="88779-135">`az webapp deployment source config-zip` : Suppression de sleep après request.get()</span><span class="sxs-lookup"><span data-stu-id="88779-135">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="88779-136">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-136">ARM</span></span>

* <span data-ttu-id="88779-137">Ajout de commandes What-If de déploiement de modèles</span><span class="sxs-lookup"><span data-stu-id="88779-137">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="88779-138">ARO</span><span class="sxs-lookup"><span data-stu-id="88779-138">ARO</span></span>

* <span data-ttu-id="88779-139">`az aro`: Correction de la sortie de table</span><span class="sxs-lookup"><span data-stu-id="88779-139">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="88779-140">CI</span><span class="sxs-lookup"><span data-stu-id="88779-140">CI</span></span>

* <span data-ttu-id="88779-141">Intégration de pytest et dépréciation de nose pour le test d’automatisation</span><span class="sxs-lookup"><span data-stu-id="88779-141">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="88779-142">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-142">Compute</span></span>

* <span data-ttu-id="88779-143">`az vmss disk detach` : Correction du problème NoneType du disque de données</span><span class="sxs-lookup"><span data-stu-id="88779-143">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="88779-144">`az vm availability-set list`: Prise en charge de l’affichage de la liste de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="88779-144">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="88779-145">`az vm list-skus`: Correction du problème d’affichage du format de table</span><span class="sxs-lookup"><span data-stu-id="88779-145">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-146">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-146">KeyVault</span></span>

* <span data-ttu-id="88779-147">Ajout d’un nouveau paramètre `--enable-rbac-authorization` lors de la création ou de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="88779-147">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-148">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-148">Monitor</span></span>

* <span data-ttu-id="88779-149">Prise en charge des fonctionnalités CMK de cluster LA</span><span class="sxs-lookup"><span data-stu-id="88779-149">Support LA cluster CMK features</span></span>
* <span data-ttu-id="88779-150">`az monitor log-analytics workspace linked-storage` : Prise en charge des fonctionnalités BYOS</span><span class="sxs-lookup"><span data-stu-id="88779-150">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="88779-151">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-151">Network</span></span>

* <span data-ttu-id="88779-152">`az network security-partner` : Prise en charge du fournisseur de partenaire de sécurité</span><span class="sxs-lookup"><span data-stu-id="88779-152">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="88779-153">Privatedns</span><span class="sxs-lookup"><span data-stu-id="88779-153">Privatedns</span></span>

* <span data-ttu-id="88779-154">Ajout d’une fonctionnalité dans une zone DNS privée pour importer/exporter un fichier de zone</span><span class="sxs-lookup"><span data-stu-id="88779-154">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="88779-155">21 avril 2020</span><span class="sxs-lookup"><span data-stu-id="88779-155">April 21, 2020</span></span>

<span data-ttu-id="88779-156">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="88779-156">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="88779-157">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-157">ACR</span></span>

* <span data-ttu-id="88779-158">`az acr run --cmd` : désactivation du remplacement du répertoire de travail</span><span class="sxs-lookup"><span data-stu-id="88779-158">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="88779-159">Prise en charge du point de terminaison de données dédié</span><span class="sxs-lookup"><span data-stu-id="88779-159">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="88779-160">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-160">AKS</span></span>

* <span data-ttu-id="88779-161">`az aks list -o table` doit afficher privateFqdn comme nom de domaine complet pour les clusters privés</span><span class="sxs-lookup"><span data-stu-id="88779-161">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="88779-162">Ajout de --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="88779-162">Add --uptime-sla</span></span>
* <span data-ttu-id="88779-163">Mise à jour du package containerservice</span><span class="sxs-lookup"><span data-stu-id="88779-163">Update containerservice package</span></span>
* <span data-ttu-id="88779-164">Ajout de la prise en charge de l’adresse IP publique de nœud</span><span class="sxs-lookup"><span data-stu-id="88779-164">Add node public IP support</span></span>
* <span data-ttu-id="88779-165">Correction d’une faute de frappe dans la commande d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-165">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-166">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-166">AppConfig</span></span>

* <span data-ttu-id="88779-167">Résolution de la référence du coffre de clés pour la liste Key Vault et les commandes d’exportation</span><span class="sxs-lookup"><span data-stu-id="88779-167">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="88779-168">Résolution de bogue pour les valeurs de clé de liste</span><span class="sxs-lookup"><span data-stu-id="88779-168">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-169">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-169">AppService</span></span>

* <span data-ttu-id="88779-170">`az functionapp create`: Modification de la façon dont linuxFxVersion était défini pour les applications de fonction dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="88779-170">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="88779-171">Cela doit résoudre un bogue qui empêchait la création d’applications de consommation dotnet linux</span><span class="sxs-lookup"><span data-stu-id="88779-171">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="88779-172">[CHANGEMENT CASSANT] `az webapp create` : correctif pour conserver les paramètres d’application existants avec az webapp create</span><span class="sxs-lookup"><span data-stu-id="88779-172">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="88779-173">[CHANGEMENT CASSANT] `az webapp up` : correctif pour créer un groupe de ressources pour la commande az webapp up lors de l’utilisation de l’indicateur -g</span><span class="sxs-lookup"><span data-stu-id="88779-173">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="88779-174">[CHANGEMENT CASSANT] `az webapp config` : correctif pour afficher des valeurs pour la sortie non-JSON avec la liste de chaînes de connexion az webapp config</span><span class="sxs-lookup"><span data-stu-id="88779-174">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="88779-175">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-175">ARM</span></span>

* <span data-ttu-id="88779-176">`az deployment create/validate`: Ajout d’un paramètre `--no-prompt` pour prendre en charge le saut de l’invite de paramètres manquants pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="88779-176">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="88779-177">`az deployment group/mg/sub/tenant validate`: Prise en charge de commentaires dans le fichier de paramètres de déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-177">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="88779-178">`az deployment`: Suppression de `is_preview` pour le paramètre `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="88779-178">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="88779-179">`az deployment group/mg/sub/tenant cancel`: Prise en charge de l’annulation du déploiement pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="88779-179">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="88779-180">`az deployment group/mg/sub/tenant validate`: Amélioration du message d’erreur lors de l’échec de la vérification du déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-180">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="88779-181">`az deployment-scripts`: Ajout de nouvelles commandes pour DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="88779-181">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="88779-182">`az resource tag`: Ajout du paramètre `--is-incremental` pour prendre en charge l’ajout incrémentiel de balises aux ressources</span><span class="sxs-lookup"><span data-stu-id="88779-182">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="88779-183">ARO</span><span class="sxs-lookup"><span data-stu-id="88779-183">ARO</span></span>

* <span data-ttu-id="88779-184">`az aro`:  Ajout du module de commande aro Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="88779-184">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="88779-185">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-185">Batch</span></span>

* <span data-ttu-id="88779-186">Mise à jour de l’API Batch</span><span class="sxs-lookup"><span data-stu-id="88779-186">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="88779-187">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-187">Compute</span></span>

* <span data-ttu-id="88779-188">`az sig image-version create`: Ajout d’un type de compte de stockage Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="88779-188">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="88779-189">`az vmss update`: Correction d’un problème de mise à jour de notification d’arrêt</span><span class="sxs-lookup"><span data-stu-id="88779-189">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="88779-190">`az vm/vmss create`: Ajout de la prise en charge de la version d’image spécialisée</span><span class="sxs-lookup"><span data-stu-id="88779-190">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="88779-191">Version de l’API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="88779-191">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="88779-192">`az sig image-version create`: Ajout de --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="88779-192">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="88779-193">Correction de l’échec des tests lors d’une exécution en série en raison d’un nom de coffre de clés en double dans le cache en mémoire global</span><span class="sxs-lookup"><span data-stu-id="88779-193">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-194">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-194">CosmosDB</span></span>

* <span data-ttu-id="88779-195">Prise en charge d’`az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="88779-195">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="88779-196">IoT Central</span><span class="sxs-lookup"><span data-stu-id="88779-196">IoT Central</span></span>

* <span data-ttu-id="88779-197">Dépréciation d’`az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="88779-197">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="88779-198">Ajout du module de commande `az iot central`</span><span class="sxs-lookup"><span data-stu-id="88779-198">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-199">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-199">Monitor</span></span>

* <span data-ttu-id="88779-200">Prise en charge du scénario de lien privé pour la supervision</span><span class="sxs-lookup"><span data-stu-id="88779-200">Support private link scenario for monitor</span></span>
* <span data-ttu-id="88779-201">Correction du mode de simulation incorrect dans test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="88779-201">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="88779-202">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-202">Network</span></span>

* <span data-ttu-id="88779-203">Dépréciation de la référence sku pour la commande de mise à jour de l’adresse IP publique</span><span class="sxs-lookup"><span data-stu-id="88779-203">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="88779-204">`az network private-endpoint`: Prise en charge du groupe de zones DNS privées</span><span class="sxs-lookup"><span data-stu-id="88779-204">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="88779-205">Activation de la fonctionnalité de contexte local pour le paramètre de réseau virtuel/sous-réseau</span><span class="sxs-lookup"><span data-stu-id="88779-205">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="88779-206">Correction d’un exemple d’utilisation incorrect dans test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="88779-206">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-207">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-207">Packaging</span></span>

* <span data-ttu-id="88779-208">Suppression de la prise en charge d’un package Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="88779-208">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-209">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-209">RBAC</span></span>

* <span data-ttu-id="88779-210">`az ad app create/update` : prise en charge de --optional-claims en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="88779-210">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-211">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-211">RDBMS</span></span>

* <span data-ttu-id="88779-212">Ajout des commandes d’administrateur Azure Active Directory pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="88779-212">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="88779-213">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-213">Service Fabric</span></span>

* <span data-ttu-id="88779-214">Correctif n  12891 : `az sf application update --application-parameters` supprime les anciens paramètres qui ne sont pas dans la demande</span><span class="sxs-lookup"><span data-stu-id="88779-214">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="88779-215">Correctif n  12470, az sf create cluster, résolution de bogues dans la durabilité et la fiabilité des mises à jour, et recherche de groupes identiques de machines virtuelles correctement dans le code en fonction d’un nom de type de nœud</span><span class="sxs-lookup"><span data-stu-id="88779-215">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="88779-216">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-216">SQL</span></span>

* <span data-ttu-id="88779-217">Ajout d’`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="88779-217">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="88779-218">`az sql midb` : mise à jour/affichage de la stratégie de conservation à long terme, affichage/suppression des sauvegardes de conservation à long terme, restauration de la sauvegarde de conservation à long terme</span><span class="sxs-lookup"><span data-stu-id="88779-218">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="88779-219">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-219">Storage</span></span>

* <span data-ttu-id="88779-220">Mise à niveau d’azure-mgmt-storage vers 9.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-220">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="88779-221">`az storage logging off`: Prise en charge de la désactivation de la journalisation pour un compte de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-221">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="88779-222">`az storage account update`: Activation de la rotation automatique de la clé pour CMK</span><span class="sxs-lookup"><span data-stu-id="88779-222">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="88779-223">`az storage account encryption-scope create/update/list/show`: Ajout de la prise en charge de la personnalisation de l’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="88779-223">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="88779-224">`az storage container create`: Ajout de --default-encryption-scope et --deny-encryption-scope-override pour définir l’étendue du chiffrement de niveau de conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-224">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="88779-225">Enquête</span><span class="sxs-lookup"><span data-stu-id="88779-225">Survey</span></span>

* <span data-ttu-id="88779-226">Ajout d’une instruction switch pour désactiver le lien d’enquête</span><span class="sxs-lookup"><span data-stu-id="88779-226">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="88779-227">01 avril 2020</span><span class="sxs-lookup"><span data-stu-id="88779-227">April 01, 2020</span></span>

<span data-ttu-id="88779-228">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="88779-228">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="88779-229">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-229">ACR</span></span>

* <span data-ttu-id="88779-230">Correction d’une version incorrecte d’azure-mgmt-containerregistry pour Linux</span><span class="sxs-lookup"><span data-stu-id="88779-230">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="88779-231">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-231">Profile</span></span>

* <span data-ttu-id="88779-232">az login : Correction des échecs de connexion avec les profils cloud autres que `latest`</span><span class="sxs-lookup"><span data-stu-id="88779-232">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="88779-233">31 mars 2020</span><span class="sxs-lookup"><span data-stu-id="88779-233">March 31, 2020</span></span>

<span data-ttu-id="88779-234">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="88779-234">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="88779-235">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-235">ACR</span></span>

* <span data-ttu-id="88779-236">'az acr task update' : exception du pointeur null</span><span class="sxs-lookup"><span data-stu-id="88779-236">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="88779-237">`az acr import`: Modification de l’aide et du message d’erreur pour clarifier l’utilisation de --source et --registry</span><span class="sxs-lookup"><span data-stu-id="88779-237">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="88779-238">Ajout d’un validateur pour l’argument 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="88779-238">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="88779-239">`az acr login` : Suppression de l’indicateur de préversion sur '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="88779-239">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="88779-240">[CHANGEMENT CASSANT] Suppression du paramètre de branche 'az acr task create/update'</span><span class="sxs-lookup"><span data-stu-id="88779-240">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="88779-241">'az acr task update' : Le client peut maintenant mettre à jour le contexte, git-token et/ou les déclencheurs individuellement</span><span class="sxs-lookup"><span data-stu-id="88779-241">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="88779-242">'az acr agentpool' : nouvelle fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="88779-242">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="88779-243">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-243">AKS</span></span>

* <span data-ttu-id="88779-244">Correction d’apiServerAccessProfile lors de la mise à jour de --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="88779-244">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="88779-245">aks update : Remplacement des adresses IP sortantes par des valeurs d’entrée lors de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="88779-245">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="88779-246">Pas de création de SPN pour les clusters MSI et prise en charge de l’attachement d’acr à des clusters MSI</span><span class="sxs-lookup"><span data-stu-id="88779-246">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="88779-247">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-247">AMS</span></span>

* <span data-ttu-id="88779-248">Correctif #12469 : échec de l’ajout de Fairplay content-key-policy en raison de problèmes avec le paramètre « ask »</span><span class="sxs-lookup"><span data-stu-id="88779-248">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-249">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-249">AppConfig</span></span>

* <span data-ttu-id="88779-250">Ajout de --skip-keyvault pour l’exportation de kv</span><span class="sxs-lookup"><span data-stu-id="88779-250">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-251">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-251">AppService</span></span>

* <span data-ttu-id="88779-252">Correctif #12509 : Suppression de la balise d’az webapp up par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-252">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="88779-253">az functionapp create : Mise à jour du menu d’aide --runtime-version et ajout d’un avertissement quand l’utilisateur spécifie --runtime-version pour dotnet</span><span class="sxs-lookup"><span data-stu-id="88779-253">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="88779-254">az functionapp create : Mise à jour du mode de définition de javaVersion pour les applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="88779-254">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="88779-255">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-255">ARM</span></span>

* <span data-ttu-id="88779-256">az deployment create/validate : Utilisation du --handle-extended-json-format par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-256">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="88779-257">az lock create : Ajout d’exemples de création de sous-ressources dans la documentation d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-257">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="88779-258">az deployment {group/mg/sub/tenant} list : Prise en charge du filtrage provisioningState</span><span class="sxs-lookup"><span data-stu-id="88779-258">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="88779-259">az deployment : Correction du bogue d’analyse pour les commentaires sous le dernier argument</span><span class="sxs-lookup"><span data-stu-id="88779-259">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="88779-260">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-260">Backup</span></span>

* <span data-ttu-id="88779-261">Ajout de plusieurs fonctionnalités de restauration de fichiers</span><span class="sxs-lookup"><span data-stu-id="88779-261">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="88779-262">Ajout de la prise en charge de la sauvegarde des disques de système d’exploitation uniquement</span><span class="sxs-lookup"><span data-stu-id="88779-262">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="88779-263">Ajout du paramètre restore-as-unmanaged-disk pour spécifier une restauration non gérée</span><span class="sxs-lookup"><span data-stu-id="88779-263">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="88779-264">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-264">Compute</span></span>

* <span data-ttu-id="88779-265">az vm create : Ajout de l’option NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="88779-265">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="88779-266">az vmss create/update : suppression de la balise d’aperçu des réparations automatiques vmss</span><span class="sxs-lookup"><span data-stu-id="88779-266">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="88779-267">az vm update : Prise en charge de --workspace</span><span class="sxs-lookup"><span data-stu-id="88779-267">az vm update: Support --workspace</span></span>
* <span data-ttu-id="88779-268">Correction d’un bogue dans le code d’initialisation VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="88779-268">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="88779-269">Mise à niveau de VMAccessAgent vers la version 2.4</span><span class="sxs-lookup"><span data-stu-id="88779-269">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="88779-270">az vmss set-orchestration-service-state : prise en charge de l’état de la définition du service d’orchestration vmss</span><span class="sxs-lookup"><span data-stu-id="88779-270">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="88779-271">Mise à niveau de la version d’API de disque vers la version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="88779-271">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="88779-272">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="88779-272">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-273">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-273">Cosmos DB</span></span>

* <span data-ttu-id="88779-274">Correction de l’option --type manquante pour les redirections de dépréciation</span><span class="sxs-lookup"><span data-stu-id="88779-274">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="88779-275">Docker</span><span class="sxs-lookup"><span data-stu-id="88779-275">Docker</span></span>

* <span data-ttu-id="88779-276">Mise à jour vers Alpine 3.11 et Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="88779-276">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="88779-277">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-277">Extension</span></span>

* <span data-ttu-id="88779-278">Autorisation de charger des extensions dans le chemin système via des packages</span><span class="sxs-lookup"><span data-stu-id="88779-278">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-279">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-279">HDInsight</span></span>

* <span data-ttu-id="88779-280">(az hdinsight create:) Les clients du support spécifient une version TLS minimale prise en charge à l’aide du paramètre `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="88779-280">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="88779-281">La valeur autorisée est 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="88779-281">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="88779-282">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-282">IoT</span></span>

* <span data-ttu-id="88779-283">Ajout de codeowner</span><span class="sxs-lookup"><span data-stu-id="88779-283">Add codeowner</span></span>
* <span data-ttu-id="88779-284">az iot hub create : changement de la référence SKU par défaut S1 en F1</span><span class="sxs-lookup"><span data-stu-id="88779-284">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="88779-285">iot hub : Prise en charge d’IotHub dans le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="88779-285">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="88779-286">IotCentral</span><span class="sxs-lookup"><span data-stu-id="88779-286">IoTCentral</span></span>

* <span data-ttu-id="88779-287">Mise à jour des détails d’erreur, du modèle d’application par défaut et du message d’invite</span><span class="sxs-lookup"><span data-stu-id="88779-287">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-288">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-288">KeyVault</span></span>

* <span data-ttu-id="88779-289">Prise en charge de la sauvegarde/restauration de certificat</span><span class="sxs-lookup"><span data-stu-id="88779-289">Support certificate backup/restore</span></span>
* <span data-ttu-id="88779-290">keyvault create/update : Prise en charge de --retention-days</span><span class="sxs-lookup"><span data-stu-id="88779-290">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="88779-291">Plus d’affichage des clés/secrets managés lors du listing</span><span class="sxs-lookup"><span data-stu-id="88779-291">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="88779-292">az keyvault create : prise en charge de `--network-acls`, `--network-acls-ips` et `--network-acls-vnets` pour spécifier des règles réseau lors de la création de coffres</span><span class="sxs-lookup"><span data-stu-id="88779-292">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="88779-293">Verrouillage</span><span class="sxs-lookup"><span data-stu-id="88779-293">Lock</span></span>

* <span data-ttu-id="88779-294">Correction de bogue pour az lock delete : az lock delete ne fonctionne pas sur Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="88779-294">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-295">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-295">Monitor</span></span>

* <span data-ttu-id="88779-296">az monitor clone : prise en charge des règles de clonage de métriques d’une ressource à une autre</span><span class="sxs-lookup"><span data-stu-id="88779-296">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="88779-297">Correctif IcM179210086 : impossible de créer une alerte de métrique personnalisée pour la métrique Application Insights</span><span class="sxs-lookup"><span data-stu-id="88779-297">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="88779-298">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="88779-298">NetAppFiles</span></span>

* <span data-ttu-id="88779-299">az volume create : Autorisation des volumes de protection des données à ajouter des opérations de réplication : approuver, suspendre, reprendre, état, supprimer</span><span class="sxs-lookup"><span data-stu-id="88779-299">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="88779-300">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-300">Network</span></span>

* <span data-ttu-id="88779-301">az network application-gateway waf-policy managed-rule rule-set add : prise en charge de Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="88779-301">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="88779-302">network watcher flow-log show: correction d’une information de dépréciation fausse</span><span class="sxs-lookup"><span data-stu-id="88779-302">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="88779-303">Prise en charge des noms d’hôte dans l’écouteur de passerelle d’application</span><span class="sxs-lookup"><span data-stu-id="88779-303">support host names in application gateway listener</span></span>
* <span data-ttu-id="88779-304">az network nat gateway : prise en charge de la création d’une ressource vide sans IP publique ni préfixe d’IP publique</span><span class="sxs-lookup"><span data-stu-id="88779-304">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="88779-305">Prise en charge de la génération de passerelles VPN</span><span class="sxs-lookup"><span data-stu-id="88779-305">Support vpn gateway generation</span></span>
* <span data-ttu-id="88779-306">Prise en charge de `--if-none-match` dans `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="88779-306">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-307">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-307">Packaging</span></span>

* <span data-ttu-id="88779-308">Arrêt de la prise en charge de Python 3.5</span><span class="sxs-lookup"><span data-stu-id="88779-308">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="88779-309">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-309">Profile</span></span>

* <span data-ttu-id="88779-310">az login : Affichage d’un avertissement pour l’erreur MFA</span><span class="sxs-lookup"><span data-stu-id="88779-310">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-311">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-311">RDBMS</span></span>

* <span data-ttu-id="88779-312">Ajout de commandes de gestion de clés de chiffrement de données de serveur pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="88779-312">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="88779-313">10 mars 2020</span><span class="sxs-lookup"><span data-stu-id="88779-313">March 10, 2020</span></span>

<span data-ttu-id="88779-314">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="88779-314">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="88779-315">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-315">ACR</span></span>

* <span data-ttu-id="88779-316">Correctif : `az acr login` déclenche une erreur de manière erronée</span><span class="sxs-lookup"><span data-stu-id="88779-316">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="88779-317">Ajout d’une nouvelle commande `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="88779-317">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="88779-318">Ajout d’un lien privé et de la prise en charge CMK</span><span class="sxs-lookup"><span data-stu-id="88779-318">Add private link and CMK support</span></span>
* <span data-ttu-id="88779-319">Ajout de la commande « private-link-resource list »</span><span class="sxs-lookup"><span data-stu-id="88779-319">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="88779-320">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-320">AKS</span></span>

* <span data-ttu-id="88779-321">Correction de la navigation aks dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-321">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="88779-322">az aks : correction de la supervision des erreurs NoneType addon et agentpool</span><span class="sxs-lookup"><span data-stu-id="88779-322">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="88779-323">Ajout de --nodepool-tags au pool de nœuds lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-323">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="88779-324">Ajout de --tags lors de l’ajout ou de la mise à jour d’un nodepool à un cluster</span><span class="sxs-lookup"><span data-stu-id="88779-324">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="88779-325">aks create : ajout de `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="88779-325">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="88779-326">Ajout de --nodepool-labels lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-326">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="88779-327">Ajout de --labels lors de l’ajout d’un nouveau nodepool à un cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-327">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="88779-328">Ajout d’un caractère / manquant à l’URL de tableau de bord</span><span class="sxs-lookup"><span data-stu-id="88779-328">add missing / in the dashboard url</span></span>
* <span data-ttu-id="88779-329">Prise en charge de la création de clusters AKS activant l’identité managée</span><span class="sxs-lookup"><span data-stu-id="88779-329">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="88779-330">az aks : validation du plug-in réseau pour qu’il soit « azure » ou « kubenet »</span><span class="sxs-lookup"><span data-stu-id="88779-330">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="88779-331">az aks : Ajout de la prise en charge des clés de session AAD</span><span class="sxs-lookup"><span data-stu-id="88779-331">az aks: Add aad session key support</span></span>
* <span data-ttu-id="88779-332">[CHANGEMENT CASSANT] az aks : prise en charge des modifications MSI pour GF et BF pour omsagent (supervision de conteneur) (#1)</span><span class="sxs-lookup"><span data-stu-id="88779-332">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="88779-333">az aks use-dev-spaces : ajout de l’option de type de point de terminaison à la commande use-dev-spaces pour personnaliser le point de terminaison créé sur un contrôleur Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="88779-333">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-334">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-334">AppConfig</span></span>

* <span data-ttu-id="88779-335">Déblocage de l’utilisation de « kv set » pour ajouter la fonctionnalité et la référence de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="88779-335">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-336">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-336">AppService</span></span>

* <span data-ttu-id="88779-337">az webapp create : résolution d’un problème lors de l’exécution de la commande avec --runtime</span><span class="sxs-lookup"><span data-stu-id="88779-337">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="88779-338">az functionapp deployment source config-zip : ajout d’un message d’erreur si le nom du groupe de ressources ou de la fonction n’est pas valide ou n’existe pas</span><span class="sxs-lookup"><span data-stu-id="88779-338">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="88779-339">functionapp create : correction du message d’avertissement qui s’affiche aujourd’hui avec `functionapp create`, qui mentionne un indicateur `--functions_version` mais utilise de manière erronée un `_` au lieu d’un `-` dans le nom de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="88779-339">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="88779-340">az functionapp create : mise à jour de la façon dont linuxFxVersion et le nom de l’image conteneur étaient définis pour les applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="88779-340">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="88779-341">az functionapp deployment source config-zip : résolution d’un problème dû à une condition de concurrence en cas de modification des paramètres d’application pendant le déploiement de fichier zip, provoquant des erreurs 5xx lors du déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-341">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="88779-342">Correctif 5720946 : az webapp backup ne parvient pas à définir le nom</span><span class="sxs-lookup"><span data-stu-id="88779-342">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="88779-343">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-343">ARM</span></span>

* <span data-ttu-id="88779-344">az resource : amélioration des exemples du module de ressources</span><span class="sxs-lookup"><span data-stu-id="88779-344">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="88779-345">az policy assignment list : prise en charge de l’énumération des affectations de stratégie au niveau de l’étendue du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="88779-345">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="88779-346">Ajout de `az deployment group` et `az deployment operation group` pour le déploiement de modèle au niveau des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="88779-346">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="88779-347">Il s’agit d’un doublon de `az group deployment` et `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="88779-347">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="88779-348">Ajout de `az deployment sub` et `az deployment operation sub` pour le déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="88779-348">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="88779-349">Il s’agit d’un doublon de `az deployment` et `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="88779-349">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="88779-350">Ajout de `az deployment mg` et `az deployment operation mg` pour le déploiement de modèle au niveau des groupes de gestion</span><span class="sxs-lookup"><span data-stu-id="88779-350">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="88779-351">Ajout de `az deployment tenant` et `az deployment operation tenant` pour le déploiement de modèle à l’étendue du locataire</span><span class="sxs-lookup"><span data-stu-id="88779-351">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="88779-352">az policy assignment create : ajout d’une description au paramètre `--location`</span><span class="sxs-lookup"><span data-stu-id="88779-352">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="88779-353">az group deployment create : ajout du paramètre `--aux-tenants` pour prendre en charge les locataires croisés</span><span class="sxs-lookup"><span data-stu-id="88779-353">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-354">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-354">CDN</span></span>

* <span data-ttu-id="88779-355">Ajouter de commandes WAF CDN</span><span class="sxs-lookup"><span data-stu-id="88779-355">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="88779-356">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-356">Compute</span></span>

* <span data-ttu-id="88779-357">az sig image-version : ajout de --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="88779-357">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="88779-358">az ppg show: ajout de --colocation-status pour permettre l’extraction de l’état de colocalisation de toutes les ressources dans le groupe de placement de proximité</span><span class="sxs-lookup"><span data-stu-id="88779-358">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="88779-359">az vmss create/update : prise en charge des réparations automatiques</span><span class="sxs-lookup"><span data-stu-id="88779-359">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="88779-360">[CHANGEMENT CASSANT] az image template : template a été renommé builder</span><span class="sxs-lookup"><span data-stu-id="88779-360">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="88779-361">az image builder create : ajout de --image-template</span><span class="sxs-lookup"><span data-stu-id="88779-361">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-362">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-362">Cosmos DB</span></span>

* <span data-ttu-id="88779-363">Ajout d’applets de commande de déclencheur, de procédure stockée SQL et de fonctions définies par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="88779-363">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="88779-364">az cosmosdb create : ajout de --key-uri pour prendre en charge l’ajout d’informations de chiffrement de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="88779-364">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-365">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-365">KeyVault</span></span>

* <span data-ttu-id="88779-366">keyvault create : activation de la suppression réversible par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-366">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-367">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-367">Monitor</span></span>

* <span data-ttu-id="88779-368">az monitor metrics alert create : prise en charge de `~` dans `--condition`</span><span class="sxs-lookup"><span data-stu-id="88779-368">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="88779-369">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-369">Network</span></span>

* <span data-ttu-id="88779-370">az network application-gateway rewrite-rule create : prise en charge de la configuration d’URL</span><span class="sxs-lookup"><span data-stu-id="88779-370">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="88779-371">az network dns zone import : --zone-name respectera la casse à l’avenir</span><span class="sxs-lookup"><span data-stu-id="88779-371">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="88779-372">az network private-endpoint/private-link-service : suppression de l’étiquette d’aperçu</span><span class="sxs-lookup"><span data-stu-id="88779-372">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="88779-373">az network bastion : prise en charge de bastion</span><span class="sxs-lookup"><span data-stu-id="88779-373">az network bastion: support bastion</span></span>
* <span data-ttu-id="88779-374">az network vnet list-available-ips : prise en charge de l’énumération des adresses IP disponibles sur un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="88779-374">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="88779-375">az network watcher flow-log create/list/delete/update : ajout de nouvelles commandes pour gérer le journal de flux d’observateur et l’exposition de --location pour identifier explicitement l’observateur</span><span class="sxs-lookup"><span data-stu-id="88779-375">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="88779-376">az network watcher flow-log configure : dépréciée</span><span class="sxs-lookup"><span data-stu-id="88779-376">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="88779-377">az network watcher flow-log show : prise en charge de --location et de --name pour obtenir un résultat au format ARM. L’ancienne sortie mise en forme est dépréciée</span><span class="sxs-lookup"><span data-stu-id="88779-377">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="88779-378">Stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-378">Policy</span></span>

* <span data-ttu-id="88779-379">az policy assignment create : correction du bogue qui générait automatiquement un nom d’attribution de stratégie dépassant la limite</span><span class="sxs-lookup"><span data-stu-id="88779-379">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-380">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-380">RBAC</span></span>

* <span data-ttu-id="88779-381">az ad group show : correction du bogue qui faisait que --group était traité comme un problème Regex</span><span class="sxs-lookup"><span data-stu-id="88779-381">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-382">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-382">RDBMS</span></span>

* <span data-ttu-id="88779-383">Passage du SDK azure-mgmt-rdbms à la version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-383">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="88779-384">az postgres private-endpoint-connection : gestion des connexions de point de terminaison privé postgres</span><span class="sxs-lookup"><span data-stu-id="88779-384">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="88779-385">az postgres private-link-resource : gestion des ressources de lien privé postgres</span><span class="sxs-lookup"><span data-stu-id="88779-385">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="88779-386">az mysql private-endpoint-connection : gestion des connexions de point de terminaison privé mysql</span><span class="sxs-lookup"><span data-stu-id="88779-386">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="88779-387">az mysql private-link-resource : gestion des ressources de lien privé mysql</span><span class="sxs-lookup"><span data-stu-id="88779-387">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="88779-388">az mariadb private-endpoint-connection : gestion des connexions de point de terminaison privé mariadb</span><span class="sxs-lookup"><span data-stu-id="88779-388">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="88779-389">az mariadb private-link-resource : gestion des ressources de lien privé mariadb</span><span class="sxs-lookup"><span data-stu-id="88779-389">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="88779-390">Mise à jour des tests de point de terminaison privé SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-390">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="88779-391">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-391">SQL</span></span>

* <span data-ttu-id="88779-392">Sql midb ; ajout de list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="88779-392">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="88779-393">(sql server create :) Ajout de l’indicateur facultatif « Enable »/« Disable » d’accès au réseau public à sql server create</span><span class="sxs-lookup"><span data-stu-id="88779-393">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="88779-394">(sql server update :) modifications du client</span><span class="sxs-lookup"><span data-stu-id="88779-394">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="88779-395">Ajout de propriété minimal_tls_version pour MI et SQL DB</span><span class="sxs-lookup"><span data-stu-id="88779-395">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="88779-396">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-396">Storage</span></span>

* <span data-ttu-id="88779-397">az storage blob delete-batch : comportement incorrect de l’indicateur `--dryrun`</span><span class="sxs-lookup"><span data-stu-id="88779-397">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="88779-398">az storage account network-rule add (correctif de bogue) : l’opération d’ajout doit être idempotent</span><span class="sxs-lookup"><span data-stu-id="88779-398">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="88779-399">az storage account create/update : Ajout de la prise en charge des préférences de routage</span><span class="sxs-lookup"><span data-stu-id="88779-399">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="88779-400">Mise à niveau de la version azure-mgmt-storage vers 8.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-400">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="88779-401">az storage container immutability create : ajout du paramètre --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="88779-401">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="88779-402">az storage account private-link-resource list : ajout de la prise en charge de l’énumération des ressources de lien privé pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-402">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="88779-403">az storage account private-endpoint-connection approve/reject/show/delete : prise en charge de la gestion des connexions de point de terminaison privé</span><span class="sxs-lookup"><span data-stu-id="88779-403">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="88779-404">az storage account blob-service-properties update : ajout de --enable-restore-policy et --restore-days</span><span class="sxs-lookup"><span data-stu-id="88779-404">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="88779-405">az storage blob restore : ajout de la prise en charge de la restauration des plages d’objets blob</span><span class="sxs-lookup"><span data-stu-id="88779-405">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="88779-406">18 février 2020</span><span class="sxs-lookup"><span data-stu-id="88779-406">February 18, 2020</span></span>

<span data-ttu-id="88779-407">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="88779-407">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="88779-408">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-408">ACR</span></span>

* <span data-ttu-id="88779-409">Ajoute un nouvel argument `--expose-token` pour `az acr login`</span><span class="sxs-lookup"><span data-stu-id="88779-409">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="88779-410">Corrige la sortie incorrecte de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="88779-410">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="88779-411">az acr login : lève une CLIError si des erreurs sont retournées par la commande docker</span><span class="sxs-lookup"><span data-stu-id="88779-411">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="88779-412">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-412">ACS</span></span>

* <span data-ttu-id="88779-413">aks create/update : ajoute la validation `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="88779-413">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="88779-414">Aladdin</span><span class="sxs-lookup"><span data-stu-id="88779-414">Aladdin</span></span>

* <span data-ttu-id="88779-415">Analyse les exemples générés dans le _help.py des commandes</span><span class="sxs-lookup"><span data-stu-id="88779-415">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="88779-416">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-416">AMS</span></span>

* <span data-ttu-id="88779-417">az ams est désormais en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="88779-417">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-418">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-418">AppConfig</span></span>

* <span data-ttu-id="88779-419">Modifie le message d’aide pour exclure les filtres de clé ou d’étiquette non pris en charge</span><span class="sxs-lookup"><span data-stu-id="88779-419">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="88779-420">Supprimer l’étiquette d’aperçu pour la plupart des commandes, à l’exception des indicateurs d’identité managée et de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="88779-420">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="88779-421">Ajoute une clé gérée par le client lors de la mise à jour des magasins</span><span class="sxs-lookup"><span data-stu-id="88779-421">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-422">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-422">AppService</span></span>

* <span data-ttu-id="88779-423">az webapp list-runtimes : correction du bogue concernant list-runtimes</span><span class="sxs-lookup"><span data-stu-id="88779-423">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="88779-424">Ajoute az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="88779-424">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="88779-425">Ajoute la prise en charge des applications de fonction v3 et du nœud 12</span><span class="sxs-lookup"><span data-stu-id="88779-425">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="88779-426">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-426">ARM</span></span>

* <span data-ttu-id="88779-427">az policy assignment create : correction du message d’erreur lorsque le paramètre `--policy` n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="88779-427">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="88779-428">az group deployment create : correction de l’erreur « stat: path too long for Windows » (Chemin trop long pour Windows) lors de l’utilisation d’un fichier parameters.json volumineux</span><span class="sxs-lookup"><span data-stu-id="88779-428">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="88779-429">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-429">Backup</span></span>

* <span data-ttu-id="88779-430">Correction du flux de récupération au niveau de l’élément dans OLR</span><span class="sxs-lookup"><span data-stu-id="88779-430">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="88779-431">Ajout de la prise en charge de la restauration sous forme de fichiers pour les bases de données SQL et SAP</span><span class="sxs-lookup"><span data-stu-id="88779-431">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="88779-432">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-432">Compute</span></span>

* <span data-ttu-id="88779-433">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="88779-433">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="88779-434">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="88779-434">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="88779-435">az vm host : supprime l’étiquette d’aperçu pour `vm host` et `vm host group`</span><span class="sxs-lookup"><span data-stu-id="88779-435">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="88779-436">[CHANGEMENT CASSANT] Correctif n° 10728 : `az vm create` Création automatique d’un sous-réseau si un réseau virtuel est spécifié et s’il n’existe pas de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="88779-436">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="88779-437">Amélioration de la robustesse de la liste d’images de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="88779-437">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="88779-438">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="88779-438">Eventhub</span></span>

* <span data-ttu-id="88779-439">Prise en charge d’Azure Stack pour le profil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="88779-439">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-440">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-440">KeyVault</span></span>

* <span data-ttu-id="88779-441">az keyvault key create : ajouter une nouvelle valeur `import` pour le paramètre `--ops`</span><span class="sxs-lookup"><span data-stu-id="88779-441">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="88779-442">az keyvault key list-versions : prise en charge du paramètre `--id` pour la spécification des clés</span><span class="sxs-lookup"><span data-stu-id="88779-442">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="88779-443">Prise en charge des connexions de points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="88779-443">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="88779-444">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-444">Network</span></span>

* <span data-ttu-id="88779-445">Passage à azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-445">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="88779-446">az network private-link-service update/create: support --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="88779-446">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="88779-447">Ajout de la fonctionnalité Moniteur de connexion v2</span><span class="sxs-lookup"><span data-stu-id="88779-447">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-448">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-448">Packaging</span></span>

* <span data-ttu-id="88779-449">[CHANGEMENT CASSANT] Python 2.7 n’est plus pris en charge</span><span class="sxs-lookup"><span data-stu-id="88779-449">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="88779-450">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-450">Profile</span></span>

* <span data-ttu-id="88779-451">Aperçu : Ajoutez les nouveaux attributs `homeTenantId` et `managedByTenants` aux comptes d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="88779-451">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="88779-452">Réexécutez `az login` pour que les modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="88779-452">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="88779-453">az login : affiche un avertissement lorsqu’un abonnement est listé par plusieurs locataires et s’affiche par défaut pour le premier.</span><span class="sxs-lookup"><span data-stu-id="88779-453">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="88779-454">Pour sélectionner un locataire lors de l’accès à cet abonnement, ajoutez `--tenant` dans `az login`</span><span class="sxs-lookup"><span data-stu-id="88779-454">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="88779-455">Role</span><span class="sxs-lookup"><span data-stu-id="88779-455">Role</span></span>

* <span data-ttu-id="88779-456">az role assignment create : correction de l’erreur lors de laquelle l’attribution d’un rôle à un principal de service par nom d’affichage générait une erreur HTTP 400</span><span class="sxs-lookup"><span data-stu-id="88779-456">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="88779-457">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-457">SQL</span></span>

* <span data-ttu-id="88779-458">Mise à jour de l’applet de commande SQL Managed Instance `az sql mi update` avec deux nouveaux paramètres : tier et family</span><span class="sxs-lookup"><span data-stu-id="88779-458">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="88779-459">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-459">Storage</span></span>

* <span data-ttu-id="88779-460">[CHANGEMENT CASSANT] `az storage account create` : Remplacement du type de compte de stockage par défaut par StorageV2</span><span class="sxs-lookup"><span data-stu-id="88779-460">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="88779-461">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="88779-461">February 04, 2020</span></span>

<span data-ttu-id="88779-462">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="88779-462">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="88779-463">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-463">ACS</span></span>

* <span data-ttu-id="88779-464">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="88779-464">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="88779-465">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="88779-465">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="88779-466">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-466">ACR</span></span>

* <span data-ttu-id="88779-467">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="88779-467">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="88779-468">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="88779-468">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="88779-469">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="88779-469">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="88779-470">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-470">AKS</span></span>

* <span data-ttu-id="88779-471">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="88779-471">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-472">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-472">AppConfig</span></span>

* <span data-ttu-id="88779-473">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="88779-473">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="88779-474">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="88779-474">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="88779-475">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="88779-475">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="88779-476">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="88779-476">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="88779-477">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="88779-477">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-478">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-478">AppService</span></span>

* <span data-ttu-id="88779-479">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="88779-479">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="88779-480">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="88779-480">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="88779-481">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-481">ARM</span></span>

* <span data-ttu-id="88779-482">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="88779-482">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="88779-483">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="88779-483">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="88779-484">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="88779-484">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="88779-485">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="88779-485">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="88779-486">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="88779-486">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="88779-487">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="88779-487">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="88779-488">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="88779-488">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-489">BotService</span><span class="sxs-lookup"><span data-stu-id="88779-489">BotService</span></span>

* <span data-ttu-id="88779-490">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="88779-490">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="88779-491">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="88779-491">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-492">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-492">CDN</span></span>

* <span data-ttu-id="88779-493">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="88779-493">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="88779-494">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="88779-494">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="88779-495">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="88779-495">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="88779-496">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-496">Deployment Manager</span></span>

* <span data-ttu-id="88779-497">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="88779-497">Add list operation for all resources.</span></span>
* <span data-ttu-id="88779-498">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="88779-498">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="88779-499">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="88779-499">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="88779-500">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-500">IoT</span></span>

* <span data-ttu-id="88779-501">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="88779-501">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="88779-502">IoT Central</span><span class="sxs-lookup"><span data-stu-id="88779-502">IoT Central</span></span>

* <span data-ttu-id="88779-503">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="88779-503">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-504">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-504">Key Vault</span></span>

* <span data-ttu-id="88779-505">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="88779-505">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="88779-506">Divers</span><span class="sxs-lookup"><span data-stu-id="88779-506">Misc</span></span>

* <span data-ttu-id="88779-507">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="88779-507">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="88779-508">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-508">Network</span></span>

* <span data-ttu-id="88779-509">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="88779-509">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="88779-510">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="88779-510">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="88779-511">Stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-511">Policy</span></span>

* <span data-ttu-id="88779-512">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="88779-512">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="88779-513">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="88779-513">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="88779-514">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-514">Profile</span></span>

* <span data-ttu-id="88779-515">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-515">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-516">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-516">RBAC</span></span>

* <span data-ttu-id="88779-517">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="88779-517">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="88779-518">Sécurité</span><span class="sxs-lookup"><span data-stu-id="88779-518">Security</span></span>

* <span data-ttu-id="88779-519">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="88779-519">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="88779-520">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-520">SQL</span></span>

* <span data-ttu-id="88779-521">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="88779-521">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="88779-522">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="88779-522">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="88779-523">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="88779-523">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="88779-524">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="88779-524">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="88779-525">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="88779-525">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="88779-526">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="88779-526">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="88779-527">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-527">Storage</span></span>

* <span data-ttu-id="88779-528">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="88779-528">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="88779-529">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="88779-529">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="88779-530">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="88779-530">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="88779-531">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="88779-531">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="88779-532">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="88779-532">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="88779-533">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="88779-533">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="88779-534">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="88779-534">ServiceFabric</span></span>

* <span data-ttu-id="88779-535">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="88779-535">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="88779-536">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="88779-536">January 13, 2020</span></span>

<span data-ttu-id="88779-537">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="88779-537">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="88779-538">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-538">Compute</span></span>

* <span data-ttu-id="88779-539">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="88779-539">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="88779-540">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="88779-540">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="88779-541">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-541">Storage</span></span>

* <span data-ttu-id="88779-542">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="88779-542">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="88779-543">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="88779-543">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="88779-544">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="88779-544">January 07, 2020</span></span>

<span data-ttu-id="88779-545">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="88779-545">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="88779-546">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-546">ACR</span></span>

* <span data-ttu-id="88779-547">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="88779-547">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="88779-548">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="88779-548">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-549">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-549">AppConfig</span></span>

* <span data-ttu-id="88779-550">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="88779-550">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="88779-551">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-551">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="88779-552">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="88779-552">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-553">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-553">AppService</span></span>

* <span data-ttu-id="88779-554">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="88779-554">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="88779-555">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-555">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="88779-556">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="88779-556">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="88779-557">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-557">ARM</span></span>

* <span data-ttu-id="88779-558">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="88779-558">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="88779-559">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-559">Backup</span></span>

* <span data-ttu-id="88779-560">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="88779-560">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="88779-561">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="88779-561">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="88779-562">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="88779-562">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="88779-563">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-563">Compute</span></span>

* <span data-ttu-id="88779-564">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="88779-564">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="88779-565">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="88779-565">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="88779-566">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="88779-566">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-567">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-567">HDInsight</span></span>

* <span data-ttu-id="88779-568">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="88779-568">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="88779-569">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="88779-569">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="88779-570">Divers</span><span class="sxs-lookup"><span data-stu-id="88779-570">Misc.</span></span>

* <span data-ttu-id="88779-571">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="88779-571">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="88779-572">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="88779-572">Event Hubs</span></span>

* <span data-ttu-id="88779-573">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="88779-573">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="88779-574">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="88779-574">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="88779-575">Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-575">Service Bus</span></span>

* <span data-ttu-id="88779-576">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="88779-576">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="88779-577">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="88779-577">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-578">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-578">RBAC</span></span>

* <span data-ttu-id="88779-579">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="88779-579">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="88779-580">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-580">Storage</span></span>

* <span data-ttu-id="88779-581">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="88779-581">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="88779-582">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="88779-582">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="88779-583">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="88779-583">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="88779-584">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-584">December 17, 2019</span></span>

<span data-ttu-id="88779-585">2.0.78</span><span class="sxs-lookup"><span data-stu-id="88779-585">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="88779-586">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-586">ACR</span></span>

* <span data-ttu-id="88779-587">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="88779-587">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="88779-588">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-588">ACS</span></span>

* <span data-ttu-id="88779-589">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="88779-589">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="88779-590">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-590">AMS</span></span>

* <span data-ttu-id="88779-591">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="88779-591">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-592">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-592">AppConfig</span></span>

* <span data-ttu-id="88779-593">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="88779-593">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="88779-594">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="88779-594">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="88779-595">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="88779-595">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-596">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-596">AppService</span></span>

* <span data-ttu-id="88779-597">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="88779-597">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="88779-598">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="88779-598">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="88779-599">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="88779-599">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="88779-600">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="88779-600">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="88779-601">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-601">ARM</span></span>

* <span data-ttu-id="88779-602">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-602">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="88779-603">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="88779-603">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="88779-604">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="88779-604">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="88779-605">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-605">Backup</span></span>

* <span data-ttu-id="88779-606">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="88779-606">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-607">BotService</span><span class="sxs-lookup"><span data-stu-id="88779-607">BotService</span></span>

* <span data-ttu-id="88779-608">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="88779-608">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="88779-609">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="88779-609">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="88779-610">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="88779-610">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="88779-611">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="88779-611">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="88779-612">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="88779-612">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="88779-613">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="88779-613">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="88779-614">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="88779-614">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="88779-615">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="88779-615">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="88779-616">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="88779-616">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="88779-617">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-617">Compute</span></span>

* <span data-ttu-id="88779-618">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="88779-618">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="88779-619">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="88779-619">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="88779-620">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="88779-620">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="88779-621">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="88779-621">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="88779-622">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="88779-622">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="88779-623">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="88779-623">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="88779-624">Core</span><span class="sxs-lookup"><span data-stu-id="88779-624">Core</span></span>

* <span data-ttu-id="88779-625">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="88779-625">Removed support for Python 3.4</span></span>
* <span data-ttu-id="88779-626">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="88779-626">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="88779-627">DLS</span><span class="sxs-lookup"><span data-stu-id="88779-627">DLS</span></span>

* <span data-ttu-id="88779-628">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="88779-628">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="88779-629">Installer</span><span class="sxs-lookup"><span data-stu-id="88779-629">Install</span></span>

* <span data-ttu-id="88779-630">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="88779-630">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="88779-631">IOT</span><span class="sxs-lookup"><span data-stu-id="88779-631">IOT</span></span>

* <span data-ttu-id="88779-632">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="88779-632">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="88779-633">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="88779-633">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-634">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-634">Key Vault</span></span>

* <span data-ttu-id="88779-635">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-635">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="88779-636">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="88779-636">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="88779-637">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="88779-637">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="88779-638">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="88779-638">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="88779-639">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="88779-639">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="88779-640">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-640">Network</span></span>

* <span data-ttu-id="88779-641">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="88779-641">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="88779-642">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-642">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="88779-643">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="88779-643">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="88779-644">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="88779-644">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="88779-645">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="88779-645">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-646">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-646">Packaging</span></span>

* <span data-ttu-id="88779-647">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="88779-647">Added back edge builds for pip install</span></span>
* <span data-ttu-id="88779-648">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="88779-648">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="88779-649">Stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-649">Policy</span></span>

* <span data-ttu-id="88779-650">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="88779-650">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="88779-651">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="88779-651">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="88779-652">Redis</span><span class="sxs-lookup"><span data-stu-id="88779-652">Redis</span></span>

* <span data-ttu-id="88779-653">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="88779-653">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="88779-654">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="88779-654">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="88779-655">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="88779-655">ServiceFabric</span></span>

* <span data-ttu-id="88779-656">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="88779-656">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="88779-657">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="88779-657">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="88779-658">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-658">SQL</span></span>

* <span data-ttu-id="88779-659">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="88779-659">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="88779-660">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-660">Storage</span></span>

* <span data-ttu-id="88779-661">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="88779-661">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="88779-662">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="88779-662">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="88779-663">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="88779-663">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="88779-664">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="88779-664">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="88779-665">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="88779-665">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="88779-666">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-666">November 26, 2019</span></span>

<span data-ttu-id="88779-667">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="88779-667">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="88779-668">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-668">ACR</span></span>

* <span data-ttu-id="88779-669">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="88779-669">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="88779-670">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="88779-670">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="88779-671">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="88779-671">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="88779-672">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="88779-672">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="88779-673">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-673">AKS</span></span>

* <span data-ttu-id="88779-674">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="88779-674">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-675">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-675">AppConfig</span></span>

* <span data-ttu-id="88779-676">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="88779-676">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="88779-677">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="88779-677">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="88779-678">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="88779-678">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="88779-679">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-679">AppService</span></span>

* <span data-ttu-id="88779-680">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="88779-680">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="88779-681">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="88779-681">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="88779-682">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="88779-682">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="88779-683">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-683">Backup</span></span>

* <span data-ttu-id="88779-684">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="88779-684">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="88779-685">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="88779-685">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="88779-686">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-686">Compute</span></span>

* <span data-ttu-id="88779-687">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="88779-687">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="88779-688">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="88779-688">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="88779-689">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="88779-689">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="88779-690">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="88779-690">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="88779-691">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="88779-691">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="88779-692">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="88779-692">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="88779-693">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-693">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="88779-694">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="88779-694">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="88779-695">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="88779-695">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="88779-696">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="88779-696">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="88779-697">IOT</span><span class="sxs-lookup"><span data-stu-id="88779-697">IOT</span></span>

* <span data-ttu-id="88779-698">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="88779-698">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="88779-699">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="88779-699">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="88779-700">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="88779-700">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-701">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-701">Key Vault</span></span>

* <span data-ttu-id="88779-702">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="88779-702">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="88779-703">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="88779-703">NetAppFiles</span></span>

* <span data-ttu-id="88779-704">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="88779-704">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="88779-705">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-705">Network</span></span>

* <span data-ttu-id="88779-706">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="88779-706">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="88779-707">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="88779-707">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="88779-708">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="88779-708">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="88779-709">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="88779-709">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="88779-710">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="88779-710">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="88779-711">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="88779-711">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="88779-712">Packaging</span><span class="sxs-lookup"><span data-stu-id="88779-712">Packaging</span></span>

* <span data-ttu-id="88779-713">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="88779-713">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="88779-714">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="88779-714">Added support for Python 3.8</span></span>
* <span data-ttu-id="88779-715">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="88779-715">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="88779-716">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-716">Profile</span></span>

* <span data-ttu-id="88779-717">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="88779-717">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="88779-718">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="88779-718">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="88779-719">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="88779-719">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="88779-720">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="88779-720">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="88779-721">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="88779-721">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-722">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-722">RBAC</span></span>

* <span data-ttu-id="88779-723">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="88779-723">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="88779-724">Redis</span><span class="sxs-lookup"><span data-stu-id="88779-724">Redis</span></span>

* <span data-ttu-id="88779-725">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="88779-725">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="88779-726">Réservations</span><span class="sxs-lookup"><span data-stu-id="88779-726">Reservations</span></span>

* <span data-ttu-id="88779-727">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="88779-727">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="88779-728">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="88779-728">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="88779-729">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="88779-729">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="88779-730">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="88779-730">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="88779-731">Rest</span><span class="sxs-lookup"><span data-stu-id="88779-731">Rest</span></span>
* <span data-ttu-id="88779-732">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="88779-732">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="88779-733">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-733">SQL</span></span>

* <span data-ttu-id="88779-734">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="88779-734">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="88779-735">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-735">Storage</span></span>

* <span data-ttu-id="88779-736">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="88779-736">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="88779-737">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="88779-737">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="88779-738">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="88779-738">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="88779-739">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="88779-739">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="88779-740">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-740">November 4, 2019</span></span>

<span data-ttu-id="88779-741">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="88779-741">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="88779-742">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-742">ACR</span></span>

* <span data-ttu-id="88779-743">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="88779-743">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="88779-744">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="88779-744">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="88779-745">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="88779-745">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="88779-746">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-746">AKS</span></span>

* <span data-ttu-id="88779-747">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="88779-747">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="88779-748">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="88779-748">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="88779-749">AppConfig</span><span class="sxs-lookup"><span data-stu-id="88779-749">AppConfig</span></span>

* <span data-ttu-id="88779-750">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="88779-750">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="88779-751">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="88779-751">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="88779-752">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="88779-752">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-753">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-753">AppService</span></span>

* <span data-ttu-id="88779-754">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="88779-754">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="88779-755">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="88779-755">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="88779-756">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="88779-756">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="88779-757">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="88779-757">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="88779-758">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="88779-758">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="88779-759">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-759">ARM</span></span>

* <span data-ttu-id="88779-760">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="88779-760">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="88779-761">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="88779-761">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="88779-762">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-762">Backup</span></span>

* <span data-ttu-id="88779-763">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="88779-763">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="88779-764">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-764">Compute</span></span>

* <span data-ttu-id="88779-765">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="88779-765">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="88779-766">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="88779-766">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="88779-767">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="88779-767">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="88779-768">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="88779-768">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="88779-769">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="88779-769">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="88779-770">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="88779-770">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="88779-771">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="88779-771">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="88779-772">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="88779-772">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-773">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-773">CosmosDB</span></span>

* <span data-ttu-id="88779-774">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="88779-774">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="88779-775">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="88779-775">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="88779-776">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-776">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="88779-777">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="88779-777">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="88779-778">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-778">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="88779-779">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="88779-779">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="88779-780">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-780">Fixed typo in help message</span></span>
* <span data-ttu-id="88779-781">base de données : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="88779-781">database: Added deprecation information</span></span>
* <span data-ttu-id="88779-782">collection : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="88779-782">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="88779-783">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-783">IoT</span></span>

* <span data-ttu-id="88779-784">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="88779-784">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="88779-785">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="88779-785">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-786">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-786">Key Vault</span></span>

* <span data-ttu-id="88779-787">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="88779-787">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="88779-788">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-788">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="88779-789">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="88779-789">NetAppFiles</span></span>

* <span data-ttu-id="88779-790">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="88779-790">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="88779-791">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="88779-791">This new API version includes:</span></span>

    - <span data-ttu-id="88779-792">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="88779-792">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="88779-793">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="88779-793">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="88779-794">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="88779-794">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="88779-795">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="88779-795">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="88779-796">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-796">Network</span></span>

* <span data-ttu-id="88779-797">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="88779-797">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="88779-798">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="88779-798">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="88779-799">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="88779-799">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="88779-800">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="88779-800">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="88779-801">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="88779-801">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="88779-802">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="88779-802">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-803">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-803">Profile</span></span>

* <span data-ttu-id="88779-804">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-804">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="88779-805">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="88779-805">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-806">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-806">RBAC</span></span>

* <span data-ttu-id="88779-807">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-807">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="88779-808">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="88779-808">ServiceFabric</span></span>

* <span data-ttu-id="88779-809">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="88779-809">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="88779-810">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-810">SQL</span></span>

* <span data-ttu-id="88779-811">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="88779-811">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="88779-812">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-812">Storage</span></span>

* <span data-ttu-id="88779-813">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="88779-813">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="88779-814">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="88779-814">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="88779-815">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-815">October 15, 2019</span></span>

<span data-ttu-id="88779-816">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="88779-816">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="88779-817">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-817">AKS</span></span>

* <span data-ttu-id="88779-818">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-818">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="88779-819">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-819">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="88779-820">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-820">AMS</span></span>

* <span data-ttu-id="88779-821">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="88779-821">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="88779-822">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="88779-822">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-823">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-823">AppService</span></span>

* <span data-ttu-id="88779-824">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="88779-824">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="88779-825">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-825">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="88779-826">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="88779-826">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="88779-827">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-827">ARM</span></span>

* <span data-ttu-id="88779-828">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="88779-828">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="88779-829">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-829">Compute</span></span>

* <span data-ttu-id="88779-830">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-830">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="88779-831">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="88779-831">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="88779-832">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="88779-832">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="88779-833">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="88779-833">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="88779-834">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-834">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="88779-835">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="88779-835">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="88779-836">Core</span><span class="sxs-lookup"><span data-stu-id="88779-836">Core</span></span>

* <span data-ttu-id="88779-837">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="88779-837">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="88779-838">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-838">IoT</span></span>

* <span data-ttu-id="88779-839">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="88779-839">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-840">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-840">Monitor</span></span>

* <span data-ttu-id="88779-841">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="88779-841">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="88779-842">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-842">Network</span></span>

* <span data-ttu-id="88779-843">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-843">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="88779-844">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="88779-844">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="88779-845">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-845">SQL</span></span>

* <span data-ttu-id="88779-846">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="88779-846">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="88779-847">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-847">Storage</span></span>

* <span data-ttu-id="88779-848">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="88779-848">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="88779-849">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-849">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="88779-850">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-850">September 24, 2019</span></span>

<span data-ttu-id="88779-851">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="88779-851">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="88779-852">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-852">ACR</span></span>

* <span data-ttu-id="88779-853">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="88779-853">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="88779-854">[CHANGEMENT CASSANT] Renommage du paramètre `--name -n` en `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="88779-854">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="88779-855">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-855">AKS</span></span>

* <span data-ttu-id="88779-856">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="88779-856">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="88779-857">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="88779-857">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="88779-858">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="88779-858">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="88779-859">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-859">ARM</span></span>

* <span data-ttu-id="88779-860">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="88779-860">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="88779-861">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-861">Compute</span></span>

* <span data-ttu-id="88779-862">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="88779-862">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="88779-863">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="88779-863">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="88779-864">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-864">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="88779-865">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="88779-865">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="88779-866">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="88779-866">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-867">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-867">Cosmos DB</span></span>

* <span data-ttu-id="88779-868">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="88779-868">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="88779-869">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="88779-869">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="88779-870">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="88779-870">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="88779-871">EventGrid</span><span class="sxs-lookup"><span data-stu-id="88779-871">EventGrid</span></span>

* <span data-ttu-id="88779-872">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="88779-872">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-873">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-873">Key Vault</span></span>

* <span data-ttu-id="88779-874">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="88779-874">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-875">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-875">Monitor</span></span>

* <span data-ttu-id="88779-876">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="88779-876">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="88779-877">Stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-877">Policy</span></span>

* <span data-ttu-id="88779-878">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="88779-878">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="88779-879">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="88779-879">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="88779-880">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-880">Storage</span></span>

* <span data-ttu-id="88779-881">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="88779-881">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="88779-882">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="88779-882">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="88779-883">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-883">ACR</span></span>

* <span data-ttu-id="88779-884">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="88779-884">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="88779-885">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-885">AKS</span></span>

* <span data-ttu-id="88779-886">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="88779-886">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="88779-887">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="88779-887">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="88779-888">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="88779-888">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="88779-889">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-889">ARM</span></span>

* <span data-ttu-id="88779-890">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="88779-890">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="88779-891">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-891">Batch</span></span>

* <span data-ttu-id="88779-892">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="88779-892">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="88779-893">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="88779-893">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="88779-894">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="88779-894">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="88779-895">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="88779-895">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="88779-896">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="88779-896">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="88779-897">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="88779-897">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="88779-898">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="88779-898">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-899">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-899">HDInsight</span></span>

* <span data-ttu-id="88779-900">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="88779-900">GA release</span></span>
* <span data-ttu-id="88779-901">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="88779-901">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-902">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-902">Key Vault</span></span>

* <span data-ttu-id="88779-903">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="88779-903">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="88779-904">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="88779-904">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="88779-905">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-905">Network</span></span>

* <span data-ttu-id="88779-906">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="88779-906">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="88779-907">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="88779-907">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="88779-908">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="88779-908">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="88779-909">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="88779-909">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="88779-910">Stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-910">Policy</span></span>

* <span data-ttu-id="88779-911">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="88779-911">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="88779-912">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="88779-912">August 27, 2019</span></span>

<span data-ttu-id="88779-913">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="88779-913">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="88779-914">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-914">ACR</span></span>

* <span data-ttu-id="88779-915">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="88779-915">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="88779-916">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="88779-916">API Management</span></span>

* <span data-ttu-id="88779-917">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="88779-917">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-918">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-918">AppService</span></span>

* <span data-ttu-id="88779-919">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="88779-919">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="88779-920">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-920">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-921">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-921">Keyvault</span></span>

* <span data-ttu-id="88779-922">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="88779-922">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="88779-923">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-923">Network</span></span>

* <span data-ttu-id="88779-924">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="88779-924">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="88779-925">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="88779-925">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="88779-926">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="88779-926">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="88779-927">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="88779-927">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-928">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-928">RBAC</span></span>

* <span data-ttu-id="88779-929">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="88779-929">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="88779-930">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="88779-930">ServiceFabric</span></span>

* <span data-ttu-id="88779-931">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="88779-931">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="88779-932">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-932">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="88779-933">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="88779-933">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="88779-934">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="88779-934">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="88779-935">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-935">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="88779-936">SignalR</span><span class="sxs-lookup"><span data-stu-id="88779-936">SignalR</span></span>

* <span data-ttu-id="88779-937">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="88779-937">Added new commands:</span></span>
  * <span data-ttu-id="88779-938">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="88779-938">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="88779-939">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="88779-939">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="88779-940">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="88779-940">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="88779-941">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="88779-941">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-942">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-942">Storage</span></span>

* <span data-ttu-id="88779-943">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="88779-943">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="88779-944">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="88779-944">August 13, 2019</span></span>

<span data-ttu-id="88779-945">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="88779-945">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-946">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-946">AppService</span></span>

* <span data-ttu-id="88779-947">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="88779-947">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-948">BotService</span><span class="sxs-lookup"><span data-stu-id="88779-948">BotService</span></span>

* <span data-ttu-id="88779-949">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="88779-949">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="88779-950">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="88779-950">CognitiveServices</span></span>

* <span data-ttu-id="88779-951">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-951">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-952">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-952">Cosmos DB</span></span>

* <span data-ttu-id="88779-953">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="88779-953">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="88779-954">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="88779-954">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-955">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-955">HDInsight</span></span>

<span data-ttu-id="88779-956">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="88779-956">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="88779-957">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="88779-957">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="88779-958">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="88779-958">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="88779-959">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="88779-959">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="88779-960">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="88779-960">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="88779-961">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="88779-961">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="88779-962">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="88779-962">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="88779-963">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="88779-963">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="88779-964">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="88779-964">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="88779-965">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="88779-965">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="88779-966">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="88779-966">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="88779-967">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="88779-967">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="88779-968">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="88779-968">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="88779-969">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="88779-969">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="88779-970">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="88779-970">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="88779-971">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="88779-971">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="88779-972">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="88779-972">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="88779-973">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="88779-973">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="88779-974">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="88779-974">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="88779-975">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="88779-975">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="88779-976">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="88779-976">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="88779-977">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-977">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="88779-978">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="88779-978">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="88779-979">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-979">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-980">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-980">Interactive</span></span>

* <span data-ttu-id="88779-981">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="88779-981">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="88779-982">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-982">Kubernetes</span></span>

* <span data-ttu-id="88779-983">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="88779-983">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="88779-984">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-984">Network</span></span>

* <span data-ttu-id="88779-985">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="88779-985">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-986">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-986">Profile</span></span>

* <span data-ttu-id="88779-987">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="88779-987">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="88779-988">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="88779-988">ServiceFabric</span></span>

* <span data-ttu-id="88779-989">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="88779-989">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="88779-990">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="88779-990">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="88779-991">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-991">Storage</span></span>

* <span data-ttu-id="88779-992">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="88779-992">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="88779-993">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="88779-993">July 30, 2019</span></span>

<span data-ttu-id="88779-994">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="88779-994">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="88779-995">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-995">ACR</span></span>

* <span data-ttu-id="88779-996">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="88779-996">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="88779-997">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="88779-997">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-998">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-998">Appservice</span></span>

* <span data-ttu-id="88779-999">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="88779-999">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="88779-1000">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="88779-1000">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="88779-1001">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="88779-1001">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="88779-1002">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1002">Network</span></span>

* <span data-ttu-id="88779-1003">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="88779-1003">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="88779-1004">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="88779-1004">Fixes #9604.</span></span> <span data-ttu-id="88779-1005">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="88779-1005">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="88779-1006">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="88779-1006">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-1007">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-1007">RBAC</span></span>

* <span data-ttu-id="88779-1008">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="88779-1008">Added `user update` command</span></span>
* <span data-ttu-id="88779-1009">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="88779-1009">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="88779-1010">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="88779-1010">Use replacement argument `--id`</span></span>
* <span data-ttu-id="88779-1011">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="88779-1011">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1012">SQL</span></span>

* <span data-ttu-id="88779-1013">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="88779-1013">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1014">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1014">Storage</span></span>

* <span data-ttu-id="88779-1015">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="88779-1015">Added `storage remove` command</span></span>
* <span data-ttu-id="88779-1016">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="88779-1016">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1017">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1017">VM</span></span>

* <span data-ttu-id="88779-1018">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="88779-1018">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="88779-1019">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="88779-1019">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="88779-1020">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="88779-1020">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="88779-1021">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="88779-1021">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="88779-1022">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1022">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="88779-1023">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1023">July 16, 2019</span></span>

<span data-ttu-id="88779-1024">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="88779-1024">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1025">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1025">Appservice</span></span>

* <span data-ttu-id="88779-1026">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="88779-1026">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="88779-1027">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="88779-1027">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="88779-1028">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="88779-1028">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="88779-1029">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1029">Core</span></span>

* <span data-ttu-id="88779-1030">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="88779-1030">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1031">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1031">Batch</span></span>

* <span data-ttu-id="88779-1032">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="88779-1032">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="88779-1033">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="88779-1033">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="88779-1034">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="88779-1034">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="88779-1035">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1035">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="88779-1036">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="88779-1036">Eventhubs</span></span>

* <span data-ttu-id="88779-1037">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="88779-1037">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1038">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-1038">RDBMS</span></span>

* <span data-ttu-id="88779-1039">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="88779-1039">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="88779-1040">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="88779-1040">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="88779-1041">Relais</span><span class="sxs-lookup"><span data-stu-id="88779-1041">Relay</span></span>

* <span data-ttu-id="88779-1042">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="88779-1042">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="88779-1043">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="88779-1043">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="88779-1044">Servicebus</span><span class="sxs-lookup"><span data-stu-id="88779-1044">Servicebus</span></span>

* <span data-ttu-id="88779-1045">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="88779-1045">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1046">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1046">Storage</span></span>

* <span data-ttu-id="88779-1047">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1047">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="88779-1048">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="88779-1048">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="88779-1049">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1049">July 2, 2019</span></span>

<span data-ttu-id="88779-1050">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="88779-1050">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="88779-1051">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1051">Core</span></span>

* <span data-ttu-id="88779-1052">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="88779-1052">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="88779-1053">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="88779-1053">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="88779-1054">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="88779-1054">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1055">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1055">ACR</span></span>

* <span data-ttu-id="88779-1056">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="88779-1056">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1057">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1057">Appservice</span></span>

* <span data-ttu-id="88779-1058">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1058">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="88779-1059">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="88779-1059">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="88779-1060">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="88779-1060">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="88779-1061">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="88779-1061">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-1062">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-1062">Cosmos DB</span></span>

* <span data-ttu-id="88779-1063">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="88779-1063">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="88779-1064">DLS</span><span class="sxs-lookup"><span data-stu-id="88779-1064">DLS</span></span>

* <span data-ttu-id="88779-1065">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="88779-1065">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="88779-1066">Commentaires</span><span class="sxs-lookup"><span data-stu-id="88779-1066">Feedback</span></span>

* <span data-ttu-id="88779-1067">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="88779-1067">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1068">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1068">HDInsight</span></span>

* <span data-ttu-id="88779-1069">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="88779-1069">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="88779-1070">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="88779-1070">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="88779-1071">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="88779-1071">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="88779-1072">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="88779-1072">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="88779-1073">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="88779-1073">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="88779-1074">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1074">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="88779-1075">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="88779-1075">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="88779-1076">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="88779-1076">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="88779-1077">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="88779-1077">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="88779-1078">Services gérés</span><span class="sxs-lookup"><span data-stu-id="88779-1078">Managed Services</span></span>

* <span data-ttu-id="88779-1079">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="88779-1079">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="88779-1080">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-1080">Profile</span></span>
* <span data-ttu-id="88779-1081">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="88779-1081">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-1082">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-1082">RBAC</span></span>

* <span data-ttu-id="88779-1083">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="88779-1083">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="88779-1084">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="88779-1084">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="88779-1085">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="88779-1085">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="88779-1086">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="88779-1086">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1087">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-1087">RDBMS</span></span>

* <span data-ttu-id="88779-1088">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="88779-1088">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1089">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1089">SQL</span></span>

* <span data-ttu-id="88779-1090">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="88779-1090">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1091">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1091">Storage</span></span>

* <span data-ttu-id="88779-1092">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="88779-1092">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="88779-1093">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="88779-1093">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="88779-1094">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1094">VM</span></span>

* <span data-ttu-id="88779-1095">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1095">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="88779-1096">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="88779-1096">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="88779-1097">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="88779-1097">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="88779-1098">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="88779-1098">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="88779-1099">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1099">June 18, 2019</span></span>

<span data-ttu-id="88779-1100">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="88779-1100">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="88779-1101">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1101">Core</span></span>

<span data-ttu-id="88779-1102">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="88779-1102">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="88779-1103">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="88779-1103">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="88779-1104">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="88779-1104">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="88779-1105">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="88779-1105">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="88779-1106">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="88779-1106">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="88779-1107">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="88779-1107">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="88779-1108">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="88779-1108">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1109">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1109">ACR</span></span>
* <span data-ttu-id="88779-1110">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="88779-1110">Added 'acr check-health' command</span></span>
* <span data-ttu-id="88779-1111">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="88779-1111">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1112">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1112">ACS</span></span>
* <span data-ttu-id="88779-1113">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="88779-1113">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1114">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1114">AMS</span></span>
* <span data-ttu-id="88779-1115">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="88779-1115">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1116">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1116">AppService</span></span>
* <span data-ttu-id="88779-1117">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="88779-1117">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="88779-1118">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-1118">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="88779-1119">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="88779-1119">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="88779-1120">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="88779-1120">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="88779-1121">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="88779-1121">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="88779-1122">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="88779-1122">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1123">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1123">Batch</span></span>
* <span data-ttu-id="88779-1124">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="88779-1124">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-1125">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-1125">BatchAI</span></span>
* <span data-ttu-id="88779-1126">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="88779-1126">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1127">BotService</span><span class="sxs-lookup"><span data-stu-id="88779-1127">BotService</span></span>
* <span data-ttu-id="88779-1128">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="88779-1128">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1129">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-1129">CosmosDB</span></span>
* <span data-ttu-id="88779-1130">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="88779-1130">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="88779-1131">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="88779-1131">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="88779-1132">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="88779-1132">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="88779-1133">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="88779-1133">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="88779-1134">EventGrid</span><span class="sxs-lookup"><span data-stu-id="88779-1134">EventGrid</span></span>
* <span data-ttu-id="88779-1135">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="88779-1135">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="88779-1136">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="88779-1136">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="88779-1137">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="88779-1137">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="88779-1138">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="88779-1138">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="88779-1139">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1139">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1140">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1140">HDInsight</span></span>
* <span data-ttu-id="88779-1141">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="88779-1141">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1142">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1142">IoT</span></span>
* <span data-ttu-id="88779-1143">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="88779-1143">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="88779-1144">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="88779-1144">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="88779-1145">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1145">Network</span></span>
* <span data-ttu-id="88779-1146">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="88779-1146">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="88779-1147">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="88779-1147">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="88779-1148">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="88779-1148">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="88779-1149">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="88779-1149">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1150">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1150">Resource</span></span>
* <span data-ttu-id="88779-1151">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="88779-1151">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="88779-1152">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="88779-1152">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="88779-1153">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="88779-1153">ServiceBus</span></span>
* <span data-ttu-id="88779-1154">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="88779-1154">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1155">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1155">SQL</span></span>
* <span data-ttu-id="88779-1156">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="88779-1156">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="88779-1157">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="88779-1157">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="88779-1158">SQLVm</span><span class="sxs-lookup"><span data-stu-id="88779-1158">SQLVm</span></span>
* <span data-ttu-id="88779-1159">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="88779-1159">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="88779-1160">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1160">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1161">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1161">Storage</span></span>
* <span data-ttu-id="88779-1162">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="88779-1162">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="88779-1163">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="88779-1163">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1164">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1164">VM</span></span>
* <span data-ttu-id="88779-1165">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1165">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="88779-1166">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1166">June 4, 2019</span></span>

<span data-ttu-id="88779-1167">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="88779-1167">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="88779-1168">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1168">Core</span></span>
* <span data-ttu-id="88779-1169">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="88779-1169">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1170">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1170">ACR</span></span>
* <span data-ttu-id="88779-1171">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="88779-1171">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1172">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1172">ACS</span></span>
* <span data-ttu-id="88779-1173">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="88779-1173">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="88779-1174">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="88779-1174">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1175">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1175">Batch</span></span>
* <span data-ttu-id="88779-1176">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="88779-1176">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1177">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1177">IoT</span></span>
* <span data-ttu-id="88779-1178">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="88779-1178">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="88779-1179">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1179">Network</span></span>
* <span data-ttu-id="88779-1180">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="88779-1180">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="88779-1181">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1181">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="88779-1182">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1182">Resource</span></span>
* <span data-ttu-id="88779-1183">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="88779-1183">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="88779-1184">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1184">Role</span></span>
* <span data-ttu-id="88779-1185">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-1185">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="88779-1186">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-1186">Compute</span></span>
* <span data-ttu-id="88779-1187">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="88779-1187">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="88779-1188">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1188">May 21, 2019</span></span>

<span data-ttu-id="88779-1189">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="88779-1189">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="88779-1190">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1190">Core</span></span>
* <span data-ttu-id="88779-1191">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="88779-1191">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="88779-1192">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="88779-1192">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="88779-1193">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="88779-1193">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1194">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1194">ACR</span></span>
* <span data-ttu-id="88779-1195">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="88779-1195">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1196">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1196">ACS</span></span>
* <span data-ttu-id="88779-1197">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="88779-1197">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1198">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1198">AppService</span></span>
* <span data-ttu-id="88779-1199">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="88779-1199">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="88779-1200">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="88779-1200">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="88779-1201">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="88779-1201">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="88779-1202">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="88779-1202">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="88779-1203">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-1203">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="88779-1204">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="88779-1204">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="88779-1205">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-1205">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1206">BotService</span><span class="sxs-lookup"><span data-stu-id="88779-1206">BotService</span></span>
* <span data-ttu-id="88779-1207">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="88779-1207">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="88779-1208">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="88779-1208">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-1209">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-1209">Consumption</span></span>
* <span data-ttu-id="88779-1210">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="88779-1210">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1211">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1211">IoT</span></span>
* <span data-ttu-id="88779-1212">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="88779-1212">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="88779-1213">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1213">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="88779-1215">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="88779-1215">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="88779-1216">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="88779-1216">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1217">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-1217">RDBMS</span></span>
* <span data-ttu-id="88779-1218">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="88779-1218">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-1219">RBAC</span><span class="sxs-lookup"><span data-stu-id="88779-1219">RBAC</span></span>
* <span data-ttu-id="88779-1220">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="88779-1220">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1221">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1221">Storage</span></span>
* <span data-ttu-id="88779-1222">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1222">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="88779-1223">Calcul</span><span class="sxs-lookup"><span data-stu-id="88779-1223">Compute</span></span>
* <span data-ttu-id="88779-1224">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1224">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="88779-1225">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="88779-1225">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="88779-1226">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="88779-1226">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="88779-1227">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="88779-1227">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="88779-1228">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1228">May 6, 2019</span></span>

<span data-ttu-id="88779-1229">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="88779-1229">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1230">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1230">ACS</span></span>
* <span data-ttu-id="88779-1231">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="88779-1231">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="88779-1232">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="88779-1232">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="88779-1233">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="88779-1233">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="88779-1234">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-1234">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1235">Appservice</span></span>
* <span data-ttu-id="88779-1236">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="88779-1236">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="88779-1237">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="88779-1237">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="88779-1238">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-1238">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="88779-1239">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="88779-1239">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="88779-1240">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-1240">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="88779-1241">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="88779-1241">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="88779-1242">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="88779-1242">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="88779-1243">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="88779-1243">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="88779-1244">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-1244">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="88779-1245">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="88779-1245">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1246">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1246">Batch</span></span>
* <span data-ttu-id="88779-1247">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="88779-1247">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1248">Botservice</span><span class="sxs-lookup"><span data-stu-id="88779-1248">Botservice</span></span>
* <span data-ttu-id="88779-1249">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="88779-1249">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="88779-1250">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="88779-1250">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="88779-1251">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="88779-1251">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="88779-1252">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1252">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="88779-1253">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="88779-1253">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="88779-1254">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="88779-1254">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="88779-1255">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="88779-1255">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="88779-1256">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="88779-1256">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="88779-1257">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="88779-1257">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="88779-1258">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="88779-1258">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="88779-1259">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="88779-1259">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="88779-1260">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="88779-1260">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="88779-1261">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="88779-1261">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="88779-1262">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="88779-1262">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="88779-1263">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1263">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="88779-1264">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="88779-1264">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="88779-1265">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="88779-1265">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="88779-1266">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="88779-1266">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="88779-1267">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="88779-1267">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="88779-1268">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="88779-1268">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="88779-1269">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="88779-1269">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="88779-1270">Configurer</span><span class="sxs-lookup"><span data-stu-id="88779-1270">Configure</span></span>
* <span data-ttu-id="88779-1271">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="88779-1271">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="88779-1272">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="88779-1272">Eventhubs</span></span>
* <span data-ttu-id="88779-1273">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-1273">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="88779-1274">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1274">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1275">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1275">Network</span></span>
* <span data-ttu-id="88779-1276">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1276">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="88779-1277">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="88779-1277">Policy Insights</span></span>
* <span data-ttu-id="88779-1278">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1278">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="88779-1279">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1279">Role</span></span>
* <span data-ttu-id="88779-1280">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1280">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="88779-1281">Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-1281">Service Bus</span></span>
* <span data-ttu-id="88779-1282">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-1282">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="88779-1283">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1283">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="88779-1284">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="88779-1284">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1285">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1285">SQL</span></span>
* <span data-ttu-id="88779-1286">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="88779-1286">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1287">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1287">VM</span></span>
* <span data-ttu-id="88779-1288">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="88779-1288">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="88779-1289">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="88779-1289">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="88779-1290">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1290">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="88779-1291">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="88779-1291">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="88779-1292">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="88779-1292">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="88779-1293">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="88779-1293">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="88779-1294">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1294">April 23, 2019</span></span>

<span data-ttu-id="88779-1295">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="88779-1295">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1296">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1296">ACS</span></span>
* <span data-ttu-id="88779-1297">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="88779-1297">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="88779-1298">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="88779-1298">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1299">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1299">AMS</span></span>
* <span data-ttu-id="88779-1300">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="88779-1300">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1301">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1301">AppService</span></span>
* <span data-ttu-id="88779-1302">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="88779-1302">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="88779-1303">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="88779-1303">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="88779-1304">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="88779-1304">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="88779-1305">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="88779-1305">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="88779-1306">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="88779-1306">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="88779-1307">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="88779-1307">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="88779-1308">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="88779-1308">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="88779-1309">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="88779-1309">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="88779-1310">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="88779-1310">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="88779-1311">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-1311">Deployment Manager</span></span>
* <span data-ttu-id="88779-1312">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="88779-1312">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="88779-1313">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-1313">Lab</span></span>
* <span data-ttu-id="88779-1314">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="88779-1314">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="88779-1315">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1315">Network</span></span>
* <span data-ttu-id="88779-1316">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="88779-1316">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1317">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1317">Resource</span></span>
* <span data-ttu-id="88779-1318">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="88779-1318">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="88779-1319">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="88779-1319">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="88779-1320">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1320">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="88779-1321">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="88779-1321">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1322">SQL</span></span>
* <span data-ttu-id="88779-1323">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="88779-1323">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="88779-1324">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="88779-1324">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="88779-1325">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1325">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="88779-1326">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1326">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1327">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1327">Storage</span></span>
* <span data-ttu-id="88779-1328">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="88779-1328">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1329">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1329">VM</span></span>
* <span data-ttu-id="88779-1330">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="88779-1330">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="88779-1331">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="88779-1331">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="88779-1332">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="88779-1332">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="88779-1333">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1333">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="88779-1334">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1334">Core</span></span>
* <span data-ttu-id="88779-1335">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="88779-1335">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1336">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1336">ACR</span></span>
* <span data-ttu-id="88779-1337">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="88779-1337">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1338">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1338">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="88779-1341">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="88779-1341">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="88779-1342">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="88779-1342">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1343">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1343">AppService</span></span>
* <span data-ttu-id="88779-1344">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-1344">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="88779-1345">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="88779-1345">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="88779-1346">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="88779-1346">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="88779-1347">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="88779-1347">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="88779-1348">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="88779-1348">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="88779-1349">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="88779-1349">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="88779-1350">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="88779-1350">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-1351">CDN</span></span>
* <span data-ttu-id="88779-1352">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="88779-1352">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="88779-1353">Commentaires</span><span class="sxs-lookup"><span data-stu-id="88779-1353">Feedback</span></span>
* <span data-ttu-id="88779-1354">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="88779-1354">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="88779-1355">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="88779-1355">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="88779-1356">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="88779-1356">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1357">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1357">Monitor</span></span>
* <span data-ttu-id="88779-1358">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1358">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="88779-1359">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1359">Network</span></span>
* <span data-ttu-id="88779-1360">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="88779-1360">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="88779-1361">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-1361">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="88779-1362">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="88779-1362">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="88779-1363">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="88779-1363">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="88779-1364">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="88779-1364">PrivateDNS</span></span>
* <span data-ttu-id="88779-1365">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="88779-1365">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1366">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1366">Resource</span></span>
* <span data-ttu-id="88779-1367">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-1367">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="88779-1368">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1368">Role</span></span>
* <span data-ttu-id="88779-1369">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="88779-1369">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="88779-1370">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-1370">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1371">SQL</span></span>
* <span data-ttu-id="88779-1372">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="88779-1372">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1373">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1373">Storage</span></span>
* <span data-ttu-id="88779-1374">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="88779-1374">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="88779-1375">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="88779-1375">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="88779-1376">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="88779-1376">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="88779-1377">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="88779-1377">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="88779-1378">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1378">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="88779-1379">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1379">Core</span></span>
* <span data-ttu-id="88779-1380">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="88779-1380">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="88779-1381">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="88779-1381">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="88779-1382">Cloud</span><span class="sxs-lookup"><span data-stu-id="88779-1382">Cloud</span></span>
* <span data-ttu-id="88779-1383">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="88779-1383">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1384">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1384">ACR</span></span>
* <span data-ttu-id="88779-1385">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="88779-1385">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="88779-1386">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="88779-1386">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="88779-1387">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="88779-1387">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="88779-1388">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="88779-1388">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1389">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1389">AppService</span></span>
* <span data-ttu-id="88779-1390">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="88779-1390">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="88779-1391">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="88779-1391">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="88779-1392">Service BOT</span><span class="sxs-lookup"><span data-stu-id="88779-1392">BOT Service</span></span>
* <span data-ttu-id="88779-1393">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="88779-1393">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="88779-1394">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="88779-1394">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="88779-1395">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="88779-1395">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="88779-1396">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="88779-1396">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-1397">CDN</span></span>
* <span data-ttu-id="88779-1398">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="88779-1398">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="88779-1399">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="88779-1399">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="88779-1400">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="88779-1400">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="88779-1401">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="88779-1401">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1402">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="88779-1402">Cosmosdb</span></span>
* <span data-ttu-id="88779-1403">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="88779-1403">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="88779-1404">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-1404">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-1405">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-1405">Interactive</span></span>
* <span data-ttu-id="88779-1406">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="88779-1406">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1407">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1407">Monitor</span></span>
* <span data-ttu-id="88779-1408">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1408">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1409">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1409">Network</span></span>
* <span data-ttu-id="88779-1410">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="88779-1410">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-1411">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-1411">Profile</span></span>
* <span data-ttu-id="88779-1412">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="88779-1412">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="88779-1413">Postgres</span><span class="sxs-lookup"><span data-stu-id="88779-1413">Postgres</span></span> 
* <span data-ttu-id="88779-1414">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="88779-1414">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="88779-1415">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="88779-1415">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1416">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1416">Resource</span></span>
* <span data-ttu-id="88779-1417">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-1417">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="88779-1418">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="88779-1418">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="88779-1419">Graph</span><span class="sxs-lookup"><span data-stu-id="88779-1419">Graph</span></span>
* <span data-ttu-id="88779-1420">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="88779-1420">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="88779-1421">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="88779-1421">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="88779-1422">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="88779-1422">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="88779-1423">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-1423">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="88779-1424">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="88779-1424">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1425">storage</span><span class="sxs-lookup"><span data-stu-id="88779-1425">storage</span></span>
* <span data-ttu-id="88779-1426">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="88779-1426">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="88779-1427">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="88779-1427">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="88779-1428">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="88779-1428">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="88779-1429">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="88779-1429">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1430">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1430">VM</span></span>
* <span data-ttu-id="88779-1431">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="88779-1431">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="88779-1432">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1432">March 12, 2019</span></span>

<span data-ttu-id="88779-1433">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="88779-1433">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="88779-1434">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1434">Core</span></span>

* <span data-ttu-id="88779-1435">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="88779-1435">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1436">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1436">ACR</span></span>

* <span data-ttu-id="88779-1437">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="88779-1437">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1438">ACS</span></span>

* <span data-ttu-id="88779-1439">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="88779-1439">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="88779-1440">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1440">AppService</span></span>

* <span data-ttu-id="88779-1441">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="88779-1441">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="88779-1442">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="88779-1442">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="88779-1443">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="88779-1443">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="88779-1444">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="88779-1444">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1445">Botservice</span><span class="sxs-lookup"><span data-stu-id="88779-1445">Botservice</span></span>

* <span data-ttu-id="88779-1446">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="88779-1446">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="88779-1447">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="88779-1447">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="88779-1448">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="88779-1448">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="88779-1449">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="88779-1449">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="88779-1450">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1450">Container</span></span>

* <span data-ttu-id="88779-1451">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="88779-1451">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="88779-1452">Event Hub</span><span class="sxs-lookup"><span data-stu-id="88779-1452">EventHub</span></span>

* <span data-ttu-id="88779-1453">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="88779-1453">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="88779-1454">Rechercher</span><span class="sxs-lookup"><span data-stu-id="88779-1454">Find</span></span>

* <span data-ttu-id="88779-1455">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="88779-1455">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1456">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1456">HDInsight</span></span>

* <span data-ttu-id="88779-1457">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="88779-1457">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="88779-1458">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1458">Network</span></span>

* <span data-ttu-id="88779-1459">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="88779-1459">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1460">Rdbms</span><span class="sxs-lookup"><span data-stu-id="88779-1460">Rdbms</span></span>

* <span data-ttu-id="88779-1461">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="88779-1461">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="88779-1462">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1462">Role</span></span>

* <span data-ttu-id="88779-1463">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="88779-1463">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="88779-1464">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="88779-1464">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="88779-1465">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-1465">Service Fabric</span></span>

* <span data-ttu-id="88779-1466">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="88779-1466">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="88779-1467">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1467">February 26, 2019</span></span>

<span data-ttu-id="88779-1468">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="88779-1468">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="88779-1469">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1469">Core</span></span>

* <span data-ttu-id="88779-1470">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="88779-1470">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1471">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1471">ACR</span></span>

* <span data-ttu-id="88779-1472">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="88779-1472">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="88779-1473">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="88779-1473">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1474">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1474">ACS</span></span>

* <span data-ttu-id="88779-1475">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="88779-1475">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1476">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1476">AppService</span></span>

* <span data-ttu-id="88779-1477">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="88779-1477">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1478">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1478">Batch</span></span>
* <span data-ttu-id="88779-1479">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="88779-1479">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="88779-1480">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="88779-1480">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="88779-1481">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="88779-1481">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="88779-1482">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="88779-1482">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="88779-1483">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="88779-1483">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="88779-1484">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="88779-1484">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1485">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-1485">CosmosDB</span></span>

* <span data-ttu-id="88779-1486">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-1486">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="88779-1487">Kusto</span><span class="sxs-lookup"><span data-stu-id="88779-1487">Kusto</span></span>

* <span data-ttu-id="88779-1488">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="88779-1488">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="88779-1489">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1489">Network</span></span>

* <span data-ttu-id="88779-1490">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1490">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="88779-1491">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="88779-1491">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="88779-1492">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="88779-1492">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="88779-1493">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1493">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="88779-1494">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1494">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="88779-1495">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1495">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="88779-1496">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="88779-1496">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1497">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1497">Resource</span></span>

* <span data-ttu-id="88779-1498">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="88779-1498">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="88779-1499">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="88779-1499">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="88779-1500">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="88779-1500">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="88779-1501">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="88779-1501">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="88779-1502">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-1502">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="88779-1503">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1503">Role</span></span>

* <span data-ttu-id="88779-1504">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1504">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1505">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1505">VM</span></span>

* <span data-ttu-id="88779-1506">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="88779-1506">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="88779-1507">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1507">February 12, 2019</span></span>

<span data-ttu-id="88779-1508">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="88779-1508">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="88779-1509">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1509">Core</span></span>

* <span data-ttu-id="88779-1510">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="88779-1510">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="88779-1511">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="88779-1511">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1512">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1512">ACR</span></span>
* <span data-ttu-id="88779-1513">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="88779-1513">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="88779-1514">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="88779-1514">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1515">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1515">ACS</span></span>
* <span data-ttu-id="88779-1516">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="88779-1516">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="88779-1517">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="88779-1517">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="88779-1518">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="88779-1518">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1519">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1519">AMS</span></span>
* <span data-ttu-id="88779-1520">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1520">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="88779-1521">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1521">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1522">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1522">Appservice</span></span>
* <span data-ttu-id="88779-1523">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1523">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="88779-1524">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="88779-1524">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="88779-1525">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="88779-1525">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="88779-1526">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="88779-1526">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="88779-1527">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="88779-1527">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1528">Botservice</span><span class="sxs-lookup"><span data-stu-id="88779-1528">Botservice</span></span>
* <span data-ttu-id="88779-1529">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="88779-1529">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="88779-1530">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="88779-1530">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="88779-1531">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="88779-1531">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="88779-1532">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="88779-1532">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="88779-1533">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="88779-1533">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="88779-1534">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="88779-1534">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="88779-1535">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="88779-1535">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="88779-1536">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="88779-1536">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="88779-1537">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="88779-1537">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="88779-1538">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="88779-1538">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-1539">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-1539">Key Vault</span></span>
* <span data-ttu-id="88779-1540">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="88779-1540">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1541">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1541">Monitor</span></span>
* <span data-ttu-id="88779-1542">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="88779-1542">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1543">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1543">Network</span></span>
* <span data-ttu-id="88779-1544">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="88779-1544">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="88779-1545">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="88779-1545">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="88779-1546">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-1546">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="88779-1547">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1547">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="88779-1548">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="88779-1548">Policy Insights</span></span>
* <span data-ttu-id="88779-1549">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="88779-1549">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1550">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-1550">RDBMS</span></span>
* <span data-ttu-id="88779-1551">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="88779-1551">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="88779-1552">Redis</span><span class="sxs-lookup"><span data-stu-id="88779-1552">Redis</span></span>
* <span data-ttu-id="88779-1553">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="88779-1553">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="88779-1554">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="88779-1554">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="88779-1555">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="88779-1555">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="88779-1556">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="88779-1556">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="88779-1557">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="88779-1557">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="88779-1558">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="88779-1558">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="88779-1559">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="88779-1559">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="88779-1560">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1560">Role</span></span>
* <span data-ttu-id="88779-1561">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="88779-1561">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="88779-1562">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1562">SQL VM</span></span>
* <span data-ttu-id="88779-1563">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="88779-1563">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1564">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1564">VM</span></span>
* <span data-ttu-id="88779-1565">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="88779-1565">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="88779-1566">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="88779-1566">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="88779-1567">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="88779-1567">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="88779-1568">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="88779-1568">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="88779-1569">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1569">January 31, 2019</span></span>

<span data-ttu-id="88779-1570">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="88779-1570">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="88779-1571">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1571">Core</span></span>

* <span data-ttu-id="88779-1572">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="88779-1572">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="88779-1573">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1573">January 28, 2019</span></span>

<span data-ttu-id="88779-1574">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="88779-1574">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1575">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1575">ACR</span></span>
* <span data-ttu-id="88779-1576">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="88779-1576">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1577">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1577">ACS</span></span>
* <span data-ttu-id="88779-1578">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="88779-1578">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="88779-1579">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="88779-1579">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="88779-1580">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="88779-1580">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1581">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1581">AMS</span></span>
* <span data-ttu-id="88779-1582">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="88779-1582">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="88779-1583">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="88779-1583">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1584">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1584">Appservice</span></span>
* <span data-ttu-id="88779-1585">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="88779-1585">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="88779-1586">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="88779-1586">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="88779-1587">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="88779-1587">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="88779-1588">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1588">Container</span></span>
* <span data-ttu-id="88779-1589">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="88779-1589">Added `container start` command</span></span>
* <span data-ttu-id="88779-1590">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1590">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="88779-1591">EventGrid</span><span class="sxs-lookup"><span data-stu-id="88779-1591">EventGrid</span></span>
* <span data-ttu-id="88779-1592">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1592">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="88779-1593">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="88779-1593">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="88779-1594">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="88779-1594">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="88779-1595">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="88779-1595">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="88779-1596">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="88779-1596">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1597">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1597">HDInsight</span></span>
* <span data-ttu-id="88779-1598">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="88779-1598">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="88779-1599">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="88779-1599">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="88779-1600">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="88779-1600">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="88779-1601">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="88779-1601">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="88779-1602">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="88779-1602">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="88779-1603">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="88779-1603">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1604">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1604">IoT</span></span>
* <span data-ttu-id="88779-1605">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="88779-1605">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="88779-1606">Kusto</span><span class="sxs-lookup"><span data-stu-id="88779-1606">Kusto</span></span>
* <span data-ttu-id="88779-1607">Préversion</span><span class="sxs-lookup"><span data-stu-id="88779-1607">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1608">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1608">Monitor</span></span>
* <span data-ttu-id="88779-1609">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="88779-1609">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="88779-1610">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-1610">Profile</span></span>
* <span data-ttu-id="88779-1611">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="88779-1611">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1612">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1612">Network</span></span>
* <span data-ttu-id="88779-1613">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="88779-1613">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="88779-1614">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="88779-1614">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1615">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1615">Resource</span></span>
* <span data-ttu-id="88779-1616">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="88779-1616">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="88779-1617">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-1617">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="88779-1618">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1618">SQL Virtual Machine</span></span>
* <span data-ttu-id="88779-1619">Préversion</span><span class="sxs-lookup"><span data-stu-id="88779-1619">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1620">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1620">Storage</span></span>
* <span data-ttu-id="88779-1621">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="88779-1621">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="88779-1622">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="88779-1622">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1623">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1623">VM</span></span>
* <span data-ttu-id="88779-1624">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="88779-1624">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="88779-1625">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="88779-1625">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="88779-1626">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="88779-1626">January 15, 2019</span></span>

<span data-ttu-id="88779-1627">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="88779-1627">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1628">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1628">ACR</span></span>
* <span data-ttu-id="88779-1629">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="88779-1629">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="88779-1630">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="88779-1630">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="88779-1631">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="88779-1631">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="88779-1632">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1632">ACS</span></span>
* <span data-ttu-id="88779-1633">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="88779-1633">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1634">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1634">Appservice</span></span>
* <span data-ttu-id="88779-1635">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="88779-1635">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="88779-1636">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="88779-1636">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="88779-1637">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-1637">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="88779-1638">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="88779-1638">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1639">Botservice</span><span class="sxs-lookup"><span data-stu-id="88779-1639">Botservice</span></span>
* <span data-ttu-id="88779-1640">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="88779-1640">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="88779-1641">Configurer</span><span class="sxs-lookup"><span data-stu-id="88779-1641">Configure</span></span>
* <span data-ttu-id="88779-1642">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="88779-1642">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1643">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-1643">CosmosDB</span></span>
* <span data-ttu-id="88779-1644">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="88779-1644">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1645">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1645">HDInsight</span></span>
* <span data-ttu-id="88779-1646">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="88779-1646">Added commands for managing applications</span></span>
* <span data-ttu-id="88779-1647">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="88779-1647">Added commands for managing script actions</span></span>
* <span data-ttu-id="88779-1648">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="88779-1648">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="88779-1649">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="88779-1649">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="88779-1650">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="88779-1650">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1651">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1651">Network</span></span>
* <span data-ttu-id="88779-1652">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1652">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="88779-1653">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="88779-1653">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="88779-1654">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1654">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="88779-1655">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="88779-1655">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="88779-1656">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1656">Role</span></span>
* <span data-ttu-id="88779-1657">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="88779-1657">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="88779-1658">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="88779-1658">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="88779-1659">Sécurité</span><span class="sxs-lookup"><span data-stu-id="88779-1659">Security</span></span>
* <span data-ttu-id="88779-1660">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-1660">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1661">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1661">Storage</span></span>
* <span data-ttu-id="88779-1662">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="88779-1662">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="88779-1663">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="88779-1663">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="88779-1664">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="88779-1664">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="88779-1665">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="88779-1665">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="88779-1666">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="88779-1666">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1667">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1667">VM</span></span>
* <span data-ttu-id="88779-1668">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="88779-1668">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="88779-1669">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-1669">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="88779-1670">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="88779-1670">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="88779-1671">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="88779-1671">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="88779-1672">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1672">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="88779-1673">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="88779-1673">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="88779-1674">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1674">December 20, 2018</span></span>

<span data-ttu-id="88779-1675">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="88779-1675">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="88779-1676">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1676">Appservice</span></span>
* <span data-ttu-id="88779-1677">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="88779-1677">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="88779-1678">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="88779-1678">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="88779-1679">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="88779-1679">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="88779-1680">IotCentral</span><span class="sxs-lookup"><span data-stu-id="88779-1680">IoTCentral</span></span>
* <span data-ttu-id="88779-1681">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="88779-1681">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="88779-1682">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1682">Role</span></span>
* <span data-ttu-id="88779-1683">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="88779-1683">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1684">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1684">SQL</span></span>
* <span data-ttu-id="88779-1685">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="88779-1685">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1686">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1686">VM</span></span>
* <span data-ttu-id="88779-1687">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="88779-1687">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="88779-1688">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1688">December 18, 2018</span></span>

<span data-ttu-id="88779-1689">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="88779-1689">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="88779-1690">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1690">ACR</span></span>
* <span data-ttu-id="88779-1691">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="88779-1691">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="88779-1692">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="88779-1692">Condensed the table layout for task list</span></span>
* <span data-ttu-id="88779-1693">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="88779-1693">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1694">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1694">ACS</span></span>
* <span data-ttu-id="88779-1695">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="88779-1695">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="88779-1696">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-1696">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="88779-1697">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="88779-1697">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="88779-1698">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="88779-1698">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="88779-1699">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="88779-1699">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="88779-1700">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="88779-1700">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1701">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1701">Appservice</span></span>
* <span data-ttu-id="88779-1702">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="88779-1702">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="88779-1703">Botservice</span><span class="sxs-lookup"><span data-stu-id="88779-1703">Botservice</span></span>
* <span data-ttu-id="88779-1704">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="88779-1704">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="88779-1705">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="88779-1705">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="88779-1706">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="88779-1706">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="88779-1707">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="88779-1707">Reduced Kudu network calls</span></span>
* <span data-ttu-id="88779-1708">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="88779-1708">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-1709">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-1709">Consumption</span></span>
* <span data-ttu-id="88779-1710">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="88779-1710">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1711">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-1711">CosmosDB</span></span>
* <span data-ttu-id="88779-1712">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="88779-1712">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="88779-1713">Cartes</span><span class="sxs-lookup"><span data-stu-id="88779-1713">Maps</span></span>
* <span data-ttu-id="88779-1714">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1714">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1715">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1715">Network</span></span>
* <span data-ttu-id="88779-1716">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="88779-1716">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="88779-1717">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-1717">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1718">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1718">Resource</span></span>
* <span data-ttu-id="88779-1719">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1719">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="88779-1720">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1720">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1721">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1721">Storage</span></span>
*  <span data-ttu-id="88779-1722">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="88779-1722">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1723">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1723">VM</span></span>
* <span data-ttu-id="88779-1724">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="88779-1724">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="88779-1725">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1725">December 4, 2018</span></span>

<span data-ttu-id="88779-1726">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="88779-1726">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="88779-1727">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1727">Core</span></span>
* <span data-ttu-id="88779-1728">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="88779-1728">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="88779-1729">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="88779-1729">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1730">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1730">Appservice</span></span>
* <span data-ttu-id="88779-1731">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="88779-1731">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="88779-1732">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="88779-1732">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="88779-1733">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1733">Network</span></span>
* <span data-ttu-id="88779-1734">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="88779-1734">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="88779-1735">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1735">Role</span></span>
* <span data-ttu-id="88779-1736">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="88779-1736">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="88779-1737">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1737">VM</span></span>
* <span data-ttu-id="88779-1738">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="88779-1738">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="88779-1739">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="88779-1739">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="88779-1740">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="88779-1740">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="88779-1741">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="88779-1741">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="88779-1742">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1742">November 20, 2018</span></span>

<span data-ttu-id="88779-1743">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="88779-1743">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="88779-1744">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1744">Core</span></span>
* <span data-ttu-id="88779-1745">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="88779-1745">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1746">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1746">ACR</span></span>
* <span data-ttu-id="88779-1747">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="88779-1747">Added context token to task step</span></span>
* <span data-ttu-id="88779-1748">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="88779-1748">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="88779-1749">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="88779-1749">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1750">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1750">Appservice</span></span>
* <span data-ttu-id="88779-1751">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="88779-1751">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="88779-1752">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="88779-1752">Updated the default `node_version`.</span></span> <span data-ttu-id="88779-1753">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="88779-1753">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="88779-1754">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="88779-1754">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="88779-1755">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="88779-1755">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="88779-1756">IotCentral</span><span class="sxs-lookup"><span data-stu-id="88779-1756">IotCentral</span></span>
* <span data-ttu-id="88779-1757">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="88779-1757">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-1758">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-1758">KeyVault</span></span>
* <span data-ttu-id="88779-1759">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="88779-1759">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="88779-1760">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1760">Network</span></span>
* <span data-ttu-id="88779-1761">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="88779-1761">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="88779-1762">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="88779-1762">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="88779-1763">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="88779-1763">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="88779-1764">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="88779-1764">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1765">Rdbms</span><span class="sxs-lookup"><span data-stu-id="88779-1765">Rdbms</span></span>
* <span data-ttu-id="88779-1766">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="88779-1766">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="88779-1767">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="88779-1767">Rbac</span></span>
* <span data-ttu-id="88779-1768">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="88779-1768">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="88779-1769">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="88779-1769">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="88779-1770">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1770">Storage</span></span>
* <span data-ttu-id="88779-1771">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1771">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="88779-1772">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="88779-1772">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="88779-1773">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="88779-1773">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="88779-1774">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="88779-1774">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1775">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1775">VM</span></span>
* <span data-ttu-id="88779-1776">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="88779-1776">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="88779-1777">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="88779-1777">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="88779-1778">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="88779-1778">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="88779-1779">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="88779-1779">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="88779-1780">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="88779-1780">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="88779-1781">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="88779-1781">Added `snapshot wait` command</span></span>
* <span data-ttu-id="88779-1782">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="88779-1782">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="88779-1783">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1783">November 6, 2018</span></span>

<span data-ttu-id="88779-1784">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="88779-1784">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="88779-1785">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1785">Core</span></span>
* <span data-ttu-id="88779-1786">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="88779-1786">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1787">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1787">ACR</span></span>
* <span data-ttu-id="88779-1788">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="88779-1788">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="88779-1789">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="88779-1789">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1790">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1790">ACS</span></span>
* <span data-ttu-id="88779-1791">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-1791">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="88779-1792">Advisor</span><span class="sxs-lookup"><span data-stu-id="88779-1792">Advisor</span></span>
* <span data-ttu-id="88779-1793">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="88779-1793">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="88779-1794">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-1794">AMS</span></span>
* <span data-ttu-id="88779-1795">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="88779-1795">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="88779-1796">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="88779-1796">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="88779-1797">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="88779-1797">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="88779-1798">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="88779-1798">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="88779-1799">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="88779-1799">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="88779-1800">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="88779-1800">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="88779-1801">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="88779-1801">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="88779-1802">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="88779-1802">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="88779-1803">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="88779-1803">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="88779-1804">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="88779-1804">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="88779-1805">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-1805">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="88779-1806">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="88779-1806">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="88779-1807">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="88779-1807">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="88779-1808">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="88779-1808">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="88779-1809">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="88779-1809">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="88779-1810">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="88779-1810">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="88779-1811">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="88779-1811">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1812">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1812">AppService</span></span>
* <span data-ttu-id="88779-1813">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="88779-1813">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="88779-1814">Configurer</span><span class="sxs-lookup"><span data-stu-id="88779-1814">Configure</span></span>
* <span data-ttu-id="88779-1815">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="88779-1815">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="88779-1816">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1816">Container</span></span>
* <span data-ttu-id="88779-1817">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="88779-1817">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="88779-1818">Event Hub</span><span class="sxs-lookup"><span data-stu-id="88779-1818">EventHub</span></span>
* <span data-ttu-id="88779-1819">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1819">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-1820">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-1820">Interactive</span></span>
* <span data-ttu-id="88779-1821">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="88779-1821">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1822">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1822">Monitor</span></span>
* <span data-ttu-id="88779-1823">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-1823">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1824">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1824">Network</span></span>
* <span data-ttu-id="88779-1825">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="88779-1825">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="88779-1826">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="88779-1826">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="88779-1827">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="88779-1827">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="88779-1828">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-1828">Profile</span></span>
* <span data-ttu-id="88779-1829">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="88779-1829">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-1830">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-1830">RDBMS</span></span>
* <span data-ttu-id="88779-1831">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="88779-1831">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="88779-1832">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-1832">Resource</span></span>
* <span data-ttu-id="88779-1833">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="88779-1833">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="88779-1834">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1834">Role</span></span>
* <span data-ttu-id="88779-1835">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="88779-1835">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="88779-1836">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="88779-1836">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="88779-1837">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="88779-1837">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1838">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1838">Storage</span></span>
* <span data-ttu-id="88779-1839">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="88779-1839">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1840">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1840">VM</span></span>
* <span data-ttu-id="88779-1841">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="88779-1841">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="88779-1842">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="88779-1842">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="88779-1843">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="88779-1843">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="88779-1844">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="88779-1844">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="88779-1845">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="88779-1845">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="88779-1846">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="88779-1846">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="88779-1847">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1847">October 23, 2018</span></span>

<span data-ttu-id="88779-1848">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="88779-1848">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="88779-1849">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1849">Core</span></span>
* <span data-ttu-id="88779-1850">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="88779-1850">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="88779-1851">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="88779-1851">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1852">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1852">ACR</span></span>
* <span data-ttu-id="88779-1853">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="88779-1853">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-1854">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-1854">CDN</span></span>
* <span data-ttu-id="88779-1855">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="88779-1855">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="88779-1856">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="88779-1856">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="88779-1857">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1857">Container</span></span>
* <span data-ttu-id="88779-1858">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="88779-1858">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="88779-1859">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-1859">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="88779-1860">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="88779-1860">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="88779-1861">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-1861">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="88779-1862">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="88779-1862">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="88779-1863">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="88779-1863">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="88779-1864">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="88779-1864">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-1865">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-1865">CosmosDB</span></span>
* <span data-ttu-id="88779-1866">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="88779-1866">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-1867">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-1867">Interactive</span></span>
* <span data-ttu-id="88779-1868">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="88779-1868">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="88779-1869">IoT Central</span><span class="sxs-lookup"><span data-stu-id="88779-1869">IoT Central</span></span>
* <span data-ttu-id="88779-1870">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="88779-1870">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="88779-1871">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="88779-1871">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-1872">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-1872">Monitor</span></span>
* <span data-ttu-id="88779-1873">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="88779-1873">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="88779-1874">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-1874">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="88779-1875">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="88779-1875">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="88779-1876">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="88779-1876">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="88779-1877">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="88779-1877">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="88779-1878">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="88779-1878">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="88779-1879">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="88779-1879">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="88779-1880">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="88779-1880">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="88779-1881">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="88779-1881">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="88779-1882">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="88779-1882">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="88779-1883">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1883">Network</span></span>
* <span data-ttu-id="88779-1884">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1884">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="88779-1885">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1885">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="88779-1886">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="88779-1886">ServiceBus</span></span>
* <span data-ttu-id="88779-1887">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-1887">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="88779-1888">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-1888">SQL</span></span>
* <span data-ttu-id="88779-1889">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="88779-1889">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="88779-1890">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-1890">Storage</span></span>
* <span data-ttu-id="88779-1891">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="88779-1891">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="88779-1892">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="88779-1892">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1893">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1893">VM</span></span>
* <span data-ttu-id="88779-1894">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-1894">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="88779-1895">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-1895">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="88779-1896">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="88779-1896">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="88779-1897">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1897">October 16, 2018</span></span>

<span data-ttu-id="88779-1898">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="88779-1898">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1899">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1899">VM</span></span>
* <span data-ttu-id="88779-1900">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="88779-1900">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="88779-1901">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1901">October 9, 2018</span></span>

<span data-ttu-id="88779-1902">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="88779-1902">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="88779-1903">Core</span><span class="sxs-lookup"><span data-stu-id="88779-1903">Core</span></span>
* <span data-ttu-id="88779-1904">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="88779-1904">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1905">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1905">ACR</span></span>
* <span data-ttu-id="88779-1906">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="88779-1906">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1907">ACS</span></span>
* <span data-ttu-id="88779-1908">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="88779-1908">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="88779-1909">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="88779-1909">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="88779-1910">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="88779-1910">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="88779-1911">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="88779-1911">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="88779-1912">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1912">Container</span></span>
* <span data-ttu-id="88779-1913">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="88779-1913">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="88779-1914">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="88779-1914">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="88779-1915">Event Hub</span><span class="sxs-lookup"><span data-stu-id="88779-1915">Event Hub</span></span>
* <span data-ttu-id="88779-1916">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="88779-1916">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="88779-1917">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="88779-1917">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="88779-1918">Extensions</span><span class="sxs-lookup"><span data-stu-id="88779-1918">Extensions</span></span>
* <span data-ttu-id="88779-1919">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="88779-1919">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="88779-1920">HDInsight</span><span class="sxs-lookup"><span data-stu-id="88779-1920">HDInsight</span></span>
* <span data-ttu-id="88779-1921">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-1921">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1922">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1922">IoT</span></span>
* <span data-ttu-id="88779-1923">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="88779-1923">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-1924">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-1924">KeyVault</span></span>
* <span data-ttu-id="88779-1925">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="88779-1925">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="88779-1926">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1926">Network</span></span>
* <span data-ttu-id="88779-1927">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="88779-1927">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="88779-1928">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="88779-1928">See #6052</span></span>
* <span data-ttu-id="88779-1929">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="88779-1929">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="88779-1930">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="88779-1930">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="88779-1931">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="88779-1931">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="88779-1932">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="88779-1932">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="88779-1933">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="88779-1933">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="88779-1934">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="88779-1934">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="88779-1935">Role</span><span class="sxs-lookup"><span data-stu-id="88779-1935">Role</span></span>
* <span data-ttu-id="88779-1936">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="88779-1936">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="88779-1937">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="88779-1937">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="88779-1938">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="88779-1938">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="88779-1939">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="88779-1939">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="88779-1940">Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-1940">Service Bus</span></span>
* <span data-ttu-id="88779-1941">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="88779-1941">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="88779-1942">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-1942">VM</span></span>
* <span data-ttu-id="88779-1943">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="88779-1943">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="88779-1944">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="88779-1944">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="88779-1945">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="88779-1945">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="88779-1946">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="88779-1946">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="88779-1947">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="88779-1947">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="88779-1948">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="88779-1948">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="88779-1949">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="88779-1949">September 21, 2018</span></span>

<span data-ttu-id="88779-1950">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="88779-1950">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="88779-1951">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1951">ACR</span></span>
* <span data-ttu-id="88779-1952">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1952">Added ACR Task commands</span></span>
* <span data-ttu-id="88779-1953">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="88779-1953">Added quick run command</span></span>
* <span data-ttu-id="88779-1954">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="88779-1954">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="88779-1955">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="88779-1955">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="88779-1956">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="88779-1956">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="88779-1957">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="88779-1957">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="88779-1958">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-1958">ACS</span></span>
* <span data-ttu-id="88779-1959">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="88779-1959">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="88779-1960">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="88779-1960">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-1961">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-1961">AppService</span></span>

* <span data-ttu-id="88779-1962">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="88779-1962">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="88779-1963">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="88779-1963">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="88779-1964">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="88779-1964">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="88779-1965">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="88779-1965">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="88779-1966">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-1966">Batch</span></span>
* <span data-ttu-id="88779-1967">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="88779-1967">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="88779-1968">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="88779-1968">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="88779-1969">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="88779-1969">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="88779-1970">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="88779-1970">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="88779-1971">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-1971">Batch AI</span></span> 
* <span data-ttu-id="88779-1972">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="88779-1972">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="88779-1973">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-1973">Cognitive Services</span></span>
* <span data-ttu-id="88779-1974">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="88779-1974">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="88779-1975">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="88779-1975">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="88779-1976">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="88779-1976">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="88779-1977">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="88779-1977">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="88779-1978">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="88779-1978">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="88779-1979">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="88779-1979">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="88779-1980">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-1980">Container</span></span>
* <span data-ttu-id="88779-1981">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="88779-1981">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="88779-1982">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1982">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="88779-1983">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="88779-1983">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="88779-1984">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-1984">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="88779-1985">DataLake</span><span class="sxs-lookup"><span data-stu-id="88779-1985">Datalake</span></span>
* <span data-ttu-id="88779-1986">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="88779-1986">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="88779-1987">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="88779-1987">Interactive Shell</span></span>
* <span data-ttu-id="88779-1988">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="88779-1988">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="88779-1989">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="88779-1989">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="88779-1990">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1990">IoT</span></span>
* <span data-ttu-id="88779-1991">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="88779-1991">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-1992">Key Vault</span><span class="sxs-lookup"><span data-stu-id="88779-1992">Key Vault</span></span>
* <span data-ttu-id="88779-1993">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="88779-1993">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="88779-1994">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-1994">Network</span></span>
* <span data-ttu-id="88779-1995">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="88779-1995">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="88779-1996">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="88779-1996">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="88779-1997">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="88779-1997">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="88779-1998">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="88779-1998">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="88779-1999">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="88779-1999">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="88779-2000">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="88779-2000">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="88779-2001">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="88779-2001">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="88779-2002">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="88779-2002">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="88779-2003">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="88779-2003">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="88779-2004">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="88779-2004">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="88779-2005">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="88779-2005">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="88779-2006">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="88779-2006">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="88779-2007">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="88779-2007">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="88779-2008">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="88779-2008">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="88779-2009">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="88779-2009">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="88779-2010">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="88779-2010">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="88779-2011">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2011">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="88779-2012">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="88779-2012">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-2013">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-2013">RDBMS</span></span>
* <span data-ttu-id="88779-2014">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="88779-2014">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="88779-2015">Réservation</span><span class="sxs-lookup"><span data-stu-id="88779-2015">Reservation</span></span>
* <span data-ttu-id="88779-2016">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="88779-2016">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="88779-2017">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="88779-2017">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="88779-2018">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="88779-2018">Manage App</span></span>
* <span data-ttu-id="88779-2019">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="88779-2019">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="88779-2020">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="88779-2020">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="88779-2021">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2021">Role</span></span>
* <span data-ttu-id="88779-2022">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="88779-2022">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="88779-2023">SignalR</span><span class="sxs-lookup"><span data-stu-id="88779-2023">SignalR</span></span>
* <span data-ttu-id="88779-2024">Première version</span><span class="sxs-lookup"><span data-stu-id="88779-2024">First release</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2025">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2025">Storage</span></span>
* <span data-ttu-id="88779-2026">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="88779-2026">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="88779-2027">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="88779-2027">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2028">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2028">VM</span></span>
* <span data-ttu-id="88779-2029">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="88779-2029">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="88779-2030">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="88779-2030">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="88779-2031">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2031">August 28, 2018</span></span>

<span data-ttu-id="88779-2032">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="88779-2032">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="88779-2033">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2033">Core</span></span>

* <span data-ttu-id="88779-2034">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="88779-2034">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="88779-2035">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="88779-2035">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2036">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2036">ACR</span></span>

* <span data-ttu-id="88779-2037">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="88779-2037">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="88779-2038">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="88779-2038">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2039">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2039">ACS</span></span>

* <span data-ttu-id="88779-2040">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="88779-2040">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="88779-2041">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="88779-2041">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2042">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2042">AppService</span></span>

* <span data-ttu-id="88779-2043">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="88779-2043">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="88779-2044">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="88779-2044">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="88779-2045">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2045">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="88779-2046">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-2046">Backup</span></span>

* <span data-ttu-id="88779-2047">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2047">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="88779-2048">Service de robot</span><span class="sxs-lookup"><span data-stu-id="88779-2048">Bot Service</span></span>

* <span data-ttu-id="88779-2049">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="88779-2049">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="88779-2050">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-2050">Cognitive Services</span></span>

* <span data-ttu-id="88779-2051">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="88779-2051">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="88779-2052">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2052">IoT</span></span>

* <span data-ttu-id="88779-2053">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="88779-2053">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2054">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2054">Monitor</span></span>

* <span data-ttu-id="88779-2055">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="88779-2055">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="88779-2056">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="88779-2056">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="88779-2057">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2057">Network</span></span>

* <span data-ttu-id="88779-2058">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2058">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2059">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2059">Resource</span></span>

* <span data-ttu-id="88779-2060">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2060">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2061">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2061">Storage</span></span>

* <span data-ttu-id="88779-2062">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2062">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2063">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2063">VM</span></span>

* <span data-ttu-id="88779-2064">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2064">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="88779-2065">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-2065">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="88779-2066">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2066">Auguest 14, 2018</span></span>

<span data-ttu-id="88779-2067">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="88779-2067">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="88779-2068">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2068">Core</span></span>

* <span data-ttu-id="88779-2069">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="88779-2069">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="88779-2070">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="88779-2070">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="88779-2071">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="88779-2071">Telemetry</span></span>

* <span data-ttu-id="88779-2072">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="88779-2072">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2073">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2073">ACR</span></span>

* <span data-ttu-id="88779-2074">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="88779-2074">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="88779-2075">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="88779-2075">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2076">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2076">ACS</span></span>

* <span data-ttu-id="88779-2077">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-2077">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="88779-2078">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="88779-2078">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="88779-2079">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="88779-2079">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="88779-2080">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="88779-2080">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="88779-2081">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="88779-2081">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="88779-2082">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2082">AppService</span></span>

* <span data-ttu-id="88779-2083">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="88779-2083">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="88779-2084">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="88779-2084">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-2085">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2085">BatchAI</span></span>

* <span data-ttu-id="88779-2086">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="88779-2086">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="88779-2087">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2087">Container</span></span>

* <span data-ttu-id="88779-2088">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2088">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="88779-2089">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2089">IoT</span></span>

* <span data-ttu-id="88779-2090">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="88779-2090">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="88779-2091">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="88779-2091">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="88779-2092">Iot Central</span><span class="sxs-lookup"><span data-stu-id="88779-2092">Iot Central</span></span>

* <span data-ttu-id="88779-2093">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="88779-2093">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-2094">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-2094">KeyVault</span></span>


* <span data-ttu-id="88779-2095">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="88779-2095">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="88779-2096">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2096">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="88779-2097">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="88779-2097">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="88779-2098">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="88779-2098">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="88779-2099">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="88779-2099">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="88779-2100">Relais</span><span class="sxs-lookup"><span data-stu-id="88779-2100">Relay</span></span>

* <span data-ttu-id="88779-2101">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2101">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2102">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2102">Sql</span></span>

* <span data-ttu-id="88779-2103">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="88779-2103">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2104">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2104">Storage</span></span>

* <span data-ttu-id="88779-2105">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="88779-2105">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="88779-2106">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="88779-2106">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="88779-2107">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="88779-2107">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="88779-2108">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="88779-2108">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="88779-2109">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2109">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2110">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2110">VM</span></span>

* <span data-ttu-id="88779-2111">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="88779-2111">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="88779-2112">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2112">July 31, 2018</span></span>

<span data-ttu-id="88779-2113">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="88779-2113">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2114">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2114">ACR</span></span>

* <span data-ttu-id="88779-2115">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="88779-2115">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="88779-2116">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="88779-2116">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2117">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2117">ACS</span></span>

* <span data-ttu-id="88779-2118">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="88779-2118">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2119">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2119">Batch</span></span>

* <span data-ttu-id="88779-2120">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-2120">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="88779-2121">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2121">Container</span></span>

* <span data-ttu-id="88779-2122">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="88779-2122">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="88779-2123">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2123">Network</span></span>

* <span data-ttu-id="88779-2124">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="88779-2124">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="88779-2125">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2125">Resource</span></span>

* <span data-ttu-id="88779-2126">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="88779-2126">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="88779-2127">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="88779-2127">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="88779-2128">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2128">Role</span></span>

* <span data-ttu-id="88779-2129">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="88779-2129">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="88779-2130">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="88779-2130">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="88779-2131">Recherche</span><span class="sxs-lookup"><span data-stu-id="88779-2131">Search</span></span>

* <span data-ttu-id="88779-2132">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="88779-2132">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="88779-2133">Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-2133">Service Bus</span></span>

* <span data-ttu-id="88779-2134">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="88779-2134">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="88779-2135">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-2135">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="88779-2136">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="88779-2136">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="88779-2137">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="88779-2137">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2138">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2138">Storage</span></span>

* <span data-ttu-id="88779-2139">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="88779-2139">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="88779-2140">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2140">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2141">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2141">VM</span></span>

* <span data-ttu-id="88779-2142">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-2142">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="88779-2143">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="88779-2143">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="88779-2144">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="88779-2144">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="88779-2145">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="88779-2145">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="88779-2146">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2146">July 18, 2018</span></span>

<span data-ttu-id="88779-2147">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="88779-2147">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="88779-2148">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2148">Core</span></span>

* <span data-ttu-id="88779-2149">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="88779-2149">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="88779-2150">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="88779-2150">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="88779-2151">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="88779-2151">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2152">ACR</span></span>

* <span data-ttu-id="88779-2153">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="88779-2153">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="88779-2154">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="88779-2154">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="88779-2155">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="88779-2155">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="88779-2156">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="88779-2156">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2157">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2157">ACS</span></span>

* <span data-ttu-id="88779-2158">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="88779-2158">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2159">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2159">AppService</span></span>

* <span data-ttu-id="88779-2160">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="88779-2160">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2161">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2161">Batch</span></span>

* <span data-ttu-id="88779-2162">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-2162">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="88779-2163">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="88779-2163">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="88779-2164">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2164">Batch AI</span></span>

* <span data-ttu-id="88779-2165">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="88779-2165">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="88779-2166">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2166">Container</span></span>

* <span data-ttu-id="88779-2167">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="88779-2167">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="88779-2168">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="88779-2168">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="88779-2169">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2169">Network</span></span>

* <span data-ttu-id="88779-2170">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="88779-2170">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="88779-2171">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="88779-2171">Added `network nic wait`</span></span>
* <span data-ttu-id="88779-2172">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="88779-2172">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="88779-2173">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="88779-2173">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="88779-2174">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2174">Resource</span></span>

* <span data-ttu-id="88779-2175">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="88779-2175">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="88779-2176">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="88779-2176">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="88779-2177">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="88779-2177">Added `deployment wait` command</span></span>
* <span data-ttu-id="88779-2178">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="88779-2178">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2179">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2179">SQL</span></span>

* <span data-ttu-id="88779-2180">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="88779-2180">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="88779-2181">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="88779-2181">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="88779-2182">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="88779-2182">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2183">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2183">Storage</span></span>

* <span data-ttu-id="88779-2184">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="88779-2184">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2185">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2185">VM</span></span>

* <span data-ttu-id="88779-2186">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2186">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="88779-2187">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="88779-2187">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="88779-2188">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="88779-2188">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="88779-2189">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2189">July 3, 2018</span></span>

<span data-ttu-id="88779-2190">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="88779-2190">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="88779-2191">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-2191">AKS</span></span>

* <span data-ttu-id="88779-2192">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-2192">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="88779-2193">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2193">July 3, 2018</span></span>

<span data-ttu-id="88779-2194">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="88779-2194">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="88779-2195">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2195">Core</span></span>

* <span data-ttu-id="88779-2196">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2196">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2197">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2197">ACR</span></span>

* <span data-ttu-id="88779-2198">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="88779-2198">Added polling build status</span></span>
* <span data-ttu-id="88779-2199">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="88779-2199">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="88779-2200">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="88779-2200">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2201">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2201">ACS</span></span>

* <span data-ttu-id="88779-2202">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2202">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="88779-2203">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2203">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="88779-2204">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="88779-2204">Updated options for `aks browse` command.</span></span> <span data-ttu-id="88779-2205">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="88779-2205">Added `--listen-port` support</span></span>
* <span data-ttu-id="88779-2206">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="88779-2206">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="88779-2207">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="88779-2207">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="88779-2208">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="88779-2208">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2209">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2209">AppService</span></span>

* <span data-ttu-id="88779-2210">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="88779-2210">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="88779-2211">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="88779-2211">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="88779-2212">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-2212">Backup</span></span>

* <span data-ttu-id="88779-2213">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="88779-2213">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-2214">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2214">BatchAI</span></span>

* <span data-ttu-id="88779-2215">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="88779-2215">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="88779-2216">Cloud</span><span class="sxs-lookup"><span data-stu-id="88779-2216">Cloud</span></span>

* <span data-ttu-id="88779-2217">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="88779-2217">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="88779-2218">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2218">Container</span></span>

* <span data-ttu-id="88779-2219">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="88779-2219">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="88779-2220">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="88779-2220">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="88779-2221">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="88779-2221">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2222">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2222">Extension</span></span>

* <span data-ttu-id="88779-2223">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="88779-2223">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="88779-2224">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2224">Network</span></span>

* <span data-ttu-id="88779-2225">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="88779-2225">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-2226">Rdbms</span><span class="sxs-lookup"><span data-stu-id="88779-2226">Rdbms</span></span>

* <span data-ttu-id="88779-2227">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-2227">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2228">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2228">Resource</span></span>

* <span data-ttu-id="88779-2229">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="88779-2229">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2230">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2230">VM</span></span>

* <span data-ttu-id="88779-2231">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="88779-2231">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="88779-2232">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2232">June 25, 2018</span></span>

<span data-ttu-id="88779-2233">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="88779-2233">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="88779-2234">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="88779-2234">CLI</span></span>

* <span data-ttu-id="88779-2235">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="88779-2235">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="88779-2236">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2236">June 19, 2018</span></span>

<span data-ttu-id="88779-2237">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="88779-2237">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="88779-2238">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2238">Core</span></span>

* <span data-ttu-id="88779-2239">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2239">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2240">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2240">ACR</span></span>

* <span data-ttu-id="88779-2241">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="88779-2241">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="88779-2242">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="88779-2242">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2243">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2243">ACS</span></span>

* <span data-ttu-id="88779-2244">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="88779-2244">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="88779-2245">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="88779-2245">Added `--update` support</span></span>
* <span data-ttu-id="88779-2246">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="88779-2246">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="88779-2247">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="88779-2247">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="88779-2248">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="88779-2248">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="88779-2249">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="88779-2249">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="88779-2250">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="88779-2250">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="88779-2251">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="88779-2251">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2252">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2252">AppService</span></span>

* <span data-ttu-id="88779-2253">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="88779-2253">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="88779-2254">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="88779-2254">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2255">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2255">Batch</span></span>

* <span data-ttu-id="88779-2256">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="88779-2256">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="88779-2257">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2257">Batch AI</span></span>

* <span data-ttu-id="88779-2258">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="88779-2258">Added support for workspaces.</span></span> <span data-ttu-id="88779-2259">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="88779-2259">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="88779-2260">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="88779-2260">Added support for experiments.</span></span> <span data-ttu-id="88779-2261">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="88779-2261">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="88779-2262">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="88779-2262">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="88779-2263">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="88779-2263">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="88779-2264">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="88779-2264">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="88779-2265">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="88779-2265">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="88779-2266">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="88779-2266">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="88779-2267">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="88779-2267">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="88779-2268">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="88779-2268">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="88779-2269">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="88779-2269">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="88779-2270">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="88779-2270">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="88779-2271">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="88779-2271">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="88779-2272">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="88779-2272">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="88779-2273">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="88779-2273">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="88779-2274">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="88779-2274">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="88779-2275">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="88779-2275">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="88779-2276">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="88779-2276">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="88779-2277">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="88779-2277">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="88779-2278">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="88779-2278">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="88779-2279">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="88779-2279">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="88779-2280">Cartes</span><span class="sxs-lookup"><span data-stu-id="88779-2280">Maps</span></span>

* <span data-ttu-id="88779-2281">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="88779-2281">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="88779-2282">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2282">Network</span></span>

* <span data-ttu-id="88779-2283">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="88779-2283">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="88779-2284">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="88779-2284">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="88779-2285">#6502</span><span class="sxs-lookup"><span data-stu-id="88779-2285">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="88779-2286">Réservations</span><span class="sxs-lookup"><span data-stu-id="88779-2286">Reservations</span></span>

* <span data-ttu-id="88779-2287">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="88779-2287">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="88779-2288">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="88779-2288">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="88779-2289">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="88779-2289">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="88779-2290">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="88779-2290">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="88779-2291">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="88779-2291">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="88779-2292">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="88779-2292">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="88779-2293">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2293">Role</span></span>

* <span data-ttu-id="88779-2294">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="88779-2294">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2295">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2295">SQL</span></span>

* <span data-ttu-id="88779-2296">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-2296">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2297">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2297">Storage</span></span>

* <span data-ttu-id="88779-2298">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="88779-2298">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2299">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2299">VM</span></span>

* <span data-ttu-id="88779-2300">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-2300">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="88779-2301">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="88779-2301">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="88779-2302">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="88779-2302">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="88779-2303">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2303">June 13, 2018</span></span>

<span data-ttu-id="88779-2304">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="88779-2304">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="88779-2305">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2305">Core</span></span>

* <span data-ttu-id="88779-2306">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2306">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="88779-2307">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2307">June 13, 2018</span></span>

<span data-ttu-id="88779-2308">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="88779-2308">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="88779-2309">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-2309">AKS</span></span>

* <span data-ttu-id="88779-2310">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-2310">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="88779-2311">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="88779-2311">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="88779-2312">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-2312">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="88779-2313">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-2313">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="88779-2314">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-2314">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2315">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2315">AppService</span></span>

* <span data-ttu-id="88779-2316">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="88779-2316">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="88779-2317">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2317">June 5, 2018</span></span>

<span data-ttu-id="88779-2318">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="88779-2318">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2319">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2319">Interactive</span></span>

* <span data-ttu-id="88779-2320">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="88779-2320">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="88779-2321">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2321">June 5, 2018</span></span>

<span data-ttu-id="88779-2322">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="88779-2322">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="88779-2323">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2323">Core</span></span>

* <span data-ttu-id="88779-2324">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="88779-2324">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="88779-2325">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="88779-2325">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2326">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2326">ACR</span></span>

* <span data-ttu-id="88779-2327">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="88779-2327">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="88779-2328">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="88779-2328">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="88779-2329">AKS</span><span class="sxs-lookup"><span data-stu-id="88779-2329">AKS</span></span>

* <span data-ttu-id="88779-2330">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="88779-2330">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2331">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2331">Batch</span></span>

* <span data-ttu-id="88779-2332">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="88779-2332">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="88779-2333">IOT</span><span class="sxs-lookup"><span data-stu-id="88779-2333">IOT</span></span>

* <span data-ttu-id="88779-2334">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="88779-2334">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="88779-2335">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2335">Network</span></span>

* <span data-ttu-id="88779-2336">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="88779-2336">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="88779-2337">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="88779-2337">Policy Insights</span></span>

* <span data-ttu-id="88779-2338">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2338">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="88779-2339">ARM</span><span class="sxs-lookup"><span data-stu-id="88779-2339">ARM</span></span>

* <span data-ttu-id="88779-2340">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="88779-2340">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2341">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2341">SQL</span></span>

* <span data-ttu-id="88779-2342">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="88779-2342">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="88779-2343">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="88779-2343">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="88779-2344">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2344">Storage</span></span>

* <span data-ttu-id="88779-2345">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="88779-2345">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2346">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2346">VM</span></span>

* <span data-ttu-id="88779-2347">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="88779-2347">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="88779-2348">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-2348">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="88779-2349">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="88779-2349">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="88779-2350">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2350">May 22, 2018</span></span>

<span data-ttu-id="88779-2351">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="88779-2351">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="88779-2352">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2352">Core</span></span>

* <span data-ttu-id="88779-2353">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="88779-2353">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2354">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2354">ACS</span></span>

* <span data-ttu-id="88779-2355">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="88779-2355">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="88779-2356">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="88779-2356">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2357">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2357">AppService</span></span>

* <span data-ttu-id="88779-2358">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="88779-2358">Improved generic update commands</span></span>
* <span data-ttu-id="88779-2359">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="88779-2359">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="88779-2360">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2360">Container</span></span>

* <span data-ttu-id="88779-2361">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="88779-2361">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="88779-2362">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-2362">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2363">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2363">Extension</span></span>

* <span data-ttu-id="88779-2364">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="88779-2364">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2365">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2365">Interactive</span></span>

* <span data-ttu-id="88779-2366">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="88779-2366">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="88779-2367">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="88779-2367">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-2368">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-2368">KeyVault</span></span>

* <span data-ttu-id="88779-2369">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="88779-2369">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="88779-2370">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2370">Network</span></span>

* <span data-ttu-id="88779-2371">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="88779-2371">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="88779-2372">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="88779-2372">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2373">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2373">SQL</span></span>

* <span data-ttu-id="88779-2374">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="88779-2374">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="88779-2375">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="88779-2375">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="88779-2376">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="88779-2376">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="88779-2377">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="88779-2377">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="88779-2378">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="88779-2378">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="88779-2379">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="88779-2379">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="88779-2380">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="88779-2380">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="88779-2381">`edition`.</span><span class="sxs-lookup"><span data-stu-id="88779-2381">`edition`.</span></span> <span data-ttu-id="88779-2382">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="88779-2382">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="88779-2383">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="88779-2383">`elasticPoolName`.</span></span> <span data-ttu-id="88779-2384">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="88779-2384">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="88779-2385">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="88779-2385">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="88779-2386">`edition`.</span><span class="sxs-lookup"><span data-stu-id="88779-2386">`edition`.</span></span> <span data-ttu-id="88779-2387">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="88779-2387">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="88779-2388">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="88779-2388">`dtu`.</span></span> <span data-ttu-id="88779-2389">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="88779-2389">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="88779-2390">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="88779-2390">`databaseDtuMin`.</span></span> <span data-ttu-id="88779-2391">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="88779-2391">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="88779-2392">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="88779-2392">`databaseDtuMax`.</span></span> <span data-ttu-id="88779-2393">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="88779-2393">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="88779-2394">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="88779-2394">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="88779-2395">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="88779-2395">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2396">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2396">Storage</span></span>

* <span data-ttu-id="88779-2397">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="88779-2397">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="88779-2398">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="88779-2398">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2399">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2399">VM</span></span>

* <span data-ttu-id="88779-2400">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="88779-2400">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="88779-2401">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="88779-2401">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="88779-2402">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="88779-2402">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="88779-2403">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="88779-2403">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="88779-2404">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="88779-2404">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="88779-2405">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2405">May 7, 2018</span></span>

<span data-ttu-id="88779-2406">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="88779-2406">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="88779-2407">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2407">Core</span></span>

* <span data-ttu-id="88779-2408">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="88779-2408">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="88779-2409">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="88779-2409">Added limited support for positional arguments</span></span>
* <span data-ttu-id="88779-2410">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="88779-2410">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="88779-2411">#5591</span><span class="sxs-lookup"><span data-stu-id="88779-2411">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="88779-2412">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="88779-2412">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="88779-2413">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="88779-2413">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="88779-2414">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2414">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="88779-2415">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="88779-2415">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="88779-2416">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="88779-2416">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2417">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2417">ACR</span></span>

* <span data-ttu-id="88779-2418">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2418">Added ACR Build commands</span></span>
* <span data-ttu-id="88779-2419">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="88779-2419">Improved resource not found error messages</span></span>
* <span data-ttu-id="88779-2420">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="88779-2420">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="88779-2421">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="88779-2421">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="88779-2422">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="88779-2422">Improved repository commands error messages</span></span>
* <span data-ttu-id="88779-2423">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="88779-2423">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2424">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2424">ACS</span></span>

* <span data-ttu-id="88779-2425">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="88779-2425">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="88779-2426">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="88779-2426">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="88779-2427">AMS</span><span class="sxs-lookup"><span data-stu-id="88779-2427">AMS</span></span>

* <span data-ttu-id="88779-2428">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="88779-2428">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2429">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2429">Appservice</span></span>

* <span data-ttu-id="88779-2430">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="88779-2430">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="88779-2431">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="88779-2431">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="88779-2432">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="88779-2432">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="88779-2433">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-2433">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="88779-2434">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2434">Batch AI</span></span>

* <span data-ttu-id="88779-2435">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="88779-2435">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="88779-2436">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-2436">Cognitive Services</span></span>

* <span data-ttu-id="88779-2437">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="88779-2437">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-2438">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-2438">Consumption</span></span>

* <span data-ttu-id="88779-2439">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="88779-2439">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="88779-2440">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2440">Container</span></span>

* <span data-ttu-id="88779-2441">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="88779-2441">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="88779-2442">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-2442">Cosmos DB</span></span>

* <span data-ttu-id="88779-2443">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="88779-2443">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="88779-2444">DMS</span><span class="sxs-lookup"><span data-stu-id="88779-2444">DMS</span></span>

* <span data-ttu-id="88779-2445">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="88779-2445">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2446">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2446">Extension</span></span>

* <span data-ttu-id="88779-2447">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="88779-2447">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2448">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2448">Interactive</span></span>

* <span data-ttu-id="88779-2449">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="88779-2449">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="88779-2450">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="88779-2450">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="88779-2451">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="88779-2451">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="88779-2452">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2452">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="88779-2453">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-2453">Lab</span></span>

* <span data-ttu-id="88779-2454">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="88779-2454">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="88779-2455">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2455">Network</span></span>

* <span data-ttu-id="88779-2456">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="88779-2456">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="88779-2457">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2457">Profile</span></span>

* <span data-ttu-id="88779-2458">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="88779-2458">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="88779-2459">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="88779-2459">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="88779-2460">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="88779-2460">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="88779-2461">Redis</span><span class="sxs-lookup"><span data-stu-id="88779-2461">Redis</span></span>

* <span data-ttu-id="88779-2462">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="88779-2462">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="88779-2463">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="88779-2463">Deprecated `redis list-all`.</span></span> <span data-ttu-id="88779-2464">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="88779-2464">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="88779-2465">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="88779-2465">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="88779-2466">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2466">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="88779-2467">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2467">Role</span></span>

* <span data-ttu-id="88779-2468">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="88779-2468">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2469">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2469">Storage</span></span>

* <span data-ttu-id="88779-2470">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="88779-2470">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="88779-2471">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="88779-2471">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="88779-2472">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="88779-2472">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="88779-2473">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="88779-2473">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="88779-2474">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="88779-2474">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2475">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2475">VM</span></span>

* <span data-ttu-id="88779-2476">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="88779-2476">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="88779-2477">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="88779-2477">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="88779-2478">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="88779-2478">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="88779-2479">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="88779-2479">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="88779-2480">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="88779-2480">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="88779-2481">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="88779-2481">Added write accelerator support</span></span>
* <span data-ttu-id="88779-2482">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="88779-2482">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="88779-2483">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2483">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="88779-2484">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="88779-2484">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="88779-2485">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2485">April 10, 2018</span></span>

<span data-ttu-id="88779-2486">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="88779-2486">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2487">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2487">ACR</span></span>

* <span data-ttu-id="88779-2488">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="88779-2488">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2489">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2489">ACS</span></span>

* <span data-ttu-id="88779-2490">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="88779-2490">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2491">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2491">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="88779-2493">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="88779-2493">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-2494">Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2494">BatchAI</span></span>

* <span data-ttu-id="88779-2495">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="88779-2495">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="88779-2496">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="88779-2496">Job level mounting</span></span>
  - <span data-ttu-id="88779-2497">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="88779-2497">Environment variables with secret values</span></span>
  - <span data-ttu-id="88779-2498">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="88779-2498">Performance counters settings</span></span>
  - <span data-ttu-id="88779-2499">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="88779-2499">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="88779-2500">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="88779-2500">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="88779-2501">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="88779-2501">Usage and limits reporting</span></span>
  - <span data-ttu-id="88779-2502">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="88779-2502">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="88779-2503">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="88779-2503">Support for custom images</span></span>
  - <span data-ttu-id="88779-2504">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="88779-2504">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="88779-2505">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="88779-2505">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="88779-2506">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="88779-2506">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="88779-2507">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="88779-2507">National clouds are supported</span></span>
* <span data-ttu-id="88779-2508">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="88779-2508">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="88779-2509">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="88779-2509">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="88779-2510">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-2510">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="88779-2511">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="88779-2511">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="88779-2512">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="88779-2512">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="88779-2513">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="88779-2513">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="88779-2514">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="88779-2514">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="88779-2515">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="88779-2515">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="88779-2516">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="88779-2516">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="88779-2517">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="88779-2517">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="88779-2518">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="88779-2518">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="88779-2519">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="88779-2519">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="88779-2520">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="88779-2520">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="88779-2521">Facturation</span><span class="sxs-lookup"><span data-stu-id="88779-2521">Billing</span></span>

* <span data-ttu-id="88779-2522">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="88779-2522">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-2523">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-2523">Consumption</span></span>

* <span data-ttu-id="88779-2524">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="88779-2524">Added `marketplace` commands</span></span>
* <span data-ttu-id="88779-2525">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="88779-2525">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="88779-2526">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="88779-2526">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="88779-2527">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="88779-2527">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="88779-2528">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="88779-2528">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="88779-2529">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="88779-2529">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="88779-2530">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2530">Container</span></span>

* <span data-ttu-id="88779-2531">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="88779-2531">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="88779-2532">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="88779-2532">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2533">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2533">Extension</span></span>

* <span data-ttu-id="88779-2534">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="88779-2534">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2535">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2535">Interactive</span></span>

* <span data-ttu-id="88779-2536">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="88779-2536">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="88779-2537">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="88779-2537">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="88779-2538">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="88779-2538">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="88779-2539">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2539">Network</span></span>

* <span data-ttu-id="88779-2540">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="88779-2540">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="88779-2541">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="88779-2541">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="88779-2542">#4910</span><span class="sxs-lookup"><span data-stu-id="88779-2542">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="88779-2543">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="88779-2543">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="88779-2544">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="88779-2544">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="88779-2545">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2545">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="88779-2546">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2546">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="88779-2547">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="88779-2547">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-2548">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2548">Profile</span></span>

* <span data-ttu-id="88779-2549">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="88779-2549">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="88779-2550">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="88779-2550">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-2551">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-2551">RDBMS</span></span>

* <span data-ttu-id="88779-2552">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="88779-2552">Added `georestore` command</span></span>
* <span data-ttu-id="88779-2553">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="88779-2553">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2554">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2554">Resource</span></span>

* <span data-ttu-id="88779-2555">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="88779-2555">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="88779-2556">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="88779-2556">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2557">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2557">SQL</span></span>

* <span data-ttu-id="88779-2558">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="88779-2558">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2559">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2559">Storage</span></span>

* <span data-ttu-id="88779-2560">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="88779-2560">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2561">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2561">VM</span></span>

* <span data-ttu-id="88779-2562">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="88779-2562">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="88779-2563">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="88779-2563">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="88779-2565">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-2565">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="88779-2566">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="88779-2566">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="88779-2567">#5718</span><span class="sxs-lookup"><span data-stu-id="88779-2567">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="88779-2568">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="88779-2568">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="88779-2569">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2569">March 27, 2018</span></span>

<span data-ttu-id="88779-2570">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="88779-2570">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="88779-2571">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2571">Core</span></span>

* <span data-ttu-id="88779-2572">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="88779-2572">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2573">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2573">ACS</span></span>

* <span data-ttu-id="88779-2574">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-2574">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2575">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2575">Appservice</span></span>

* <span data-ttu-id="88779-2576">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="88779-2576">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="88779-2577">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-2577">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="88779-2578">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-2578">Backup</span></span>

* <span data-ttu-id="88779-2579">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="88779-2579">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="88779-2580">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-2580">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="88779-2581">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="88779-2581">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="88779-2582">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="88779-2582">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="88779-2583">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2583">Container</span></span>

* <span data-ttu-id="88779-2584">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="88779-2584">Added `container exec` command.</span></span> <span data-ttu-id="88779-2585">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="88779-2585">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="88779-2586">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-2586">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2587">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2587">Extension</span></span>

* <span data-ttu-id="88779-2588">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="88779-2588">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="88779-2589">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="88779-2589">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="88779-2590">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2590">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2591">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2591">Interactive</span></span>

* <span data-ttu-id="88779-2592">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="88779-2592">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="88779-2593">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="88779-2593">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="88779-2594">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="88779-2594">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="88779-2595">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="88779-2595">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="88779-2596">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-2596">Lab</span></span>

* <span data-ttu-id="88779-2597">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="88779-2597">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2598">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2598">Monitor</span></span>

* <span data-ttu-id="88779-2599">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="88779-2599">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="88779-2600">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="88779-2600">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="88779-2601">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="88779-2601">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="88779-2602">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2602">Network</span></span>

* <span data-ttu-id="88779-2603">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="88779-2603">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="88779-2604">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2604">Profile</span></span>

* <span data-ttu-id="88779-2605">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="88779-2605">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-2606">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-2606">RDBMS</span></span>

* <span data-ttu-id="88779-2607">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="88779-2607">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2608">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2608">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="88779-2610">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2610">Role</span></span>

* <span data-ttu-id="88779-2611">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="88779-2611">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="88779-2612">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="88779-2612">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="88779-2613">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="88779-2613">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="88779-2614">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-2614">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="88779-2615">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="88779-2615">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2616">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2616">Storage</span></span>

* <span data-ttu-id="88779-2617">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="88779-2617">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="88779-2618">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="88779-2618">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2619">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2619">VM</span></span>

* <span data-ttu-id="88779-2620">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="88779-2620">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="88779-2621">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="88779-2621">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="88779-2622">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="88779-2622">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="88779-2623">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="88779-2623">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="88779-2624">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2624">March 13, 2018</span></span>

<span data-ttu-id="88779-2625">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="88779-2625">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2626">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2626">ACR</span></span>

* <span data-ttu-id="88779-2627">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="88779-2627">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="88779-2628">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="88779-2628">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="88779-2629">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="88779-2629">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2630">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2630">ACS</span></span>

* <span data-ttu-id="88779-2631">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="88779-2631">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="88779-2632">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="88779-2632">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="88779-2633">Advisor</span><span class="sxs-lookup"><span data-stu-id="88779-2633">Advisor</span></span>

* <span data-ttu-id="88779-2634">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="88779-2634">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="88779-2635">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="88779-2635">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="88779-2636">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="88779-2636">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="88779-2637">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="88779-2637">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="88779-2638">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="88779-2638">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2639">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2639">Appservice</span></span>

* <span data-ttu-id="88779-2640">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="88779-2640">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="88779-2641">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-2641">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="88779-2642">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="88779-2642">Eventhubs</span></span>

* <span data-ttu-id="88779-2643">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2643">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2644">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2644">Extension</span></span>

* <span data-ttu-id="88779-2645">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="88779-2645">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2646">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2646">Interactive</span></span>

* <span data-ttu-id="88779-2647">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="88779-2647">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="88779-2648">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="88779-2648">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="88779-2649">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="88779-2649">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="88779-2650">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="88779-2650">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2651">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2651">Monitor</span></span>

* <span data-ttu-id="88779-2652">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="88779-2652">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="88779-2653">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="88779-2653">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="88779-2654">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="88779-2654">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="88779-2655">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="88779-2655">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="88779-2656">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2656">Network</span></span>

* <span data-ttu-id="88779-2657">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="88779-2657">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="88779-2658">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="88779-2658">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="88779-2659">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="88779-2659">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="88779-2660">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="88779-2660">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-2661">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2661">Profile</span></span>

* <span data-ttu-id="88779-2662">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="88779-2662">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="88779-2663">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="88779-2663">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-2664">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-2664">RDBMS</span></span>

* <span data-ttu-id="88779-2665">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="88779-2665">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="88779-2666">Service Bus</span><span class="sxs-lookup"><span data-stu-id="88779-2666">Service Bus</span></span>

* <span data-ttu-id="88779-2667">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2667">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2668">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2668">Storage</span></span>

* <span data-ttu-id="88779-2669">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="88779-2669">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="88779-2670">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="88779-2670">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2671">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2671">VM</span></span>

* <span data-ttu-id="88779-2672">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="88779-2672">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="88779-2673">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="88779-2673">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="88779-2674">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="88779-2674">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="88779-2675">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="88779-2675">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="88779-2676">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2676">February 27, 2018</span></span>

<span data-ttu-id="88779-2677">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="88779-2677">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="88779-2678">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2678">Core</span></span>

* <span data-ttu-id="88779-2679">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="88779-2679">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="88779-2680">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="88779-2680">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="88779-2681">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="88779-2681">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2682">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2682">ACS</span></span>

* <span data-ttu-id="88779-2683">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2683">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="88779-2684">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="88779-2684">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="88779-2685">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="88779-2685">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="88779-2686">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="88779-2686">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2687">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2687">Appservice</span></span>

* <span data-ttu-id="88779-2688">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="88779-2688">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="88779-2689">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="88779-2689">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="88779-2690">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-2690">Cognitive Services</span></span>

* <span data-ttu-id="88779-2691">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-2691">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-2692">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-2692">Consumption</span></span>

* <span data-ttu-id="88779-2693">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="88779-2693">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="88779-2694">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="88779-2694">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="88779-2695">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2695">Container</span></span>

* <span data-ttu-id="88779-2696">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="88779-2696">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="88779-2697">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2697">Network</span></span>

* <span data-ttu-id="88779-2698">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="88779-2698">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2699">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2699">Resource</span></span>

* <span data-ttu-id="88779-2700">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="88779-2700">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="88779-2701">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2701">Role</span></span>

* <span data-ttu-id="88779-2702">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="88779-2702">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2703">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2703">SQL</span></span>

* <span data-ttu-id="88779-2704">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="88779-2704">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2705">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2705">Storage</span></span>

* <span data-ttu-id="88779-2706">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="88779-2706">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2707">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2707">VM</span></span>

* <span data-ttu-id="88779-2708">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="88779-2708">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="88779-2709">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2709">February 13, 2018</span></span>

<span data-ttu-id="88779-2710">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="88779-2710">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="88779-2711">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2711">Core</span></span>

* <span data-ttu-id="88779-2712">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="88779-2712">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2713">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2713">ACS</span></span>

* <span data-ttu-id="88779-2714">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="88779-2714">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="88779-2715">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="88779-2715">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="88779-2716">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-2716">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="88779-2717">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="88779-2717">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="88779-2718">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="88779-2718">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="88779-2719">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="88779-2719">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="88779-2720">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-2720">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="88779-2721">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="88779-2721">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2722">Appservice</span></span>

* <span data-ttu-id="88779-2723">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="88779-2723">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="88779-2724">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="88779-2724">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-2725">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-2725">CDN</span></span>

* <span data-ttu-id="88779-2726">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="88779-2726">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="88779-2727">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2727">Container</span></span>

* <span data-ttu-id="88779-2728">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="88779-2728">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="88779-2729">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2729">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-2730">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-2730">CosmosDB</span></span>

* <span data-ttu-id="88779-2731">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="88779-2731">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2732">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2732">Extension</span></span>

* <span data-ttu-id="88779-2733">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2733">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="88779-2734">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2734">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="88779-2735">Commentaires</span><span class="sxs-lookup"><span data-stu-id="88779-2735">Feedback</span></span>

* <span data-ttu-id="88779-2736">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="88779-2736">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2737">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2737">Interactive</span></span>

* <span data-ttu-id="88779-2738">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="88779-2738">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="88779-2739">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="88779-2739">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="88779-2740">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2740">IoT</span></span>

* <span data-ttu-id="88779-2741">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="88779-2741">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="88779-2742">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="88779-2742">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="88779-2743">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2743">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="88779-2744">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="88779-2744">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2745">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2745">Monitor</span></span>

* <span data-ttu-id="88779-2746">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="88779-2746">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="88779-2747">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2747">Network</span></span>

* <span data-ttu-id="88779-2748">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="88779-2748">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="88779-2749">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2749">Profile</span></span>

* <span data-ttu-id="88779-2750">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="88779-2750">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2751">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2751">Resource</span></span>

* <span data-ttu-id="88779-2752">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="88779-2752">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="88779-2753">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2753">Role</span></span>

* <span data-ttu-id="88779-2754">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="88779-2754">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2755">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2755">SQL</span></span>

* <span data-ttu-id="88779-2756">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="88779-2756">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="88779-2757">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="88779-2757">Added `sql db rename`</span></span>
* <span data-ttu-id="88779-2758">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="88779-2758">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2759">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2759">Storage</span></span>

* <span data-ttu-id="88779-2760">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="88779-2760">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2761">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2761">VM</span></span>

* <span data-ttu-id="88779-2762">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="88779-2762">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="88779-2763">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="88779-2763">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="88779-2764">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="88779-2764">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="88779-2765">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2765">January 31, 2018</span></span>

<span data-ttu-id="88779-2766">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="88779-2766">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="88779-2767">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2767">Core</span></span>

* <span data-ttu-id="88779-2768">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="88779-2768">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="88779-2769">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="88779-2769">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="88779-2770">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="88779-2770">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="88779-2771">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="88779-2771">Use `--verbose` to see</span></span>
* <span data-ttu-id="88779-2772">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="88779-2772">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2773">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2773">ACS</span></span>

* <span data-ttu-id="88779-2774">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="88779-2774">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="88779-2775">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="88779-2775">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2776">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2776">Appservice</span></span>

* <span data-ttu-id="88779-2777">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="88779-2777">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="88779-2778">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="88779-2778">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-2779">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-2779">CDN</span></span>

* <span data-ttu-id="88779-2780">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="88779-2780">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-2781">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-2781">CosmosDB</span></span>

* <span data-ttu-id="88779-2782">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="88779-2782">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2783">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2783">Interactive</span></span>

* <span data-ttu-id="88779-2784">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="88779-2784">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="88779-2785">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2785">Network</span></span>

* <span data-ttu-id="88779-2786">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="88779-2786">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="88779-2787">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2787">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="88779-2788">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="88779-2788">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="88779-2789">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="88779-2789">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="88779-2790">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="88779-2790">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="88779-2791">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="88779-2791">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="88779-2792">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="88779-2792">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="88779-2793">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="88779-2793">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="88779-2794">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="88779-2794">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="88779-2795">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="88779-2795">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="88779-2796">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2796">Profile</span></span>

* <span data-ttu-id="88779-2797">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="88779-2797">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2798">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2798">Resource</span></span>

* <span data-ttu-id="88779-2799">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="88779-2799">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2800">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2800">Storage</span></span>

* <span data-ttu-id="88779-2801">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="88779-2801">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="88779-2802">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="88779-2802">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="88779-2803">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="88779-2803">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="88779-2804">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-2804">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="88779-2805">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="88779-2805">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2806">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2806">VM</span></span>

* <span data-ttu-id="88779-2807">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="88779-2807">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="88779-2808">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="88779-2808">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="88779-2809">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="88779-2809">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="88779-2810">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-2810">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="88779-2811">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="88779-2811">January 17, 2018</span></span>

<span data-ttu-id="88779-2812">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="88779-2812">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2813">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2813">ACR</span></span>

* <span data-ttu-id="88779-2814">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="88779-2814">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="88779-2815">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="88779-2815">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2816">ACS</span></span>

* <span data-ttu-id="88779-2817">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="88779-2817">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="88779-2818">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="88779-2818">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2819">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2819">Appservice</span></span>

* <span data-ttu-id="88779-2820">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="88779-2820">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="88779-2821">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="88779-2821">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="88779-2822">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="88779-2822">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="88779-2823">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-2823">Backup</span></span>

* <span data-ttu-id="88779-2824">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="88779-2824">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="88779-2825">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="88779-2825">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="88779-2826">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="88779-2826">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="88779-2827">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="88779-2827">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="88779-2828">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2828">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2829">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2829">Batch</span></span>

* <span data-ttu-id="88779-2830">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="88779-2830">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="88779-2831">Cloud</span><span class="sxs-lookup"><span data-stu-id="88779-2831">Cloud</span></span>

* <span data-ttu-id="88779-2832">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="88779-2832">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-2833">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-2833">Consumption</span></span>

* <span data-ttu-id="88779-2834">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="88779-2834">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="88779-2835">Event Grid</span><span class="sxs-lookup"><span data-stu-id="88779-2835">Event Grid</span></span>

* <span data-ttu-id="88779-2836">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="88779-2836">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="88779-2837">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="88779-2837">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="88779-2838">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="88779-2838">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="88779-2839">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="88779-2839">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="88779-2840">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="88779-2840">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="88779-2841">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="88779-2841">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="88779-2842">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="88779-2842">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="88779-2843">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="88779-2843">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-2844">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-2844">Interactive</span></span>

* <span data-ttu-id="88779-2845">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="88779-2845">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="88779-2846">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="88779-2846">Fixed errors on startup</span></span>
* <span data-ttu-id="88779-2847">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="88779-2847">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="88779-2848">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2848">IoT</span></span>

* <span data-ttu-id="88779-2849">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="88779-2849">Added support for device provisioning service</span></span>
* <span data-ttu-id="88779-2850">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2850">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="88779-2851">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2851">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2852">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2852">Monitor</span></span>

* <span data-ttu-id="88779-2853">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="88779-2853">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="88779-2854">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="88779-2854">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="88779-2855">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="88779-2855">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="88779-2856">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2856">Network</span></span>

* <span data-ttu-id="88779-2857">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="88779-2857">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="88779-2858">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2858">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-2859">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-2859">Profile</span></span>

* <span data-ttu-id="88779-2860">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="88779-2860">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="88779-2861">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2861">Role</span></span>

* <span data-ttu-id="88779-2862">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="88779-2862">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="88779-2863">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-2863">Service Fabric</span></span>

* <span data-ttu-id="88779-2864">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="88779-2864">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="88779-2865">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="88779-2865">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2866">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2866">VM</span></span>

* <span data-ttu-id="88779-2867">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="88779-2867">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="88779-2868">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="88779-2868">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="88779-2869">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="88779-2869">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="88779-2870">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="88779-2870">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="88779-2871">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="88779-2871">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="88779-2872">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-2872">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="88779-2873">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-2873">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="88779-2874">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="88779-2874">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="88779-2875">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-2875">December 19, 2017</span></span>

<span data-ttu-id="88779-2876">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="88779-2876">Version 2.0.23</span></span>

* <span data-ttu-id="88779-2877">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="88779-2877">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="88779-2878">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2878">Container</span></span>

* <span data-ttu-id="88779-2879">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2879">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="88779-2880">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2880">Network</span></span>

* <span data-ttu-id="88779-2881">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2881">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="88779-2882">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2882">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2883">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2883">Storage</span></span>

* <span data-ttu-id="88779-2884">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="88779-2884">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2885">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2885">VM</span></span>

* <span data-ttu-id="88779-2886">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="88779-2886">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="88779-2887">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-2887">December 5, 2017</span></span>

<span data-ttu-id="88779-2888">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="88779-2888">Version 2.0.22</span></span>

* <span data-ttu-id="88779-2889">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="88779-2889">Removed `az component` commands.</span></span> <span data-ttu-id="88779-2890">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="88779-2890">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="88779-2891">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2891">Core</span></span>
* <span data-ttu-id="88779-2892">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="88779-2892">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="88779-2893">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="88779-2893">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2894">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2894">ACS</span></span>

* <span data-ttu-id="88779-2895">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="88779-2895">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="88779-2896">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="88779-2896">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="88779-2897">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="88779-2897">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="88779-2898">Advisor</span><span class="sxs-lookup"><span data-stu-id="88779-2898">Advisor</span></span>

* <span data-ttu-id="88779-2899">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2899">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2900">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2900">Appservice</span></span>

* <span data-ttu-id="88779-2901">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="88779-2901">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="88779-2902">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="88779-2902">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="88779-2903">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="88779-2903">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="88779-2904">Consommation</span><span class="sxs-lookup"><span data-stu-id="88779-2904">Consumption</span></span>

* <span data-ttu-id="88779-2905">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="88779-2905">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="88779-2906">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2906">Container</span></span>

* <span data-ttu-id="88779-2907">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2907">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2908">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2908">Monitor</span></span>

* <span data-ttu-id="88779-2909">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="88779-2909">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2910">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2910">Resource</span></span>

* <span data-ttu-id="88779-2911">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="88779-2911">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="88779-2912">Role</span><span class="sxs-lookup"><span data-stu-id="88779-2912">Role</span></span>

* <span data-ttu-id="88779-2913">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="88779-2913">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="88779-2914">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="88779-2914">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="88779-2915">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="88779-2915">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2916">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2916">SQL</span></span>

* <span data-ttu-id="88779-2917">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="88779-2917">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="88779-2918">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="88779-2918">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2919">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2919">VM</span></span>

* <span data-ttu-id="88779-2920">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="88779-2920">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="88779-2921">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-2921">November 14, 2017</span></span>

<span data-ttu-id="88779-2922">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="88779-2922">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2923">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2923">ACR</span></span>

* <span data-ttu-id="88779-2924">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="88779-2924">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="88779-2925">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2925">ACS</span></span>

* <span data-ttu-id="88779-2926">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="88779-2926">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="88779-2927">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="88779-2927">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="88779-2928">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="88779-2928">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="88779-2929">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-2929">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="88779-2930">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="88779-2930">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2931">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2931">Appservice</span></span>

* <span data-ttu-id="88779-2932">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="88779-2932">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="88779-2933">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="88779-2933">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="88779-2934">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="88779-2934">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="88779-2935">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="88779-2935">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="88779-2936">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="88779-2936">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="88779-2937">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="88779-2937">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="88779-2938">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-2938">Batch</span></span>

* <span data-ttu-id="88779-2939">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="88779-2939">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-2940">Batchai</span><span class="sxs-lookup"><span data-stu-id="88779-2940">Batchai</span></span>

* <span data-ttu-id="88779-2941">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="88779-2941">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="88779-2942">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="88779-2942">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="88779-2943">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="88779-2943">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="88779-2944">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="88779-2944">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="88779-2945">Cloud</span><span class="sxs-lookup"><span data-stu-id="88779-2945">Cloud</span></span>

* <span data-ttu-id="88779-2946">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="88779-2946">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="88779-2947">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-2947">Container</span></span>

* <span data-ttu-id="88779-2948">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="88779-2948">Added support to open multiple ports</span></span>
* <span data-ttu-id="88779-2949">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="88779-2949">Added container group restart policy</span></span>
* <span data-ttu-id="88779-2950">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="88779-2950">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="88779-2951">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="88779-2951">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="88779-2952">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-2952">Data Lake Analytics</span></span>

* <span data-ttu-id="88779-2953">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="88779-2953">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="88779-2954">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-2954">Data Lake Store</span></span>

* <span data-ttu-id="88779-2955">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="88779-2955">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="88779-2956">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-2956">Extension</span></span>

* <span data-ttu-id="88779-2957">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="88779-2957">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="88779-2958">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="88779-2958">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="88779-2959">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-2959">IoT</span></span>

* <span data-ttu-id="88779-2960">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="88779-2960">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-2961">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-2961">Monitor</span></span>

* <span data-ttu-id="88779-2962">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="88779-2962">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="88779-2963">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-2963">Network</span></span>

* <span data-ttu-id="88779-2964">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="88779-2964">Added support for CAA DNS records</span></span>
* <span data-ttu-id="88779-2965">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="88779-2965">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="88779-2966">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="88779-2966">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="88779-2967">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="88779-2967">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="88779-2968">Réservations</span><span class="sxs-lookup"><span data-stu-id="88779-2968">Reservations</span></span>

* <span data-ttu-id="88779-2969">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="88779-2969">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="88779-2970">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-2970">Resource</span></span>

* <span data-ttu-id="88779-2971">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="88779-2971">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="88779-2972">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-2972">SQL</span></span>

* <span data-ttu-id="88779-2973">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2973">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-2974">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-2974">Storage</span></span>

* <span data-ttu-id="88779-2975">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-2975">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="88779-2976">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="88779-2976">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="88779-2977">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="88779-2977">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="88779-2978">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="88779-2978">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="88779-2979">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="88779-2979">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="88779-2980">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="88779-2980">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="88779-2981">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-2981">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="88779-2982">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-2982">VM</span></span>

* <span data-ttu-id="88779-2983">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="88779-2983">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="88779-2984">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="88779-2984">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="88779-2985">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="88779-2985">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="88779-2986">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="88779-2986">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="88779-2987">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="88779-2987">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="88779-2988">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-2988">October 24, 2017</span></span>

<span data-ttu-id="88779-2989">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="88779-2989">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="88779-2990">Core</span><span class="sxs-lookup"><span data-stu-id="88779-2990">Core</span></span>

* <span data-ttu-id="88779-2991">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="88779-2991">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="88779-2992">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-2992">ACR</span></span>

* <span data-ttu-id="88779-2993">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="88779-2993">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="88779-2994">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="88779-2994">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="88779-2995">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="88779-2995">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="88779-2996">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-2996">ACS</span></span>

* <span data-ttu-id="88779-2997">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="88779-2997">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="88779-2998">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="88779-2998">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-2999">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-2999">Appservice</span></span>

* <span data-ttu-id="88779-3000">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="88779-3000">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="88779-3001">Composant</span><span class="sxs-lookup"><span data-stu-id="88779-3001">Component</span></span>

* <span data-ttu-id="88779-3002">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="88779-3002">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-3003">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-3003">Monitor</span></span>

* <span data-ttu-id="88779-3004">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="88779-3004">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3005">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3005">Resource</span></span>

* <span data-ttu-id="88779-3006">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="88779-3006">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="88779-3007">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="88779-3007">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3008">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3008">VM</span></span>

* <span data-ttu-id="88779-3009">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="88779-3009">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="88779-3010">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3010">October 9, 2017</span></span>

<span data-ttu-id="88779-3011">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="88779-3011">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="88779-3012">Core</span><span class="sxs-lookup"><span data-stu-id="88779-3012">Core</span></span>

* <span data-ttu-id="88779-3013">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="88779-3013">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3014">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3014">Appservice</span></span>

* <span data-ttu-id="88779-3015">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="88779-3015">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="88779-3016">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-3016">Batch</span></span>

* <span data-ttu-id="88779-3017">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-3017">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="88779-3018">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="88779-3018">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="88779-3019">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="88779-3019">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="88779-3020">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="88779-3020">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="88779-3021">Batchai</span><span class="sxs-lookup"><span data-stu-id="88779-3021">Batchai</span></span>

* <span data-ttu-id="88779-3022">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="88779-3022">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-3023">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-3023">Keyvault</span></span>

* <span data-ttu-id="88779-3024">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="88779-3024">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="88779-3025">(#4448)</span><span class="sxs-lookup"><span data-stu-id="88779-3025">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="88779-3026">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3026">Network</span></span>

* <span data-ttu-id="88779-3027">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="88779-3027">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="88779-3028">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="88779-3028">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3029">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3029">Resource</span></span>

* <span data-ttu-id="88779-3030">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="88779-3030">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="88779-3031">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-3031">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="88779-3032">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="88779-3032">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="88779-3033">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="88779-3033">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="88779-3034">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-3034">Sql</span></span>

* <span data-ttu-id="88779-3035">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="88779-3035">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="88779-3036">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="88779-3036">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="88779-3037">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="88779-3037">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3038">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3038">Storage</span></span>

* <span data-ttu-id="88779-3039">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="88779-3039">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3040">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3040">Vm</span></span>

* <span data-ttu-id="88779-3041">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="88779-3041">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="88779-3042">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="88779-3042">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="88779-3043">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="88779-3043">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="88779-3044">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-3044">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="88779-3045">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="88779-3045">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="88779-3046">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3046">September 22, 2017</span></span>

<span data-ttu-id="88779-3047">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="88779-3047">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3048">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3048">Resource</span></span>

* <span data-ttu-id="88779-3049">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="88779-3049">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="88779-3050">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="88779-3050">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="88779-3051">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="88779-3051">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="88779-3052">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="88779-3052">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="88779-3053">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3053">Network</span></span>

* <span data-ttu-id="88779-3054">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="88779-3054">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="88779-3055">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="88779-3055">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="88779-3056">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="88779-3056">Added `asg` application security group commands</span></span>
* <span data-ttu-id="88779-3057">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3057">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="88779-3058">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3058">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="88779-3059">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3059">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="88779-3060">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="88779-3060">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3061">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3061">Storage</span></span>

* <span data-ttu-id="88779-3062">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="88779-3062">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="88779-3063">Événement</span><span class="sxs-lookup"><span data-stu-id="88779-3063">Eventgrid</span></span>

* <span data-ttu-id="88779-3064">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="88779-3064">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="88779-3065">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-3065">SQL</span></span>

* <span data-ttu-id="88779-3066">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="88779-3066">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="88779-3067">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="88779-3067">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="88779-3068">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3068">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-3069">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-3069">Keyvault</span></span>

* <span data-ttu-id="88779-3070">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="88779-3070">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3071">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3071">VM</span></span>

* <span data-ttu-id="88779-3072">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="88779-3072">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="88779-3073">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="88779-3073">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="88779-3074">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="88779-3074">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="88779-3075">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="88779-3075">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="88779-3076">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="88779-3076">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="88779-3077">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="88779-3077">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3078">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3078">ACS</span></span>

* <span data-ttu-id="88779-3079">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="88779-3079">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3080">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3080">Appservice</span></span>

* <span data-ttu-id="88779-3081">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="88779-3081">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="88779-3082">Backup</span><span class="sxs-lookup"><span data-stu-id="88779-3082">Backup</span></span>

* <span data-ttu-id="88779-3083">Préversion</span><span class="sxs-lookup"><span data-stu-id="88779-3083">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="88779-3084">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3084">September 11, 2017</span></span>

<span data-ttu-id="88779-3085">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="88779-3085">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="88779-3086">Core</span><span class="sxs-lookup"><span data-stu-id="88779-3086">Core</span></span>

* <span data-ttu-id="88779-3087">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="88779-3087">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="88779-3088">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="88779-3088">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3089">Acs</span><span class="sxs-lookup"><span data-stu-id="88779-3089">Acs</span></span>

* <span data-ttu-id="88779-3090">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="88779-3090">Added `acs list-locations` command</span></span>
* <span data-ttu-id="88779-3091">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="88779-3091">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3092">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3092">Appservice</span></span>

* <span data-ttu-id="88779-3093">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="88779-3093">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-3094">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-3094">CDN</span></span>

* <span data-ttu-id="88779-3095">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="88779-3095">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="88779-3096">Extension</span><span class="sxs-lookup"><span data-stu-id="88779-3096">Extension</span></span>

* <span data-ttu-id="88779-3097">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-3097">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-3098">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-3098">Keyvault</span></span>

* <span data-ttu-id="88779-3099">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-3099">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="88779-3100">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3100">Network</span></span>

* <span data-ttu-id="88779-3101">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="88779-3101">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="88779-3102">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="88779-3102">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="88779-3103">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="88779-3103">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="88779-3104">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="88779-3104">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="88779-3105">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="88779-3105">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3106">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3106">Resource</span></span>

* <span data-ttu-id="88779-3107">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="88779-3107">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="88779-3108">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="88779-3108">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="88779-3109">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="88779-3109">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="88779-3110">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="88779-3110">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="88779-3111">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-3111">SQL</span></span>

* <span data-ttu-id="88779-3112">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-3112">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3113">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3113">VM</span></span>

* <span data-ttu-id="88779-3114">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="88779-3114">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="88779-3115">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="88779-3115">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="88779-3116">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-3116">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="88779-3117">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="88779-3117">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="88779-3118">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="88779-3118">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="88779-3119">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3119">August 31, 2017</span></span>

<span data-ttu-id="88779-3120">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="88779-3120">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-3121">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-3121">Keyvault</span></span>

* <span data-ttu-id="88779-3122">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="88779-3122">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="88779-3123">Sf</span><span class="sxs-lookup"><span data-stu-id="88779-3123">Sf</span></span>

* <span data-ttu-id="88779-3124">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="88779-3124">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3125">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3125">Storage</span></span>

* <span data-ttu-id="88779-3126">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="88779-3126">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="88779-3127">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="88779-3127">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="88779-3128">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3128">August 28, 2017</span></span>

<span data-ttu-id="88779-3129">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="88779-3129">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="88779-3130">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="88779-3130">CLI</span></span>

* <span data-ttu-id="88779-3131">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="88779-3131">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3132">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3132">ACS</span></span>

* <span data-ttu-id="88779-3133">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="88779-3133">Corrected preview regions</span></span>
* <span data-ttu-id="88779-3134">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="88779-3134">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="88779-3135">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3135">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3136">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3136">Appservice</span></span>

* <span data-ttu-id="88779-3137">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="88779-3137">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="88779-3138">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="88779-3138">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="88779-3139">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="88779-3139">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="88779-3140">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="88779-3140">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="88779-3141">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="88779-3141">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="88779-3142">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-3142">IoT</span></span>

* <span data-ttu-id="88779-3143">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="88779-3143">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="88779-3144">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3144">Network</span></span>

* <span data-ttu-id="88779-3145">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="88779-3145">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="88779-3146">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3146">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="88779-3147">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="88779-3147">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="88779-3148">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="88779-3148">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="88779-3149">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="88779-3149">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-3150">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-3150">Profile</span></span>

* <span data-ttu-id="88779-3151">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3151">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="88779-3152">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-3152">Service Fabric</span></span>

* <span data-ttu-id="88779-3153">Préversion</span><span class="sxs-lookup"><span data-stu-id="88779-3153">Preview release</span></span>
* <span data-ttu-id="88779-3154">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="88779-3154">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="88779-3155">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="88779-3155">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="88779-3156">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="88779-3156">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3157">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3157">Storage</span></span>

* <span data-ttu-id="88779-3158">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="88779-3158">Enabled setting blob tier</span></span>
* <span data-ttu-id="88779-3159">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="88779-3159">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="88779-3160">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="88779-3160">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="88779-3161">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="88779-3161">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="88779-3162">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="88779-3162">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="88779-3163">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="88779-3163">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3164">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3164">VM</span></span>

* <span data-ttu-id="88779-3165">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="88779-3165">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="88779-3166">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="88779-3166">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="88779-3167">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="88779-3167">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="88779-3168">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="88779-3168">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="88779-3169">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="88779-3169">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="88779-3170">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="88779-3170">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="88779-3171">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3171">August 15, 2017</span></span>

<span data-ttu-id="88779-3172">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="88779-3172">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3173">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3173">ACS</span></span>

* <span data-ttu-id="88779-3174">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="88779-3174">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3175">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3175">Appservice</span></span>

* <span data-ttu-id="88779-3176">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="88779-3176">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="88779-3177">Event Grid</span><span class="sxs-lookup"><span data-stu-id="88779-3177">Event Grid</span></span>

* <span data-ttu-id="88779-3178">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="88779-3178">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="88779-3179">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3179">August 11, 2017</span></span>

<span data-ttu-id="88779-3180">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="88779-3180">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3181">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3181">ACS</span></span>

* <span data-ttu-id="88779-3182">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="88779-3182">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="88779-3183">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-3183">Batch</span></span>

* <span data-ttu-id="88779-3184">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="88779-3184">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="88779-3185">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="88779-3185">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="88779-3186">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="88779-3186">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="88779-3187">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="88779-3187">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="88779-3188">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="88779-3188">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="88779-3189">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="88779-3189">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="88779-3190">Composant</span><span class="sxs-lookup"><span data-stu-id="88779-3190">Component</span></span>

* <span data-ttu-id="88779-3191">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="88779-3191">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="88779-3192">Conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-3192">Container</span></span>

* <span data-ttu-id="88779-3193">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="88779-3193">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="88779-3194">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3194">Data Lake Store</span></span>

* <span data-ttu-id="88779-3195">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="88779-3195">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="88779-3196">Event Grid</span><span class="sxs-lookup"><span data-stu-id="88779-3196">Event Grid</span></span>

* <span data-ttu-id="88779-3197">Version initiale</span><span class="sxs-lookup"><span data-stu-id="88779-3197">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="88779-3198">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3198">Network</span></span>

* <span data-ttu-id="88779-3199">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="88779-3199">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="88779-3200">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="88779-3200">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="88779-3201">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="88779-3201">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="88779-3202">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="88779-3202">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="88779-3203">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-3203">Profile</span></span>

* <span data-ttu-id="88779-3204">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="88779-3204">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3205">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3205">Storage</span></span>

* <span data-ttu-id="88779-3206">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="88779-3206">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3207">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3207">VM</span></span>

* <span data-ttu-id="88779-3208">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="88779-3208">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="88779-3209">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="88779-3209">Exposed `list-skus` command</span></span>
* <span data-ttu-id="88779-3210">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="88779-3210">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="88779-3211">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="88779-3211">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="88779-3212">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="88779-3212">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="88779-3213">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3213">July 28, 2017</span></span>

<span data-ttu-id="88779-3214">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="88779-3214">Version 2.0.12</span></span>

* <span data-ttu-id="88779-3215">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="88779-3215">Added container commands</span></span>
* <span data-ttu-id="88779-3216">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="88779-3216">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="88779-3217">Core</span><span class="sxs-lookup"><span data-stu-id="88779-3217">Core</span></span>

* <span data-ttu-id="88779-3218">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="88779-3218">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="88779-3219">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="88779-3219">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="88779-3220">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="88779-3220">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="88779-3221">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="88779-3221">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="88779-3222">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="88779-3222">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="88779-3223">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="88779-3223">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="88779-3224">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="88779-3224">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="88779-3225">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="88779-3225">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="88779-3226">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="88779-3226">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="88779-3227">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="88779-3227">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="88779-3228">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="88779-3228">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="88779-3229">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="88779-3229">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="88779-3230">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="88779-3230">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="88779-3231">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="88779-3231">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="88779-3232">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="88779-3232">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="88779-3233">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="88779-3233">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="88779-3234">ACR</span><span class="sxs-lookup"><span data-stu-id="88779-3234">ACR</span></span>

* <span data-ttu-id="88779-3235">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="88779-3235">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="88779-3236">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="88779-3236">Support SKU update for managed registries</span></span>
* <span data-ttu-id="88779-3237">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="88779-3237">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="88779-3238">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="88779-3238">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="88779-3239">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="88779-3239">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="88779-3240">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="88779-3240">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3241">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3241">ACS</span></span>

* <span data-ttu-id="88779-3242">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="88779-3242">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3243">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3243">Appservice</span></span>

* <span data-ttu-id="88779-3244">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="88779-3244">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="88779-3245">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="88779-3245">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="88779-3246">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="88779-3246">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="88779-3247">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="88779-3247">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="88779-3248">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="88779-3248">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="88779-3249">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="88779-3249">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="88779-3250">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="88779-3250">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="88779-3251">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="88779-3251">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="88779-3252">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="88779-3252">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="88779-3253">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="88779-3253">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="88779-3254">Batch</span><span class="sxs-lookup"><span data-stu-id="88779-3254">Batch</span></span>

* <span data-ttu-id="88779-3255">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="88779-3255">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="88779-3256">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="88779-3256">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="88779-3257">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="88779-3257">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="88779-3258">CDN</span><span class="sxs-lookup"><span data-stu-id="88779-3258">CDN</span></span>

* <span data-ttu-id="88779-3259">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="88779-3259">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="88779-3260">Cloud</span><span class="sxs-lookup"><span data-stu-id="88779-3260">Cloud</span></span>

* <span data-ttu-id="88779-3261">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="88779-3261">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="88779-3262">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="88779-3262">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="88779-3263">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="88779-3263">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="88779-3264">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="88779-3264">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="88779-3265">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="88779-3265">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-3266">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-3266">CosmosDB</span></span>

* <span data-ttu-id="88779-3267">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="88779-3267">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="88779-3268">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="88779-3268">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="88779-3269">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-3269">Data Lake Analytics</span></span>

* <span data-ttu-id="88779-3270">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="88779-3270">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="88779-3271">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="88779-3271">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="88779-3272">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="88779-3272">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="88779-3273">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3273">Data Lake Store</span></span>

* <span data-ttu-id="88779-3274">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="88779-3274">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="88779-3275">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="88779-3275">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="88779-3276">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="88779-3276">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="88779-3277">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3277">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="88779-3278">Interactive</span><span class="sxs-lookup"><span data-stu-id="88779-3278">Interactive</span></span>

* <span data-ttu-id="88779-3279">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="88779-3279">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="88779-3280">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="88779-3280">Increased test coverage</span></span>
* <span data-ttu-id="88779-3281">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="88779-3281">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="88779-3282">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="88779-3282">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="88779-3283">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="88779-3283">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="88779-3284">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="88779-3284">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="88779-3285">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="88779-3285">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="88779-3286">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="88779-3286">Added `--progress` flag</span></span>
* <span data-ttu-id="88779-3287">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="88779-3287">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="88779-3288">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="88779-3288">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="88779-3289">IoT</span><span class="sxs-lookup"><span data-stu-id="88779-3289">IoT</span></span>

* <span data-ttu-id="88779-3290">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="88779-3290">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="88779-3291">(#3934)</span><span class="sxs-lookup"><span data-stu-id="88779-3291">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="88779-3292">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="88779-3292">Key vault</span></span>

* <span data-ttu-id="88779-3293">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="88779-3293">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="88779-3294">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="88779-3294">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="88779-3295">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="88779-3295">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="88779-3296">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="88779-3296">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="88779-3297">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="88779-3297">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="88779-3298">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="88779-3298">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="88779-3299">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="88779-3299">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="88779-3300">(#3307)</span><span class="sxs-lookup"><span data-stu-id="88779-3300">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="88779-3301">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3301">Lab</span></span>

* <span data-ttu-id="88779-3302">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="88779-3302">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="88779-3303">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="88779-3303">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-3304">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-3304">Monitor</span></span>

* <span data-ttu-id="88779-3305">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="88779-3305">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="88779-3306">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="88779-3306">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="88779-3307">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="88779-3307">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="88779-3308">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="88779-3308">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="88779-3309">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="88779-3309">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="88779-3310">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="88779-3310">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="88779-3311">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="88779-3311">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="88779-3312">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="88779-3312">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="88779-3313">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="88779-3313">`location` no longer required</span></span>
  * <span data-ttu-id="88779-3314">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="88779-3314">Add name and ID support for target</span></span>
  * <span data-ttu-id="88779-3315">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="88779-3315">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="88779-3316">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="88779-3316">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="88779-3317">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="88779-3317">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="88779-3318">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="88779-3318">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="88779-3319">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="88779-3319">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="88779-3320">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="88779-3320">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="88779-3321">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3321">Network</span></span>

* <span data-ttu-id="88779-3322">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="88779-3322">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="88779-3323">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="88779-3323">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="88779-3324">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="88779-3324">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="88779-3325">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="88779-3325">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="88779-3326">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="88779-3326">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="88779-3327">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="88779-3327">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="88779-3328">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="88779-3328">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="88779-3329">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="88779-3329">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="88779-3330">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="88779-3330">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="88779-3331">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="88779-3331">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="88779-3332">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="88779-3332">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="88779-3333">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="88779-3333">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="88779-3334">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="88779-3334">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="88779-3335">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="88779-3335">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="88779-3336">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="88779-3336">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="88779-3337">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="88779-3337">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="88779-3338">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="88779-3338">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="88779-3339">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="88779-3339">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="88779-3340">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="88779-3340">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="88779-3341">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="88779-3341">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="88779-3342">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="88779-3342">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="88779-3343">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-3343">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="88779-3344">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="88779-3344">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="88779-3345">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="88779-3345">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="88779-3346">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="88779-3346">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="88779-3347">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="88779-3347">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="88779-3348">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="88779-3348">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="88779-3349">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-3349">Profile</span></span>

* <span data-ttu-id="88779-3350">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="88779-3350">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="88779-3351">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="88779-3351">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="88779-3352">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="88779-3352">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="88779-3353">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="88779-3353">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="88779-3354">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="88779-3354">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="88779-3355">SGBDR</span><span class="sxs-lookup"><span data-stu-id="88779-3355">RDBMS</span></span>

* <span data-ttu-id="88779-3356">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="88779-3356">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="88779-3357">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="88779-3357">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="88779-3358">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="88779-3358">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="88779-3359">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="88779-3359">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3360">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3360">Resource</span></span>

* <span data-ttu-id="88779-3361">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="88779-3361">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="88779-3362">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="88779-3362">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="88779-3363">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="88779-3363">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="88779-3364">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="88779-3364">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="88779-3365">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="88779-3365">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="88779-3366">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="88779-3366">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="88779-3367">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="88779-3367">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="88779-3368">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="88779-3368">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="88779-3369">Role</span><span class="sxs-lookup"><span data-stu-id="88779-3369">Role</span></span>

* <span data-ttu-id="88779-3370">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="88779-3370">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="88779-3371">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="88779-3371">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="88779-3372">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="88779-3372">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="88779-3373">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="88779-3373">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="88779-3374">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="88779-3374">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="88779-3375">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-3375">Service Fabric</span></span>
* <span data-ttu-id="88779-3376">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="88779-3376">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="88779-3377">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="88779-3377">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="88779-3378">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="88779-3378">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="88779-3379">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-3379">SQL</span></span>

* <span data-ttu-id="88779-3380">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="88779-3380">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="88779-3381">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="88779-3381">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="88779-3382">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="88779-3382">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3383">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3383">Storage</span></span>

* <span data-ttu-id="88779-3384">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="88779-3384">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="88779-3385">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="88779-3385">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="88779-3386">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="88779-3386">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="88779-3387">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="88779-3387">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="88779-3388">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="88779-3388">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="88779-3389">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="88779-3389">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3390">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3390">VM</span></span>

* <span data-ttu-id="88779-3391">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3391">Support configuring nsg</span></span>
* <span data-ttu-id="88779-3392">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="88779-3392">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="88779-3393">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="88779-3393">Support managed service identities</span></span>
* <span data-ttu-id="88779-3394">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="88779-3394">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="88779-3395">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="88779-3395">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="88779-3396">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3396">May 10, 2017</span></span>

<span data-ttu-id="88779-3397">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="88779-3397">Version 2.0.6</span></span>

* <span data-ttu-id="88779-3398">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="88779-3398">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="88779-3399">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="88779-3399">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="88779-3400">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3400">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="88779-3401">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="88779-3401">Include Cognitive Services module</span></span>
* <span data-ttu-id="88779-3402">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="88779-3402">Include Service Fabric module</span></span>
* <span data-ttu-id="88779-3403">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="88779-3403">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="88779-3404">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="88779-3404">Add support for CDN commands</span></span>
* <span data-ttu-id="88779-3405">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="88779-3405">Remove Container module</span></span>
* <span data-ttu-id="88779-3406">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="88779-3406">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="88779-3407">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="88779-3407">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="88779-3408">Core</span><span class="sxs-lookup"><span data-stu-id="88779-3408">Core</span></span>

* <span data-ttu-id="88779-3409">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="88779-3409">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="88779-3410">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="88779-3410">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="88779-3411">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="88779-3411">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="88779-3412">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="88779-3412">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="88779-3413">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="88779-3413">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="88779-3414">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="88779-3414">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="88779-3415">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="88779-3415">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="88779-3416">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="88779-3416">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="88779-3417">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="88779-3417">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="88779-3418">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="88779-3418">core: Improved performance</span></span>
* <span data-ttu-id="88779-3419">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="88779-3419">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="88779-3420">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="88779-3420">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3421">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3421">ACS</span></span>

* <span data-ttu-id="88779-3422">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="88779-3422">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="88779-3423">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="88779-3423">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="88779-3424">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="88779-3424">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="88779-3425">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="88779-3425">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3426">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3426">AppService</span></span>

* <span data-ttu-id="88779-3427">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="88779-3427">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="88779-3428">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="88779-3428">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="88779-3429">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="88779-3429">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="88779-3430">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="88779-3430">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="88779-3431">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="88779-3431">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="88779-3432">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="88779-3432">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="88779-3433">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="88779-3433">support slot swap with preview</span></span>
* <span data-ttu-id="88779-3434">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="88779-3434">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="88779-3435">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="88779-3435">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="88779-3436">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="88779-3436">CosmosDB</span></span>

* <span data-ttu-id="88779-3437">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="88779-3437">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="88779-3438">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="88779-3438">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="88779-3439">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="88779-3439">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="88779-3440">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="88779-3440">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="88779-3441">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-3441">Data Lake Analytics</span></span>

* <span data-ttu-id="88779-3442">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="88779-3442">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="88779-3443">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="88779-3443">Add support for new catalog item type: package.</span></span> <span data-ttu-id="88779-3444">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="88779-3444">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="88779-3445">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="88779-3445">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="88779-3446">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="88779-3446">Table</span></span>
  * <span data-ttu-id="88779-3447">Fonction table</span><span class="sxs-lookup"><span data-stu-id="88779-3447">Table valued function</span></span>
  * <span data-ttu-id="88779-3448">Affichage</span><span class="sxs-lookup"><span data-stu-id="88779-3448">View</span></span>
  * <span data-ttu-id="88779-3449">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="88779-3449">Table Statistics.</span></span> <span data-ttu-id="88779-3450">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="88779-3450">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="88779-3451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3451">Data Lake Store</span></span>

* <span data-ttu-id="88779-3452">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="88779-3452">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="88779-3453">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="88779-3453">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="88779-3454">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="88779-3454">missed help for access show.</span></span> <span data-ttu-id="88779-3455">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="88779-3455">adding it.</span></span> <span data-ttu-id="88779-3456">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="88779-3456">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="88779-3457">Rechercher</span><span class="sxs-lookup"><span data-stu-id="88779-3457">Find</span></span>

* <span data-ttu-id="88779-3458">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="88779-3458">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="88779-3459">KeyVault</span><span class="sxs-lookup"><span data-stu-id="88779-3459">KeyVault</span></span>

* <span data-ttu-id="88779-3460">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="88779-3460">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="88779-3461">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="88779-3461">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="88779-3462">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="88779-3462">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="88779-3463">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="88779-3463">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="88779-3464">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="88779-3464">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="88779-3465">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3465">Lab</span></span>

* <span data-ttu-id="88779-3466">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3466">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="88779-3467">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3467">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="88779-3468">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3468">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="88779-3469">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3469">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="88779-3470">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="88779-3470">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="88779-3471">Superviser</span><span class="sxs-lookup"><span data-stu-id="88779-3471">Monitor</span></span>

* <span data-ttu-id="88779-3472">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="88779-3472">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="88779-3473">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="88779-3473">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="88779-3474">Réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3474">Network</span></span>

* <span data-ttu-id="88779-3475">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="88779-3475">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="88779-3476">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="88779-3476">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="88779-3477">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="88779-3477">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="88779-3478">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="88779-3478">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="88779-3479">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="88779-3479">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="88779-3480">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="88779-3480">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="88779-3481">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="88779-3481">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="88779-3482">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="88779-3482">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="88779-3483">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="88779-3483">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="88779-3484">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="88779-3484">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="88779-3485">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="88779-3485">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="88779-3486">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="88779-3486">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="88779-3487">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="88779-3487">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="88779-3488">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="88779-3488">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="88779-3489">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="88779-3489">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="88779-3490">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="88779-3490">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="88779-3491">Profil</span><span class="sxs-lookup"><span data-stu-id="88779-3491">Profile</span></span>

* <span data-ttu-id="88779-3492">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="88779-3492">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="88779-3493">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="88779-3493">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="88779-3494">Redis</span><span class="sxs-lookup"><span data-stu-id="88779-3494">Redis</span></span>

* <span data-ttu-id="88779-3495">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="88779-3495">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="88779-3496">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="88779-3496">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="88779-3497">Ressource</span><span class="sxs-lookup"><span data-stu-id="88779-3497">Resource</span></span>

* <span data-ttu-id="88779-3498">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="88779-3498">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="88779-3499">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="88779-3499">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="88779-3500">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="88779-3500">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="88779-3501">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="88779-3501">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="88779-3502">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="88779-3502">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="88779-3503">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="88779-3503">Add docs for az lock update.</span></span> <span data-ttu-id="88779-3504">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="88779-3504">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="88779-3505">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="88779-3505">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="88779-3506">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="88779-3506">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="88779-3507">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="88779-3507">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="88779-3508">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="88779-3508">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="88779-3509">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="88779-3509">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="88779-3510">Role</span><span class="sxs-lookup"><span data-stu-id="88779-3510">Role</span></span>

* <span data-ttu-id="88779-3511">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="88779-3511">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="88779-3512">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="88779-3512">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="88779-3513">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="88779-3513">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="88779-3514">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="88779-3514">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="88779-3515">SQL</span><span class="sxs-lookup"><span data-stu-id="88779-3515">SQL</span></span>

* <span data-ttu-id="88779-3516">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="88779-3516">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="88779-3517">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="88779-3517">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="88779-3518">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3518">Storage</span></span>

* <span data-ttu-id="88779-3519">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="88779-3519">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="88779-3520">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="88779-3520">Add support for incremental blob copy</span></span>
* <span data-ttu-id="88779-3521">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="88779-3521">Add support for large block blob upload</span></span>
* <span data-ttu-id="88779-3522">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="88779-3522">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3523">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3523">VM</span></span>

* <span data-ttu-id="88779-3524">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="88779-3524">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="88779-3525">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="88779-3525">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="88779-3526">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="88779-3526">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="88779-3527">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="88779-3527">az vm/vmss disk</span></span>
  3. <span data-ttu-id="88779-3528">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="88779-3528">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="88779-3529">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="88779-3529">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="88779-3530">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="88779-3530">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="88779-3531">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3531">April 3, 2017</span></span>

<span data-ttu-id="88779-3532">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="88779-3532">Version 2.0.2</span></span>

<span data-ttu-id="88779-3533">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="88779-3533">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="88779-3534">Core</span><span class="sxs-lookup"><span data-stu-id="88779-3534">Core</span></span>

* <span data-ttu-id="88779-3535">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-3535">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="88779-3536">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="88779-3536">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="88779-3537">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="88779-3537">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="88779-3538">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="88779-3538">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="88779-3539">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="88779-3539">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="88779-3540">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="88779-3540">Add prompting for missing template parameters.</span></span> <span data-ttu-id="88779-3541">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="88779-3541">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="88779-3542">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="88779-3542">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="88779-3543">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="88779-3543">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="88779-3544">ACS</span><span class="sxs-lookup"><span data-stu-id="88779-3544">ACS</span></span>

* <span data-ttu-id="88779-3545">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="88779-3545">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="88779-3546">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="88779-3546">Add support for ssh key password prompting.</span></span> <span data-ttu-id="88779-3547">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="88779-3547">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="88779-3548">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="88779-3548">Add support for windows clusters.</span></span> <span data-ttu-id="88779-3549">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="88779-3549">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="88779-3550">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="88779-3550">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="88779-3551">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="88779-3551">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="88779-3552">AppService</span><span class="sxs-lookup"><span data-stu-id="88779-3552">AppService</span></span>

* <span data-ttu-id="88779-3553">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="88779-3553">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="88779-3554">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="88779-3554">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="88779-3555">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="88779-3555">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="88779-3556">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="88779-3556">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="88779-3557">DataLake</span><span class="sxs-lookup"><span data-stu-id="88779-3557">DataLake</span></span>

* <span data-ttu-id="88779-3558">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="88779-3558">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="88779-3559">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="88779-3559">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="88779-3560">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="88779-3560">DocuemntDB</span></span>

* <span data-ttu-id="88779-3561">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="88779-3561">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="88779-3562">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="88779-3562">VM</span></span>

* <span data-ttu-id="88779-3563">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="88779-3563">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="88779-3564">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="88779-3564">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="88779-3565">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="88779-3565">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="88779-3566">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="88779-3566">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="88779-3567">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="88779-3567">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="88779-3568">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="88779-3568">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="88779-3569">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="88779-3569">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="88779-3570">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="88779-3570">February 27, 2017</span></span>

<span data-ttu-id="88779-3571">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="88779-3571">Version 2.0.0</span></span>

<span data-ttu-id="88779-3572">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="88779-3572">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="88779-3573">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="88779-3573">Container Service (acs)</span></span>
- <span data-ttu-id="88779-3574">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="88779-3574">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="88779-3575">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="88779-3575">Networking</span></span>
- <span data-ttu-id="88779-3576">Stockage</span><span class="sxs-lookup"><span data-stu-id="88779-3576">Storage</span></span>

<span data-ttu-id="88779-3577">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="88779-3577">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="88779-3578">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="88779-3578">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="88779-3579">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="88779-3579">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="88779-3580">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="88779-3580">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="88779-3581">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="88779-3581">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="88779-3582">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="88779-3582">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="88779-3583">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="88779-3583">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="88779-3584">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="88779-3584">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="88779-3585">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="88779-3585">Provide feedback from the command line with the `az feedback` command</span></span>
