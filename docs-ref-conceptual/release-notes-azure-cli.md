---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/19/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c95a635cc58afcc7956c230d0e3f47351fa0893d
ms.sourcegitcommit: d05660a42b2a77c4b05a7f96c386e656bd2db0fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2020
ms.locfileid: "83569185"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="a6136-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a6136-103">Azure CLI release notes</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="a6136-104">19 mai 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-104">May 19, 2020</span></span>

<span data-ttu-id="a6136-105">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="a6136-105">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-106">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-106">ACR</span></span>

* <span data-ttu-id="a6136-107">Ajout du délai d’expiration par défaut de 5 minutes pour toute demande à ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-107">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="a6136-108">Prise en charge de la désactivation de l’accès au réseau public</span><span class="sxs-lookup"><span data-stu-id="a6136-108">Support disable public network access</span></span>
* <span data-ttu-id="a6136-109">`az acr token create` : exposition de l’argument --days</span><span class="sxs-lookup"><span data-stu-id="a6136-109">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="a6136-110">`az acr import` : acceptation des valeurs de l’argument --source qui contiennent le nom du serveur de connexion résultant d’une correction côté du client</span><span class="sxs-lookup"><span data-stu-id="a6136-110">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-111">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-111">ACS</span></span>

* <span data-ttu-id="a6136-112">Correctif de bogue : suppression du nettoyage des champs pour les champs qui n’existent plus</span><span class="sxs-lookup"><span data-stu-id="a6136-112">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-113">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-113">AKS</span></span>

* <span data-ttu-id="a6136-114">Mise à jour du contexte de l’aide pour la commande uptime-sla</span><span class="sxs-lookup"><span data-stu-id="a6136-114">Update uptime-sla command help context</span></span>
* <span data-ttu-id="a6136-115">Suppression de la vérification de plage pour la mise à jour du nombre minimal pour l’autoscaler</span><span class="sxs-lookup"><span data-stu-id="a6136-115">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="a6136-116">Correction de l’interface CLI qui n’échoue pas quand l’utilisateur spécifie uniquement un mot de passe Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-116">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-117">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-117">AMS</span></span>

* <span data-ttu-id="a6136-118">`az ams transform create`: Ajout de la possibilité de créer une transformation avec une présélection FaceDetector</span><span class="sxs-lookup"><span data-stu-id="a6136-118">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="a6136-119">`az ams content-key-policy create` : Ajout de la possibilité de créer une stratégie de clé de contenu FairPlay avec une configuration de location hors connexion</span><span class="sxs-lookup"><span data-stu-id="a6136-119">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-120">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-120">AppConfig</span></span>

* <span data-ttu-id="a6136-121">Correction de bogue pour les valeurs de clé de liste avec champs</span><span class="sxs-lookup"><span data-stu-id="a6136-121">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-122">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-122">AppService</span></span>

* <span data-ttu-id="a6136-123">`az functionapp create`: AzureWebJobsDashboard ne sera défini que si AppInsights est désactivé</span><span class="sxs-lookup"><span data-stu-id="a6136-123">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="a6136-124">Correctif #10664 – Intégration de réseau virtuel – Problème de vérification d’emplacement et correctif #13257 – Échec d’az webapp up quand un groupe de ressources doit être créé</span><span class="sxs-lookup"><span data-stu-id="a6136-124">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="a6136-125">`az webapp|functionapp config ssl import`: Recherche dans le coffre de clés des groupes de ressources d’un abonnement et amélioration de l’aide et des exemples.</span><span class="sxs-lookup"><span data-stu-id="a6136-125">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="a6136-126">Intégration du contexte local pour App Service</span><span class="sxs-lookup"><span data-stu-id="a6136-126">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-127">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-127">ARM</span></span>

* <span data-ttu-id="a6136-128">`az deployment`: Correction du problème lié à l’absence de retour de templateLink pendant le déploiement ou la validation de template-uri</span><span class="sxs-lookup"><span data-stu-id="a6136-128">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="a6136-129">`az deployment`: Correction du problème lié au fait que les caractères spécialement encodés ne sont pas pris en charge par le déploiement/la validation</span><span class="sxs-lookup"><span data-stu-id="a6136-129">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="a6136-130">`az deployment sub/group what-if`: Correction de l’alignement de tableau et gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a6136-130">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="a6136-131">`az deployment operation`: Modification des informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="a6136-131">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="a6136-132">ARO</span><span class="sxs-lookup"><span data-stu-id="a6136-132">ARO</span></span>

* <span data-ttu-id="a6136-133">Ajout d’exemples pour az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="a6136-133">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="a6136-134">Ajout de la fonction generate_random_id</span><span class="sxs-lookup"><span data-stu-id="a6136-134">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-135">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-135">Backup</span></span>

* <span data-ttu-id="a6136-136">Autorisation de FriendlyName dans la commande d’activation de la protection pour AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="a6136-136">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="a6136-137">Correction dans la commande IaasVM restore-disks</span><span class="sxs-lookup"><span data-stu-id="a6136-137">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="a6136-138">Ajout de BackupManagementType « MAB » à la commande item list</span><span class="sxs-lookup"><span data-stu-id="a6136-138">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="a6136-139">Ajout de la prise en charge des nouvelles tentatives de mise à jour de stratégie pour les éléments en échec.</span><span class="sxs-lookup"><span data-stu-id="a6136-139">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="a6136-140">Ajout d’une fonctionnalité de reprise de protection pour Machine Virtuelle Azure</span><span class="sxs-lookup"><span data-stu-id="a6136-140">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="a6136-141">Ajout d’une prise en charge permettant de spécifier ResourceGroup pour stocker instantRP pendant la création ou la modification d’une stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-141">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="a6136-142">CI</span><span class="sxs-lookup"><span data-stu-id="a6136-142">CI</span></span>

* <span data-ttu-id="a6136-143">Prise en charge de flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="a6136-143">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-144">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-144">Compute</span></span>

* <span data-ttu-id="a6136-145">Nouvelle commande az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="a6136-145">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="a6136-146">`az vm list-skus`: Mise à jour du comportement de --zone ; retourne désormais tous les types de références SKU</span><span class="sxs-lookup"><span data-stu-id="a6136-146">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="a6136-147">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-147">Core</span></span>

* <span data-ttu-id="a6136-148">Mise à jour de l’état activé/désactivé du contexte local vers le niveau utilisateur global</span><span class="sxs-lookup"><span data-stu-id="a6136-148">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-149">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-149">Extension</span></span>

* <span data-ttu-id="a6136-150">`az extension add`: Ajout de --system pour permettre l’installation d’extensions dans un chemin système</span><span class="sxs-lookup"><span data-stu-id="a6136-150">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="a6136-151">Prise en charge de .egg-info pour stocker les métadonnées d’extension de type wheel</span><span class="sxs-lookup"><span data-stu-id="a6136-151">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-152">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-152">IoT</span></span>

* <span data-ttu-id="a6136-153">`az iot`: Mise à jour du message de reconnaissance de la première extension exécutée par le module de commande IoT vers l’ID moderne non déconseillé `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="a6136-153">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="a6136-154">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="a6136-154">IoT Hub</span></span>

* <span data-ttu-id="a6136-155">Prise en charge des commandes de l’API 2020-03-01 et de l’isolement réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-155">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="a6136-156">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="a6136-156">NetAppFiles</span></span>

* <span data-ttu-id="a6136-157">`az volume create`: Ajout de snapshot-id en tant que paramètre pour créer un volume, permettant ainsi aux utilisateurs de créer un volume à partir d’une capture instantanée existante.</span><span class="sxs-lookup"><span data-stu-id="a6136-157">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="a6136-158">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-158">Network</span></span>

* <span data-ttu-id="a6136-159">Correction du changement non souhaité de la valeur TTL pour dns add-record</span><span class="sxs-lookup"><span data-stu-id="a6136-159">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="a6136-160">`az network public-ip create`: Information à l’intention des clients pour les prévenir d’un changement cassant imminent</span><span class="sxs-lookup"><span data-stu-id="a6136-160">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="a6136-161">Prise en charge des commandes génériques pour un scénario de liaison privée</span><span class="sxs-lookup"><span data-stu-id="a6136-161">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="a6136-162">`az network private-endpoint-connection`: Prise en charge des types mysql, postgre et mariadb</span><span class="sxs-lookup"><span data-stu-id="a6136-162">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="a6136-163">`az network private-endpoint-connection`: Prise en charge des types cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a6136-163">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="a6136-164">`az network private-endpoint` : dépréciation de --group-ids et redirection vers --group-id</span><span class="sxs-lookup"><span data-stu-id="a6136-164">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="a6136-165">Output</span><span class="sxs-lookup"><span data-stu-id="a6136-165">Output</span></span>

* <span data-ttu-id="a6136-166">Affichage de l’instruction update dans find, feedback et --help</span><span class="sxs-lookup"><span data-stu-id="a6136-166">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-167">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-167">Packaging</span></span>

* <span data-ttu-id="a6136-168">Génération de packages MSI/Homebrew avec les dépendances résolues selon requirements.txt</span><span class="sxs-lookup"><span data-stu-id="a6136-168">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-169">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-169">RBAC</span></span>

* <span data-ttu-id="a6136-170">`az ad sp credential reset` : correction de la génération d’informations d’identification faibles</span><span class="sxs-lookup"><span data-stu-id="a6136-170">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-171">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-171">Storage</span></span>

* <span data-ttu-id="a6136-172">`az storage account file-service-properties update/show`: Ajout de la prise en charge des propriétés de fichier pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-172">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="a6136-173">`az storage container create`: Correction #13373 par l’ajout d’un validateur pour l’accès public</span><span class="sxs-lookup"><span data-stu-id="a6136-173">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="a6136-174">Ajout de la prise en charge d’ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="a6136-174">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="a6136-175">`az storage blob sync`: Prise en charge d’`--connection-string`</span><span class="sxs-lookup"><span data-stu-id="a6136-175">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="a6136-176">`az storage blob sync`: Correction du message d’erreur incorrect quand azcopy ne trouve pas l’emplacement d’installation</span><span class="sxs-lookup"><span data-stu-id="a6136-176">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="a6136-177">30 avril 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-177">April 30, 2020</span></span>

<span data-ttu-id="a6136-178">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="a6136-178">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-179">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-179">ACR</span></span>

* <span data-ttu-id="a6136-180">`az acr check-health`: Correction de « DOCKER_PULL_ERROR » sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-180">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-181">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-181">Compute</span></span>

* <span data-ttu-id="a6136-182">`az vm list-ip-addresses`: Gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a6136-182">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="a6136-183">Correction d’un bogue de vm create si endpoint_vm_image_alias_doc n’est pas défini dans le profil cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-183">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="a6136-184">`az vmss create`: Ajout de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="a6136-184">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-185">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-185">Cosmos DB</span></span>

* <span data-ttu-id="a6136-186">`az cosmosdb create/update` : ajout de la prise en charge de add --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="a6136-186">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-187">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-187">Extension</span></span>

* <span data-ttu-id="a6136-188">Correction du chargement des métadonnées incorrectes pour l’extension du type de roulette</span><span class="sxs-lookup"><span data-stu-id="a6136-188">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-189">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-189">Packaging</span></span>

* <span data-ttu-id="a6136-190">Ajout du script az pour Git Bash/Cygwin sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-190">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-191">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-191">SQL</span></span>

* <span data-ttu-id="a6136-192">`az sql instance-pool`: Ajout d’un groupe de commandes pour les pools d’instances</span><span class="sxs-lookup"><span data-stu-id="a6136-192">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-193">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-193">Storage</span></span>

* <span data-ttu-id="a6136-194">Mise à niveau du package azure-multiapi-storage vers 0.3.0</span><span class="sxs-lookup"><span data-stu-id="a6136-194">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="a6136-195">Prise en charge de GZRS pour la création et la mise à jour de comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-195">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="a6136-196">`az storage account failover`: Ajout de la prise en charge du basculement de comptes de stockage grs/gzrs</span><span class="sxs-lookup"><span data-stu-id="a6136-196">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="a6136-197">`az storage blob upload`: Ajout du paramètre --encryption-scope pour prendre en charge la spécification des informations d’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="a6136-197">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="a6136-198">28 avril 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-198">April 28, 2020</span></span>

<span data-ttu-id="a6136-199">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="a6136-199">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-200">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-200">ACS</span></span>

* <span data-ttu-id="a6136-201">[CHANGEMENT CASSANT] du paramètre az openshift create: remove --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="a6136-201">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="a6136-202">`az openshift create` : Ajout d’indicateurs pour prendre en charge un cluster privé.</span><span class="sxs-lookup"><span data-stu-id="a6136-202">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="a6136-203">`az openshift` : Mise à niveau vers la version d’API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="a6136-203">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="a6136-204">`az openshift` : Ajout de la commande `update`.</span><span class="sxs-lookup"><span data-stu-id="a6136-204">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-205">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-205">AKS</span></span>

* <span data-ttu-id="a6136-206">`az aks create`: Ajout de la prise en charge de Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-206">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-207">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-207">AppService</span></span>

* <span data-ttu-id="a6136-208">`az webapp deployment source config-zip` : Suppression de sleep après request.get()</span><span class="sxs-lookup"><span data-stu-id="a6136-208">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-209">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-209">ARM</span></span>

* <span data-ttu-id="a6136-210">Ajout de commandes What-If de déploiement de modèles</span><span class="sxs-lookup"><span data-stu-id="a6136-210">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="a6136-211">ARO</span><span class="sxs-lookup"><span data-stu-id="a6136-211">ARO</span></span>

* <span data-ttu-id="a6136-212">`az aro`: Correction de la sortie de table</span><span class="sxs-lookup"><span data-stu-id="a6136-212">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="a6136-213">CI</span><span class="sxs-lookup"><span data-stu-id="a6136-213">CI</span></span>

* <span data-ttu-id="a6136-214">Intégration de pytest et dépréciation de nose pour le test d’automatisation</span><span class="sxs-lookup"><span data-stu-id="a6136-214">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-215">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-215">Compute</span></span>

* <span data-ttu-id="a6136-216">`az vmss disk detach` : Correction du problème NoneType du disque de données</span><span class="sxs-lookup"><span data-stu-id="a6136-216">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="a6136-217">`az vm availability-set list`: Prise en charge de l’affichage de la liste de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="a6136-217">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="a6136-218">`az vm list-skus`: Correction du problème d’affichage du format de table</span><span class="sxs-lookup"><span data-stu-id="a6136-218">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-219">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-219">KeyVault</span></span>

* <span data-ttu-id="a6136-220">Ajout d’un nouveau paramètre `--enable-rbac-authorization` lors de la création ou de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-220">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-221">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-221">Monitor</span></span>

* <span data-ttu-id="a6136-222">Prise en charge des fonctionnalités CMK de cluster LA</span><span class="sxs-lookup"><span data-stu-id="a6136-222">Support LA cluster CMK features</span></span>
* <span data-ttu-id="a6136-223">`az monitor log-analytics workspace linked-storage` : Prise en charge des fonctionnalités BYOS</span><span class="sxs-lookup"><span data-stu-id="a6136-223">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="a6136-224">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-224">Network</span></span>

* <span data-ttu-id="a6136-225">`az network security-partner` : Prise en charge du fournisseur de partenaire de sécurité</span><span class="sxs-lookup"><span data-stu-id="a6136-225">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="a6136-226">Privatedns</span><span class="sxs-lookup"><span data-stu-id="a6136-226">Privatedns</span></span>

* <span data-ttu-id="a6136-227">Ajout d’une fonctionnalité dans une zone DNS privée pour importer/exporter un fichier de zone</span><span class="sxs-lookup"><span data-stu-id="a6136-227">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="a6136-228">21 avril 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-228">April 21, 2020</span></span>

<span data-ttu-id="a6136-229">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="a6136-229">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-230">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-230">ACR</span></span>

* <span data-ttu-id="a6136-231">`az acr run --cmd` : désactivation du remplacement du répertoire de travail</span><span class="sxs-lookup"><span data-stu-id="a6136-231">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="a6136-232">Prise en charge du point de terminaison de données dédié</span><span class="sxs-lookup"><span data-stu-id="a6136-232">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-233">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-233">AKS</span></span>

* <span data-ttu-id="a6136-234">`az aks list -o table` doit afficher privateFqdn comme nom de domaine complet pour les clusters privés</span><span class="sxs-lookup"><span data-stu-id="a6136-234">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="a6136-235">Ajout de --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="a6136-235">Add --uptime-sla</span></span>
* <span data-ttu-id="a6136-236">Mise à jour du package containerservice</span><span class="sxs-lookup"><span data-stu-id="a6136-236">Update containerservice package</span></span>
* <span data-ttu-id="a6136-237">Ajout de la prise en charge de l’adresse IP publique de nœud</span><span class="sxs-lookup"><span data-stu-id="a6136-237">Add node public IP support</span></span>
* <span data-ttu-id="a6136-238">Correction d’une faute de frappe dans la commande d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-238">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-239">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-239">AppConfig</span></span>

* <span data-ttu-id="a6136-240">Résolution de la référence du coffre de clés pour la liste Key Vault et les commandes d’exportation</span><span class="sxs-lookup"><span data-stu-id="a6136-240">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="a6136-241">Résolution de bogue pour les valeurs de clé de liste</span><span class="sxs-lookup"><span data-stu-id="a6136-241">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-242">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-242">AppService</span></span>

* <span data-ttu-id="a6136-243">`az functionapp create`: Modification de la façon dont linuxFxVersion était défini pour les applications de fonction dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="a6136-243">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="a6136-244">Cela doit résoudre un bogue qui empêchait la création d’applications de consommation dotnet linux</span><span class="sxs-lookup"><span data-stu-id="a6136-244">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="a6136-245">[CHANGEMENT CASSANT] `az webapp create` : correctif pour conserver les paramètres d’application existants avec az webapp create</span><span class="sxs-lookup"><span data-stu-id="a6136-245">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="a6136-246">[CHANGEMENT CASSANT] `az webapp up` : correctif pour créer un groupe de ressources pour la commande az webapp up lors de l’utilisation de l’indicateur -g</span><span class="sxs-lookup"><span data-stu-id="a6136-246">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="a6136-247">[CHANGEMENT CASSANT] `az webapp config` : correctif pour afficher des valeurs pour la sortie non-JSON avec la liste de chaînes de connexion az webapp config</span><span class="sxs-lookup"><span data-stu-id="a6136-247">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-248">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-248">ARM</span></span>

* <span data-ttu-id="a6136-249">`az deployment create/validate`: Ajout d’un paramètre `--no-prompt` pour prendre en charge le saut de l’invite de paramètres manquants pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-249">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="a6136-250">`az deployment group/mg/sub/tenant validate`: Prise en charge de commentaires dans le fichier de paramètres de déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-250">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="a6136-251">`az deployment`: Suppression de `is_preview` pour le paramètre `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="a6136-251">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="a6136-252">`az deployment group/mg/sub/tenant cancel`: Prise en charge de l’annulation du déploiement pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-252">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="a6136-253">`az deployment group/mg/sub/tenant validate`: Amélioration du message d’erreur lors de l’échec de la vérification du déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-253">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="a6136-254">`az deployment-scripts`: Ajout de nouvelles commandes pour DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="a6136-254">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="a6136-255">`az resource tag`: Ajout du paramètre `--is-incremental` pour prendre en charge l’ajout incrémentiel de balises aux ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-255">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="a6136-256">ARO</span><span class="sxs-lookup"><span data-stu-id="a6136-256">ARO</span></span>

* <span data-ttu-id="a6136-257">`az aro`:  Ajout du module de commande aro Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="a6136-257">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-258">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-258">Batch</span></span>

* <span data-ttu-id="a6136-259">Mise à jour de l’API Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-259">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-260">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-260">Compute</span></span>

* <span data-ttu-id="a6136-261">`az sig image-version create`: Ajout d’un type de compte de stockage Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="a6136-261">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="a6136-262">`az vmss update`: Correction d’un problème de mise à jour de notification d’arrêt</span><span class="sxs-lookup"><span data-stu-id="a6136-262">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="a6136-263">`az vm/vmss create`: Ajout de la prise en charge de la version d’image spécialisée</span><span class="sxs-lookup"><span data-stu-id="a6136-263">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="a6136-264">Version de l’API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="a6136-264">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="a6136-265">`az sig image-version create`: Ajout de --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="a6136-265">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="a6136-266">Correction de l’échec des tests lors d’une exécution en série en raison d’un nom de coffre de clés en double dans le cache en mémoire global</span><span class="sxs-lookup"><span data-stu-id="a6136-266">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-267">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-267">CosmosDB</span></span>

* <span data-ttu-id="a6136-268">Prise en charge d’`az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="a6136-268">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6136-269">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6136-269">IoT Central</span></span>

* <span data-ttu-id="a6136-270">Dépréciation d’`az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="a6136-270">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="a6136-271">Ajout du module de commande `az iot central`</span><span class="sxs-lookup"><span data-stu-id="a6136-271">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-272">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-272">Monitor</span></span>

* <span data-ttu-id="a6136-273">Prise en charge du scénario de lien privé pour la supervision</span><span class="sxs-lookup"><span data-stu-id="a6136-273">Support private link scenario for monitor</span></span>
* <span data-ttu-id="a6136-274">Correction du mode de simulation incorrect dans test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="a6136-274">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="a6136-275">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-275">Network</span></span>

* <span data-ttu-id="a6136-276">Dépréciation de la référence sku pour la commande de mise à jour de l’adresse IP publique</span><span class="sxs-lookup"><span data-stu-id="a6136-276">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="a6136-277">`az network private-endpoint`: Prise en charge du groupe de zones DNS privées</span><span class="sxs-lookup"><span data-stu-id="a6136-277">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="a6136-278">Activation de la fonctionnalité de contexte local pour le paramètre de réseau virtuel/sous-réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-278">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="a6136-279">Correction d’un exemple d’utilisation incorrect dans test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="a6136-279">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-280">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-280">Packaging</span></span>

* <span data-ttu-id="a6136-281">Suppression de la prise en charge d’un package Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="a6136-281">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-282">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-282">RBAC</span></span>

* <span data-ttu-id="a6136-283">`az ad app create/update` : prise en charge de --optional-claims en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="a6136-283">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-284">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-284">RDBMS</span></span>

* <span data-ttu-id="a6136-285">Ajout des commandes d’administrateur Azure Active Directory pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="a6136-285">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6136-286">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-286">Service Fabric</span></span>

* <span data-ttu-id="a6136-287">Correctif n  12891 : `az sf application update --application-parameters` supprime les anciens paramètres qui ne sont pas dans la demande</span><span class="sxs-lookup"><span data-stu-id="a6136-287">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="a6136-288">Correctif n  12470, az sf create cluster, résolution de bogues dans la durabilité et la fiabilité des mises à jour, et recherche de groupes identiques de machines virtuelles correctement dans le code en fonction d’un nom de type de nœud</span><span class="sxs-lookup"><span data-stu-id="a6136-288">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-289">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-289">SQL</span></span>

* <span data-ttu-id="a6136-290">Ajout d’`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="a6136-290">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="a6136-291">`az sql midb` : mise à jour/affichage de la stratégie de conservation à long terme, affichage/suppression des sauvegardes de conservation à long terme, restauration de la sauvegarde de conservation à long terme</span><span class="sxs-lookup"><span data-stu-id="a6136-291">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-292">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-292">Storage</span></span>

* <span data-ttu-id="a6136-293">Mise à niveau d’azure-mgmt-storage vers 9.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-293">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="a6136-294">`az storage logging off`: Prise en charge de la désactivation de la journalisation pour un compte de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-294">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="a6136-295">`az storage account update`: Activation de la rotation automatique de la clé pour CMK</span><span class="sxs-lookup"><span data-stu-id="a6136-295">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="a6136-296">`az storage account encryption-scope create/update/list/show`: Ajout de la prise en charge de la personnalisation de l’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="a6136-296">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="a6136-297">`az storage container create`: Ajout de --default-encryption-scope et --deny-encryption-scope-override pour définir l’étendue du chiffrement de niveau de conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-297">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="a6136-298">Enquête</span><span class="sxs-lookup"><span data-stu-id="a6136-298">Survey</span></span>

* <span data-ttu-id="a6136-299">Ajout d’une instruction switch pour désactiver le lien d’enquête</span><span class="sxs-lookup"><span data-stu-id="a6136-299">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="a6136-300">01 avril 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-300">April 01, 2020</span></span>

<span data-ttu-id="a6136-301">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="a6136-301">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-302">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-302">ACR</span></span>

* <span data-ttu-id="a6136-303">Correction d’une version incorrecte d’azure-mgmt-containerregistry pour Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-303">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-304">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-304">Profile</span></span>

* <span data-ttu-id="a6136-305">az login : Correction des échecs de connexion avec les profils cloud autres que `latest`</span><span class="sxs-lookup"><span data-stu-id="a6136-305">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="a6136-306">31 mars 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-306">March 31, 2020</span></span>

<span data-ttu-id="a6136-307">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="a6136-307">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-308">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-308">ACR</span></span>

* <span data-ttu-id="a6136-309">'az acr task update' : exception du pointeur null</span><span class="sxs-lookup"><span data-stu-id="a6136-309">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="a6136-310">`az acr import`: Modification de l’aide et du message d’erreur pour clarifier l’utilisation de --source et --registry</span><span class="sxs-lookup"><span data-stu-id="a6136-310">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="a6136-311">Ajout d’un validateur pour l’argument 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="a6136-311">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="a6136-312">`az acr login` : Suppression de l’indicateur de préversion sur '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="a6136-312">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="a6136-313">[CHANGEMENT CASSANT] Suppression du paramètre de branche 'az acr task create/update'</span><span class="sxs-lookup"><span data-stu-id="a6136-313">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="a6136-314">'az acr task update' : Le client peut maintenant mettre à jour le contexte, git-token et/ou les déclencheurs individuellement</span><span class="sxs-lookup"><span data-stu-id="a6136-314">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="a6136-315">'az acr agentpool' : nouvelle fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="a6136-315">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-316">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-316">AKS</span></span>

* <span data-ttu-id="a6136-317">Correction d’apiServerAccessProfile lors de la mise à jour de --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="a6136-317">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="a6136-318">aks update : Remplacement des adresses IP sortantes par des valeurs d’entrée lors de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-318">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="a6136-319">Pas de création de SPN pour les clusters MSI et prise en charge de l’attachement d’acr à des clusters MSI</span><span class="sxs-lookup"><span data-stu-id="a6136-319">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-320">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-320">AMS</span></span>

* <span data-ttu-id="a6136-321">Correctif #12469 : échec de l’ajout de Fairplay content-key-policy en raison de problèmes avec le paramètre « ask »</span><span class="sxs-lookup"><span data-stu-id="a6136-321">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-322">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-322">AppConfig</span></span>

* <span data-ttu-id="a6136-323">Ajout de --skip-keyvault pour l’exportation de kv</span><span class="sxs-lookup"><span data-stu-id="a6136-323">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-324">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-324">AppService</span></span>

* <span data-ttu-id="a6136-325">Correctif #12509 : Suppression de la balise d’az webapp up par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-325">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="a6136-326">az functionapp create : Mise à jour du menu d’aide --runtime-version et ajout d’un avertissement quand l’utilisateur spécifie --runtime-version pour dotnet</span><span class="sxs-lookup"><span data-stu-id="a6136-326">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="a6136-327">az functionapp create : Mise à jour du mode de définition de javaVersion pour les applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-327">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-328">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-328">ARM</span></span>

* <span data-ttu-id="a6136-329">az deployment create/validate : Utilisation du --handle-extended-json-format par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-329">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="a6136-330">az lock create : Ajout d’exemples de création de sous-ressources dans la documentation d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-330">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="a6136-331">az deployment {group/mg/sub/tenant} list : Prise en charge du filtrage provisioningState</span><span class="sxs-lookup"><span data-stu-id="a6136-331">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="a6136-332">az deployment : Correction du bogue d’analyse pour les commentaires sous le dernier argument</span><span class="sxs-lookup"><span data-stu-id="a6136-332">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-333">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-333">Backup</span></span>

* <span data-ttu-id="a6136-334">Ajout de plusieurs fonctionnalités de restauration de fichiers</span><span class="sxs-lookup"><span data-stu-id="a6136-334">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="a6136-335">Ajout de la prise en charge de la sauvegarde des disques de système d’exploitation uniquement</span><span class="sxs-lookup"><span data-stu-id="a6136-335">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="a6136-336">Ajout du paramètre restore-as-unmanaged-disk pour spécifier une restauration non gérée</span><span class="sxs-lookup"><span data-stu-id="a6136-336">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-337">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-337">Compute</span></span>

* <span data-ttu-id="a6136-338">az vm create : Ajout de l’option NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="a6136-338">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="a6136-339">az vmss create/update : suppression de la balise d’aperçu des réparations automatiques vmss</span><span class="sxs-lookup"><span data-stu-id="a6136-339">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="a6136-340">az vm update : Prise en charge de --workspace</span><span class="sxs-lookup"><span data-stu-id="a6136-340">az vm update: Support --workspace</span></span>
* <span data-ttu-id="a6136-341">Correction d’un bogue dans le code d’initialisation VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="a6136-341">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="a6136-342">Mise à niveau de VMAccessAgent vers la version 2.4</span><span class="sxs-lookup"><span data-stu-id="a6136-342">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="a6136-343">az vmss set-orchestration-service-state : prise en charge de l’état de la définition du service d’orchestration vmss</span><span class="sxs-lookup"><span data-stu-id="a6136-343">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="a6136-344">Mise à niveau de la version d’API de disque vers la version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="a6136-344">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="a6136-345">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="a6136-345">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-346">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-346">Cosmos DB</span></span>

* <span data-ttu-id="a6136-347">Correction de l’option --type manquante pour les redirections de dépréciation</span><span class="sxs-lookup"><span data-stu-id="a6136-347">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="a6136-348">Docker</span><span class="sxs-lookup"><span data-stu-id="a6136-348">Docker</span></span>

* <span data-ttu-id="a6136-349">Mise à jour vers Alpine 3.11 et Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="a6136-349">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-350">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-350">Extension</span></span>

* <span data-ttu-id="a6136-351">Autorisation de charger des extensions dans le chemin système via des packages</span><span class="sxs-lookup"><span data-stu-id="a6136-351">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-352">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-352">HDInsight</span></span>

* <span data-ttu-id="a6136-353">(az hdinsight create:) Les clients du support spécifient une version TLS minimale prise en charge à l’aide du paramètre `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="a6136-353">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="a6136-354">La valeur autorisée est 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="a6136-354">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-355">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-355">IoT</span></span>

* <span data-ttu-id="a6136-356">Ajout de codeowner</span><span class="sxs-lookup"><span data-stu-id="a6136-356">Add codeowner</span></span>
* <span data-ttu-id="a6136-357">az iot hub create : changement de la référence SKU par défaut S1 en F1</span><span class="sxs-lookup"><span data-stu-id="a6136-357">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="a6136-358">iot hub : Prise en charge d’IotHub dans le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="a6136-358">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a6136-359">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a6136-359">IoTCentral</span></span>

* <span data-ttu-id="a6136-360">Mise à jour des détails d’erreur, du modèle d’application par défaut et du message d’invite</span><span class="sxs-lookup"><span data-stu-id="a6136-360">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-361">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-361">KeyVault</span></span>

* <span data-ttu-id="a6136-362">Prise en charge de la sauvegarde/restauration de certificat</span><span class="sxs-lookup"><span data-stu-id="a6136-362">Support certificate backup/restore</span></span>
* <span data-ttu-id="a6136-363">keyvault create/update : Prise en charge de --retention-days</span><span class="sxs-lookup"><span data-stu-id="a6136-363">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="a6136-364">Plus d’affichage des clés/secrets managés lors du listing</span><span class="sxs-lookup"><span data-stu-id="a6136-364">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="a6136-365">az keyvault create : prise en charge de `--network-acls`, `--network-acls-ips` et `--network-acls-vnets` pour spécifier des règles réseau lors de la création de coffres</span><span class="sxs-lookup"><span data-stu-id="a6136-365">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="a6136-366">Verrouillage</span><span class="sxs-lookup"><span data-stu-id="a6136-366">Lock</span></span>

* <span data-ttu-id="a6136-367">Correction de bogue pour az lock delete : az lock delete ne fonctionne pas sur Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a6136-367">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-368">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-368">Monitor</span></span>

* <span data-ttu-id="a6136-369">az monitor clone : prise en charge des règles de clonage de métriques d’une ressource à une autre</span><span class="sxs-lookup"><span data-stu-id="a6136-369">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="a6136-370">Correctif IcM179210086 : impossible de créer une alerte de métrique personnalisée pour la métrique Application Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-370">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="a6136-371">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="a6136-371">NetAppFiles</span></span>

* <span data-ttu-id="a6136-372">az volume create : Autorisation des volumes de protection des données à ajouter des opérations de réplication : approuver, suspendre, reprendre, état, supprimer</span><span class="sxs-lookup"><span data-stu-id="a6136-372">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="a6136-373">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-373">Network</span></span>

* <span data-ttu-id="a6136-374">az network application-gateway waf-policy managed-rule rule-set add : prise en charge de Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="a6136-374">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="a6136-375">network watcher flow-log show: correction d’une information de dépréciation fausse</span><span class="sxs-lookup"><span data-stu-id="a6136-375">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="a6136-376">Prise en charge des noms d’hôte dans l’écouteur de passerelle d’application</span><span class="sxs-lookup"><span data-stu-id="a6136-376">support host names in application gateway listener</span></span>
* <span data-ttu-id="a6136-377">az network nat gateway : prise en charge de la création d’une ressource vide sans IP publique ni préfixe d’IP publique</span><span class="sxs-lookup"><span data-stu-id="a6136-377">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="a6136-378">Prise en charge de la génération de passerelles VPN</span><span class="sxs-lookup"><span data-stu-id="a6136-378">Support vpn gateway generation</span></span>
* <span data-ttu-id="a6136-379">Prise en charge de `--if-none-match` dans `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="a6136-379">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-380">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-380">Packaging</span></span>

* <span data-ttu-id="a6136-381">Arrêt de la prise en charge de Python 3.5</span><span class="sxs-lookup"><span data-stu-id="a6136-381">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-382">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-382">Profile</span></span>

* <span data-ttu-id="a6136-383">az login : Affichage d’un avertissement pour l’erreur MFA</span><span class="sxs-lookup"><span data-stu-id="a6136-383">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-384">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-384">RDBMS</span></span>

* <span data-ttu-id="a6136-385">Ajout de commandes de gestion de clés de chiffrement de données de serveur pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="a6136-385">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="a6136-386">10 mars 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-386">March 10, 2020</span></span>

<span data-ttu-id="a6136-387">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="a6136-387">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-388">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-388">ACR</span></span>

* <span data-ttu-id="a6136-389">Correctif : `az acr login` déclenche une erreur de manière erronée</span><span class="sxs-lookup"><span data-stu-id="a6136-389">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="a6136-390">Ajout d’une nouvelle commande `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="a6136-390">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="a6136-391">Ajout d’un lien privé et de la prise en charge CMK</span><span class="sxs-lookup"><span data-stu-id="a6136-391">Add private link and CMK support</span></span>
* <span data-ttu-id="a6136-392">Ajout de la commande « private-link-resource list »</span><span class="sxs-lookup"><span data-stu-id="a6136-392">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-393">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-393">AKS</span></span>

* <span data-ttu-id="a6136-394">Correction de la navigation aks dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-394">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="a6136-395">az aks : correction de la supervision des erreurs NoneType addon et agentpool</span><span class="sxs-lookup"><span data-stu-id="a6136-395">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="a6136-396">Ajout de --nodepool-tags au pool de nœuds lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-396">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="a6136-397">Ajout de --tags lors de l’ajout ou de la mise à jour d’un nodepool à un cluster</span><span class="sxs-lookup"><span data-stu-id="a6136-397">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="a6136-398">aks create : ajout de `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="a6136-398">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="a6136-399">Ajout de --nodepool-labels lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-399">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="a6136-400">Ajout de --labels lors de l’ajout d’un nouveau nodepool à un cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-400">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="a6136-401">Ajout d’un caractère / manquant à l’URL de tableau de bord</span><span class="sxs-lookup"><span data-stu-id="a6136-401">add missing / in the dashboard url</span></span>
* <span data-ttu-id="a6136-402">Prise en charge de la création de clusters AKS activant l’identité managée</span><span class="sxs-lookup"><span data-stu-id="a6136-402">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="a6136-403">az aks : validation du plug-in réseau pour qu’il soit « azure » ou « kubenet »</span><span class="sxs-lookup"><span data-stu-id="a6136-403">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="a6136-404">az aks : Ajout de la prise en charge des clés de session AAD</span><span class="sxs-lookup"><span data-stu-id="a6136-404">az aks: Add aad session key support</span></span>
* <span data-ttu-id="a6136-405">[CHANGEMENT CASSANT] az aks : prise en charge des modifications MSI pour GF et BF pour omsagent (supervision de conteneur) (#1)</span><span class="sxs-lookup"><span data-stu-id="a6136-405">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="a6136-406">az aks use-dev-spaces : ajout de l’option de type de point de terminaison à la commande use-dev-spaces pour personnaliser le point de terminaison créé sur un contrôleur Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="a6136-406">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-407">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-407">AppConfig</span></span>

* <span data-ttu-id="a6136-408">Déblocage de l’utilisation de « kv set » pour ajouter la fonctionnalité et la référence de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="a6136-408">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-409">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-409">AppService</span></span>

* <span data-ttu-id="a6136-410">az webapp create : résolution d’un problème lors de l’exécution de la commande avec --runtime</span><span class="sxs-lookup"><span data-stu-id="a6136-410">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="a6136-411">az functionapp deployment source config-zip : ajout d’un message d’erreur si le nom du groupe de ressources ou de la fonction n’est pas valide ou n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a6136-411">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="a6136-412">functionapp create : correction du message d’avertissement qui s’affiche aujourd’hui avec `functionapp create`, qui mentionne un indicateur `--functions_version` mais utilise de manière erronée un `_` au lieu d’un `-` dans le nom de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="a6136-412">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="a6136-413">az functionapp create : mise à jour de la façon dont linuxFxVersion et le nom de l’image conteneur étaient définis pour les applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-413">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="a6136-414">az functionapp deployment source config-zip : résolution d’un problème dû à une condition de concurrence en cas de modification des paramètres d’application pendant le déploiement de fichier zip, provoquant des erreurs 5xx lors du déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-414">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="a6136-415">Correctif 5720946 : az webapp backup ne parvient pas à définir le nom</span><span class="sxs-lookup"><span data-stu-id="a6136-415">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-416">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-416">ARM</span></span>

* <span data-ttu-id="a6136-417">az resource : amélioration des exemples du module de ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-417">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="a6136-418">az policy assignment list : prise en charge de l’énumération des affectations de stratégie au niveau de l’étendue du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="a6136-418">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="a6136-419">Ajout de `az deployment group` et `az deployment operation group` pour le déploiement de modèle au niveau des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="a6136-419">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="a6136-420">Il s’agit d’un doublon de `az group deployment` et `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="a6136-420">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="a6136-421">Ajout de `az deployment sub` et `az deployment operation sub` pour le déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a6136-421">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="a6136-422">Il s’agit d’un doublon de `az deployment` et `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="a6136-422">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="a6136-423">Ajout de `az deployment mg` et `az deployment operation mg` pour le déploiement de modèle au niveau des groupes de gestion</span><span class="sxs-lookup"><span data-stu-id="a6136-423">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="a6136-424">Ajout de `az deployment tenant` et `az deployment operation tenant` pour le déploiement de modèle à l’étendue du locataire</span><span class="sxs-lookup"><span data-stu-id="a6136-424">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="a6136-425">az policy assignment create : ajout d’une description au paramètre `--location`</span><span class="sxs-lookup"><span data-stu-id="a6136-425">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="a6136-426">az group deployment create : ajout du paramètre `--aux-tenants` pour prendre en charge les locataires croisés</span><span class="sxs-lookup"><span data-stu-id="a6136-426">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-427">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-427">CDN</span></span>

* <span data-ttu-id="a6136-428">Ajouter de commandes WAF CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-428">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-429">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-429">Compute</span></span>

* <span data-ttu-id="a6136-430">az sig image-version : ajout de --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="a6136-430">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="a6136-431">az ppg show: ajout de --colocation-status pour permettre l’extraction de l’état de colocalisation de toutes les ressources dans le groupe de placement de proximité</span><span class="sxs-lookup"><span data-stu-id="a6136-431">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="a6136-432">az vmss create/update : prise en charge des réparations automatiques</span><span class="sxs-lookup"><span data-stu-id="a6136-432">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="a6136-433">[CHANGEMENT CASSANT] az image template : template a été renommé builder</span><span class="sxs-lookup"><span data-stu-id="a6136-433">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="a6136-434">az image builder create : ajout de --image-template</span><span class="sxs-lookup"><span data-stu-id="a6136-434">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-435">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-435">Cosmos DB</span></span>

* <span data-ttu-id="a6136-436">Ajout d’applets de commande de déclencheur, de procédure stockée SQL et de fonctions définies par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a6136-436">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="a6136-437">az cosmosdb create : ajout de --key-uri pour prendre en charge l’ajout d’informations de chiffrement de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="a6136-437">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-438">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-438">KeyVault</span></span>

* <span data-ttu-id="a6136-439">keyvault create : activation de la suppression réversible par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-439">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-440">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-440">Monitor</span></span>

* <span data-ttu-id="a6136-441">az monitor metrics alert create : prise en charge de `~` dans `--condition`</span><span class="sxs-lookup"><span data-stu-id="a6136-441">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-442">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-442">Network</span></span>

* <span data-ttu-id="a6136-443">az network application-gateway rewrite-rule create : prise en charge de la configuration d’URL</span><span class="sxs-lookup"><span data-stu-id="a6136-443">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="a6136-444">az network dns zone import : --zone-name respectera la casse à l’avenir</span><span class="sxs-lookup"><span data-stu-id="a6136-444">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="a6136-445">az network private-endpoint/private-link-service : suppression de l’étiquette d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a6136-445">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="a6136-446">az network bastion : prise en charge de bastion</span><span class="sxs-lookup"><span data-stu-id="a6136-446">az network bastion: support bastion</span></span>
* <span data-ttu-id="a6136-447">az network vnet list-available-ips : prise en charge de l’énumération des adresses IP disponibles sur un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a6136-447">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="a6136-448">az network watcher flow-log create/list/delete/update : ajout de nouvelles commandes pour gérer le journal de flux d’observateur et l’exposition de --location pour identifier explicitement l’observateur</span><span class="sxs-lookup"><span data-stu-id="a6136-448">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="a6136-449">az network watcher flow-log configure : dépréciée</span><span class="sxs-lookup"><span data-stu-id="a6136-449">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="a6136-450">az network watcher flow-log show : prise en charge de --location et de --name pour obtenir un résultat au format ARM. L’ancienne sortie mise en forme est dépréciée</span><span class="sxs-lookup"><span data-stu-id="a6136-450">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="a6136-451">Stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-451">Policy</span></span>

* <span data-ttu-id="a6136-452">az policy assignment create : correction du bogue qui générait automatiquement un nom d’attribution de stratégie dépassant la limite</span><span class="sxs-lookup"><span data-stu-id="a6136-452">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-453">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-453">RBAC</span></span>

* <span data-ttu-id="a6136-454">az ad group show : correction du bogue qui faisait que --group était traité comme un problème Regex</span><span class="sxs-lookup"><span data-stu-id="a6136-454">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-455">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-455">RDBMS</span></span>

* <span data-ttu-id="a6136-456">Passage du SDK azure-mgmt-rdbms à la version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-456">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="a6136-457">az postgres private-endpoint-connection : gestion des connexions de point de terminaison privé postgres</span><span class="sxs-lookup"><span data-stu-id="a6136-457">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="a6136-458">az postgres private-link-resource : gestion des ressources de lien privé postgres</span><span class="sxs-lookup"><span data-stu-id="a6136-458">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="a6136-459">az mysql private-endpoint-connection : gestion des connexions de point de terminaison privé mysql</span><span class="sxs-lookup"><span data-stu-id="a6136-459">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="a6136-460">az mysql private-link-resource : gestion des ressources de lien privé mysql</span><span class="sxs-lookup"><span data-stu-id="a6136-460">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="a6136-461">az mariadb private-endpoint-connection : gestion des connexions de point de terminaison privé mariadb</span><span class="sxs-lookup"><span data-stu-id="a6136-461">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="a6136-462">az mariadb private-link-resource : gestion des ressources de lien privé mariadb</span><span class="sxs-lookup"><span data-stu-id="a6136-462">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="a6136-463">Mise à jour des tests de point de terminaison privé SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-463">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-464">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-464">SQL</span></span>

* <span data-ttu-id="a6136-465">Sql midb ; ajout de list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="a6136-465">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="a6136-466">(sql server create :) Ajout de l’indicateur facultatif « Enable »/« Disable » d’accès au réseau public à sql server create</span><span class="sxs-lookup"><span data-stu-id="a6136-466">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="a6136-467">(sql server update :) modifications du client</span><span class="sxs-lookup"><span data-stu-id="a6136-467">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="a6136-468">Ajout de propriété minimal_tls_version pour MI et SQL DB</span><span class="sxs-lookup"><span data-stu-id="a6136-468">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-469">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-469">Storage</span></span>

* <span data-ttu-id="a6136-470">az storage blob delete-batch : comportement incorrect de l’indicateur `--dryrun`</span><span class="sxs-lookup"><span data-stu-id="a6136-470">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="a6136-471">az storage account network-rule add (correctif de bogue) : l’opération d’ajout doit être idempotent</span><span class="sxs-lookup"><span data-stu-id="a6136-471">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="a6136-472">az storage account create/update : Ajout de la prise en charge des préférences de routage</span><span class="sxs-lookup"><span data-stu-id="a6136-472">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="a6136-473">Mise à niveau de la version azure-mgmt-storage vers 8.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-473">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="a6136-474">az storage container immutability create : ajout du paramètre --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="a6136-474">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="a6136-475">az storage account private-link-resource list : ajout de la prise en charge de l’énumération des ressources de lien privé pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-475">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="a6136-476">az storage account private-endpoint-connection approve/reject/show/delete : prise en charge de la gestion des connexions de point de terminaison privé</span><span class="sxs-lookup"><span data-stu-id="a6136-476">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="a6136-477">az storage account blob-service-properties update : ajout de --enable-restore-policy et --restore-days</span><span class="sxs-lookup"><span data-stu-id="a6136-477">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="a6136-478">az storage blob restore : ajout de la prise en charge de la restauration des plages d’objets blob</span><span class="sxs-lookup"><span data-stu-id="a6136-478">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="a6136-479">18 février 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-479">February 18, 2020</span></span>

<span data-ttu-id="a6136-480">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="a6136-480">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-481">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-481">ACR</span></span>

* <span data-ttu-id="a6136-482">Ajoute un nouvel argument `--expose-token` pour `az acr login`</span><span class="sxs-lookup"><span data-stu-id="a6136-482">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="a6136-483">Corrige la sortie incorrecte de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="a6136-483">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="a6136-484">az acr login : lève une CLIError si des erreurs sont retournées par la commande docker</span><span class="sxs-lookup"><span data-stu-id="a6136-484">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-485">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-485">ACS</span></span>

* <span data-ttu-id="a6136-486">aks create/update : ajoute la validation `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="a6136-486">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="a6136-487">Aladdin</span><span class="sxs-lookup"><span data-stu-id="a6136-487">Aladdin</span></span>

* <span data-ttu-id="a6136-488">Analyse les exemples générés dans le _help.py des commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-488">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-489">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-489">AMS</span></span>

* <span data-ttu-id="a6136-490">az ams est désormais en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="a6136-490">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-491">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-491">AppConfig</span></span>

* <span data-ttu-id="a6136-492">Modifie le message d’aide pour exclure les filtres de clé ou d’étiquette non pris en charge</span><span class="sxs-lookup"><span data-stu-id="a6136-492">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="a6136-493">Supprimer l’étiquette d’aperçu pour la plupart des commandes, à l’exception des indicateurs d’identité managée et de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a6136-493">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="a6136-494">Ajoute une clé gérée par le client lors de la mise à jour des magasins</span><span class="sxs-lookup"><span data-stu-id="a6136-494">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-495">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-495">AppService</span></span>

* <span data-ttu-id="a6136-496">az webapp list-runtimes : correction du bogue concernant list-runtimes</span><span class="sxs-lookup"><span data-stu-id="a6136-496">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="a6136-497">Ajoute az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="a6136-497">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="a6136-498">Ajoute la prise en charge des applications de fonction v3 et du nœud 12</span><span class="sxs-lookup"><span data-stu-id="a6136-498">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-499">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-499">ARM</span></span>

* <span data-ttu-id="a6136-500">az policy assignment create : correction du message d’erreur lorsque le paramètre `--policy` n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="a6136-500">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="a6136-501">az group deployment create : correction de l’erreur « stat: path too long for Windows » (Chemin trop long pour Windows) lors de l’utilisation d’un fichier parameters.json volumineux</span><span class="sxs-lookup"><span data-stu-id="a6136-501">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-502">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-502">Backup</span></span>

* <span data-ttu-id="a6136-503">Correction du flux de récupération au niveau de l’élément dans OLR</span><span class="sxs-lookup"><span data-stu-id="a6136-503">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="a6136-504">Ajout de la prise en charge de la restauration sous forme de fichiers pour les bases de données SQL et SAP</span><span class="sxs-lookup"><span data-stu-id="a6136-504">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-505">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-505">Compute</span></span>

* <span data-ttu-id="a6136-506">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="a6136-506">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="a6136-507">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="a6136-507">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="a6136-508">az vm host : supprime l’étiquette d’aperçu pour `vm host` et `vm host group`</span><span class="sxs-lookup"><span data-stu-id="a6136-508">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="a6136-509">[CHANGEMENT CASSANT] Correctif n° 10728 : `az vm create` Création automatique d’un sous-réseau si un réseau virtuel est spécifié et s’il n’existe pas de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-509">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="a6136-510">Amélioration de la robustesse de la liste d’images de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="a6136-510">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="a6136-511">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a6136-511">Eventhub</span></span>

* <span data-ttu-id="a6136-512">Prise en charge d’Azure Stack pour le profil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="a6136-512">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-513">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-513">KeyVault</span></span>

* <span data-ttu-id="a6136-514">az keyvault key create : ajouter une nouvelle valeur `import` pour le paramètre `--ops`</span><span class="sxs-lookup"><span data-stu-id="a6136-514">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="a6136-515">az keyvault key list-versions : prise en charge du paramètre `--id` pour la spécification des clés</span><span class="sxs-lookup"><span data-stu-id="a6136-515">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="a6136-516">Prise en charge des connexions de points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="a6136-516">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="a6136-517">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-517">Network</span></span>

* <span data-ttu-id="a6136-518">Passage à azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-518">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="a6136-519">az network private-link-service update/create: support --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="a6136-519">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="a6136-520">Ajout de la fonctionnalité Moniteur de connexion v2</span><span class="sxs-lookup"><span data-stu-id="a6136-520">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-521">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-521">Packaging</span></span>

* <span data-ttu-id="a6136-522">[CHANGEMENT CASSANT] Python 2.7 n’est plus pris en charge</span><span class="sxs-lookup"><span data-stu-id="a6136-522">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-523">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-523">Profile</span></span>

* <span data-ttu-id="a6136-524">Aperçu : Ajoutez les nouveaux attributs `homeTenantId` et `managedByTenants` aux comptes d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a6136-524">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="a6136-525">Réexécutez `az login` pour que les modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="a6136-525">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="a6136-526">az login : affiche un avertissement lorsqu’un abonnement est listé par plusieurs locataires et s’affiche par défaut pour le premier.</span><span class="sxs-lookup"><span data-stu-id="a6136-526">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="a6136-527">Pour sélectionner un locataire lors de l’accès à cet abonnement, ajoutez `--tenant` dans `az login`</span><span class="sxs-lookup"><span data-stu-id="a6136-527">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="a6136-528">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-528">Role</span></span>

* <span data-ttu-id="a6136-529">az role assignment create : correction de l’erreur lors de laquelle l’attribution d’un rôle à un principal de service par nom d’affichage générait une erreur HTTP 400</span><span class="sxs-lookup"><span data-stu-id="a6136-529">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-530">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-530">SQL</span></span>

* <span data-ttu-id="a6136-531">Mise à jour de l’applet de commande SQL Managed Instance `az sql mi update` avec deux nouveaux paramètres : tier et family</span><span class="sxs-lookup"><span data-stu-id="a6136-531">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-532">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-532">Storage</span></span>

* <span data-ttu-id="a6136-533">[CHANGEMENT CASSANT] `az storage account create` : Remplacement du type de compte de stockage par défaut par StorageV2</span><span class="sxs-lookup"><span data-stu-id="a6136-533">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="a6136-534">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-534">February 04, 2020</span></span>

<span data-ttu-id="a6136-535">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="a6136-535">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-536">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-536">ACS</span></span>

* <span data-ttu-id="a6136-537">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="a6136-537">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="a6136-538">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="a6136-538">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-539">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-539">ACR</span></span>

* <span data-ttu-id="a6136-540">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="a6136-540">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="a6136-541">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="a6136-541">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="a6136-542">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="a6136-542">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-543">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-543">AKS</span></span>

* <span data-ttu-id="a6136-544">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="a6136-544">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-545">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-545">AppConfig</span></span>

* <span data-ttu-id="a6136-546">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="a6136-546">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="a6136-547">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="a6136-547">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="a6136-548">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="a6136-548">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="a6136-549">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="a6136-549">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="a6136-550">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="a6136-550">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-551">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-551">AppService</span></span>

* <span data-ttu-id="a6136-552">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="a6136-552">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="a6136-553">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-553">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-554">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-554">ARM</span></span>

* <span data-ttu-id="a6136-555">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-555">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="a6136-556">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="a6136-556">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="a6136-557">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="a6136-557">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="a6136-558">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="a6136-558">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="a6136-559">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="a6136-559">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="a6136-560">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="a6136-560">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="a6136-561">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="a6136-561">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-562">BotService</span><span class="sxs-lookup"><span data-stu-id="a6136-562">BotService</span></span>

* <span data-ttu-id="a6136-563">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="a6136-563">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="a6136-564">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="a6136-564">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-565">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-565">CDN</span></span>

* <span data-ttu-id="a6136-566">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="a6136-566">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="a6136-567">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="a6136-567">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="a6136-568">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="a6136-568">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="a6136-569">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-569">Deployment Manager</span></span>

* <span data-ttu-id="a6136-570">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="a6136-570">Add list operation for all resources.</span></span>
* <span data-ttu-id="a6136-571">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="a6136-571">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="a6136-572">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="a6136-572">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-573">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-573">IoT</span></span>

* <span data-ttu-id="a6136-574">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="a6136-574">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6136-575">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6136-575">IoT Central</span></span>

* <span data-ttu-id="a6136-576">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="a6136-576">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-577">Key Vault</span></span>

* <span data-ttu-id="a6136-578">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="a6136-578">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="a6136-579">Divers</span><span class="sxs-lookup"><span data-stu-id="a6136-579">Misc</span></span>

* <span data-ttu-id="a6136-580">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="a6136-580">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="a6136-581">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-581">Network</span></span>

* <span data-ttu-id="a6136-582">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="a6136-582">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="a6136-583">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="a6136-583">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="a6136-584">Stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-584">Policy</span></span>

* <span data-ttu-id="a6136-585">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="a6136-585">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="a6136-586">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="a6136-586">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-587">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-587">Profile</span></span>

* <span data-ttu-id="a6136-588">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-588">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-589">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-589">RBAC</span></span>

* <span data-ttu-id="a6136-590">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-590">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="a6136-591">Sécurité</span><span class="sxs-lookup"><span data-stu-id="a6136-591">Security</span></span>

* <span data-ttu-id="a6136-592">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="a6136-592">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-593">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-593">SQL</span></span>

* <span data-ttu-id="a6136-594">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="a6136-594">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="a6136-595">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="a6136-595">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="a6136-596">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="a6136-596">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="a6136-597">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="a6136-597">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="a6136-598">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="a6136-598">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="a6136-599">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="a6136-599">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-600">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-600">Storage</span></span>

* <span data-ttu-id="a6136-601">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="a6136-601">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="a6136-602">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="a6136-602">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="a6136-603">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="a6136-603">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="a6136-604">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="a6136-604">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="a6136-605">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="a6136-605">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="a6136-606">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="a6136-606">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a6136-607">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a6136-607">ServiceFabric</span></span>

* <span data-ttu-id="a6136-608">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="a6136-608">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="a6136-609">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-609">January 13, 2020</span></span>

<span data-ttu-id="a6136-610">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="a6136-610">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-611">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-611">Compute</span></span>

* <span data-ttu-id="a6136-612">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="a6136-612">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="a6136-613">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="a6136-613">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-614">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-614">Storage</span></span>

* <span data-ttu-id="a6136-615">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="a6136-615">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="a6136-616">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="a6136-616">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="a6136-617">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="a6136-617">January 07, 2020</span></span>

<span data-ttu-id="a6136-618">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="a6136-618">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-619">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-619">ACR</span></span>

* <span data-ttu-id="a6136-620">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="a6136-620">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="a6136-621">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="a6136-621">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-622">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-622">AppConfig</span></span>

* <span data-ttu-id="a6136-623">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="a6136-623">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="a6136-624">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-624">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="a6136-625">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="a6136-625">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-626">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-626">AppService</span></span>

* <span data-ttu-id="a6136-627">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="a6136-627">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="a6136-628">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-628">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="a6136-629">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="a6136-629">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-630">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-630">ARM</span></span>

* <span data-ttu-id="a6136-631">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="a6136-631">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-632">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-632">Backup</span></span>

* <span data-ttu-id="a6136-633">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="a6136-633">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="a6136-634">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="a6136-634">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="a6136-635">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="a6136-635">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-636">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-636">Compute</span></span>

* <span data-ttu-id="a6136-637">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6136-637">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="a6136-638">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="a6136-638">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="a6136-639">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="a6136-639">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-640">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-640">HDInsight</span></span>

* <span data-ttu-id="a6136-641">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="a6136-641">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="a6136-642">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="a6136-642">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="a6136-643">Divers</span><span class="sxs-lookup"><span data-stu-id="a6136-643">Misc.</span></span>

* <span data-ttu-id="a6136-644">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="a6136-644">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="a6136-645">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a6136-645">Event Hubs</span></span>

* <span data-ttu-id="a6136-646">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="a6136-646">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="a6136-647">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="a6136-647">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6136-648">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-648">Service Bus</span></span>

* <span data-ttu-id="a6136-649">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="a6136-649">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="a6136-650">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="a6136-650">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-651">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-651">RBAC</span></span>

* <span data-ttu-id="a6136-652">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a6136-652">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-653">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-653">Storage</span></span>

* <span data-ttu-id="a6136-654">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="a6136-654">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="a6136-655">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="a6136-655">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="a6136-656">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="a6136-656">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="a6136-657">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-657">December 17, 2019</span></span>

<span data-ttu-id="a6136-658">2.0.78</span><span class="sxs-lookup"><span data-stu-id="a6136-658">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-659">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-659">ACR</span></span>

* <span data-ttu-id="a6136-660">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="a6136-660">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-661">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-661">ACS</span></span>

* <span data-ttu-id="a6136-662">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="a6136-662">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-663">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-663">AMS</span></span>

* <span data-ttu-id="a6136-664">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="a6136-664">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-665">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-665">AppConfig</span></span>

* <span data-ttu-id="a6136-666">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="a6136-666">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="a6136-667">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="a6136-667">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="a6136-668">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="a6136-668">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-669">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-669">AppService</span></span>

* <span data-ttu-id="a6136-670">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="a6136-670">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="a6136-671">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="a6136-671">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="a6136-672">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="a6136-672">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="a6136-673">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="a6136-673">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-674">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-674">ARM</span></span>

* <span data-ttu-id="a6136-675">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-675">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="a6136-676">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="a6136-676">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="a6136-677">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="a6136-677">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-678">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-678">Backup</span></span>

* <span data-ttu-id="a6136-679">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="a6136-679">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-680">BotService</span><span class="sxs-lookup"><span data-stu-id="a6136-680">BotService</span></span>

* <span data-ttu-id="a6136-681">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="a6136-681">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="a6136-682">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="a6136-682">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="a6136-683">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="a6136-683">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="a6136-684">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="a6136-684">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="a6136-685">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="a6136-685">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="a6136-686">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="a6136-686">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="a6136-687">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="a6136-687">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="a6136-688">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="a6136-688">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="a6136-689">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="a6136-689">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-690">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-690">Compute</span></span>

* <span data-ttu-id="a6136-691">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="a6136-691">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="a6136-692">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="a6136-692">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="a6136-693">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="a6136-693">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="a6136-694">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="a6136-694">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="a6136-695">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="a6136-695">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="a6136-696">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="a6136-696">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="a6136-697">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-697">Core</span></span>

* <span data-ttu-id="a6136-698">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="a6136-698">Removed support for Python 3.4</span></span>
* <span data-ttu-id="a6136-699">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-699">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="a6136-700">DLS</span><span class="sxs-lookup"><span data-stu-id="a6136-700">DLS</span></span>

* <span data-ttu-id="a6136-701">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="a6136-701">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="a6136-702">Installer</span><span class="sxs-lookup"><span data-stu-id="a6136-702">Install</span></span>

* <span data-ttu-id="a6136-703">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="a6136-703">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-704">IOT</span><span class="sxs-lookup"><span data-stu-id="a6136-704">IOT</span></span>

* <span data-ttu-id="a6136-705">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="a6136-705">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="a6136-706">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="a6136-706">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-707">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-707">Key Vault</span></span>

* <span data-ttu-id="a6136-708">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-708">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="a6136-709">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="a6136-709">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="a6136-710">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="a6136-710">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="a6136-711">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="a6136-711">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="a6136-712">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="a6136-712">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-713">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-713">Network</span></span>

* <span data-ttu-id="a6136-714">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-714">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="a6136-715">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-715">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="a6136-716">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="a6136-716">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="a6136-717">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="a6136-717">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="a6136-718">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="a6136-718">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-719">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-719">Packaging</span></span>

* <span data-ttu-id="a6136-720">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="a6136-720">Added back edge builds for pip install</span></span>
* <span data-ttu-id="a6136-721">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="a6136-721">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="a6136-722">Stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-722">Policy</span></span>

* <span data-ttu-id="a6136-723">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="a6136-723">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="a6136-724">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="a6136-724">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="a6136-725">Redis</span><span class="sxs-lookup"><span data-stu-id="a6136-725">Redis</span></span>

* <span data-ttu-id="a6136-726">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="a6136-726">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="a6136-727">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="a6136-727">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a6136-728">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a6136-728">ServiceFabric</span></span>

* <span data-ttu-id="a6136-729">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="a6136-729">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="a6136-730">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="a6136-730">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-731">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-731">SQL</span></span>

* <span data-ttu-id="a6136-732">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="a6136-732">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-733">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-733">Storage</span></span>

* <span data-ttu-id="a6136-734">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="a6136-734">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="a6136-735">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="a6136-735">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="a6136-736">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="a6136-736">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="a6136-737">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="a6136-737">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="a6136-738">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="a6136-738">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="a6136-739">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-739">November 26, 2019</span></span>

<span data-ttu-id="a6136-740">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="a6136-740">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-741">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-741">ACR</span></span>

* <span data-ttu-id="a6136-742">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="a6136-742">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="a6136-743">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="a6136-743">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="a6136-744">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="a6136-744">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="a6136-745">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="a6136-745">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-746">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-746">AKS</span></span>

* <span data-ttu-id="a6136-747">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="a6136-747">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-748">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-748">AppConfig</span></span>

* <span data-ttu-id="a6136-749">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="a6136-749">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="a6136-750">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="a6136-750">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="a6136-751">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="a6136-751">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="a6136-752">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-752">AppService</span></span>

* <span data-ttu-id="a6136-753">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="a6136-753">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="a6136-754">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="a6136-754">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="a6136-755">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="a6136-755">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-756">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-756">Backup</span></span>

* <span data-ttu-id="a6136-757">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="a6136-757">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="a6136-758">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="a6136-758">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-759">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-759">Compute</span></span>

* <span data-ttu-id="a6136-760">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="a6136-760">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="a6136-761">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="a6136-761">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="a6136-762">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="a6136-762">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="a6136-763">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="a6136-763">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="a6136-764">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="a6136-764">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="a6136-765">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="a6136-765">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="a6136-766">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-766">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="a6136-767">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="a6136-767">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="a6136-768">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="a6136-768">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="a6136-769">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="a6136-769">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-770">IOT</span><span class="sxs-lookup"><span data-stu-id="a6136-770">IOT</span></span>

* <span data-ttu-id="a6136-771">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="a6136-771">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="a6136-772">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="a6136-772">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="a6136-773">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="a6136-773">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-774">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-774">Key Vault</span></span>

* <span data-ttu-id="a6136-775">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="a6136-775">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="a6136-776">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="a6136-776">NetAppFiles</span></span>

* <span data-ttu-id="a6136-777">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="a6136-777">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="a6136-778">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-778">Network</span></span>

* <span data-ttu-id="a6136-779">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="a6136-779">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="a6136-780">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="a6136-780">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="a6136-781">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="a6136-781">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="a6136-782">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="a6136-782">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="a6136-783">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="a6136-783">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="a6136-784">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="a6136-784">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="a6136-785">Packaging</span><span class="sxs-lookup"><span data-stu-id="a6136-785">Packaging</span></span>

* <span data-ttu-id="a6136-786">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="a6136-786">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="a6136-787">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="a6136-787">Added support for Python 3.8</span></span>
* <span data-ttu-id="a6136-788">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="a6136-788">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-789">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-789">Profile</span></span>

* <span data-ttu-id="a6136-790">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="a6136-790">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="a6136-791">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="a6136-791">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="a6136-792">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="a6136-792">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="a6136-793">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="a6136-793">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="a6136-794">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="a6136-794">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-795">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-795">RBAC</span></span>

* <span data-ttu-id="a6136-796">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a6136-796">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="a6136-797">Redis</span><span class="sxs-lookup"><span data-stu-id="a6136-797">Redis</span></span>

* <span data-ttu-id="a6136-798">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="a6136-798">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="a6136-799">Réservations</span><span class="sxs-lookup"><span data-stu-id="a6136-799">Reservations</span></span>

* <span data-ttu-id="a6136-800">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="a6136-800">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="a6136-801">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="a6136-801">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="a6136-802">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="a6136-802">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="a6136-803">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="a6136-803">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="a6136-804">Rest</span><span class="sxs-lookup"><span data-stu-id="a6136-804">Rest</span></span>
* <span data-ttu-id="a6136-805">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="a6136-805">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-806">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-806">SQL</span></span>

* <span data-ttu-id="a6136-807">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="a6136-807">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-808">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-808">Storage</span></span>

* <span data-ttu-id="a6136-809">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="a6136-809">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="a6136-810">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-810">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="a6136-811">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="a6136-811">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="a6136-812">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="a6136-812">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="a6136-813">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-813">November 4, 2019</span></span>

<span data-ttu-id="a6136-814">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="a6136-814">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-815">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-815">ACR</span></span>

* <span data-ttu-id="a6136-816">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="a6136-816">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="a6136-817">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="a6136-817">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="a6136-818">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="a6136-818">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-819">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-819">AKS</span></span>

* <span data-ttu-id="a6136-820">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="a6136-820">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="a6136-821">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="a6136-821">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="a6136-822">AppConfig</span><span class="sxs-lookup"><span data-stu-id="a6136-822">AppConfig</span></span>

* <span data-ttu-id="a6136-823">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="a6136-823">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="a6136-824">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="a6136-824">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="a6136-825">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="a6136-825">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-826">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-826">AppService</span></span>

* <span data-ttu-id="a6136-827">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="a6136-827">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="a6136-828">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-828">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="a6136-829">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="a6136-829">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="a6136-830">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-830">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="a6136-831">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="a6136-831">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-832">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-832">ARM</span></span>

* <span data-ttu-id="a6136-833">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="a6136-833">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="a6136-834">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="a6136-834">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-835">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-835">Backup</span></span>

* <span data-ttu-id="a6136-836">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="a6136-836">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-837">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-837">Compute</span></span>

* <span data-ttu-id="a6136-838">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="a6136-838">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="a6136-839">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="a6136-839">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="a6136-840">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="a6136-840">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="a6136-841">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="a6136-841">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="a6136-842">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="a6136-842">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="a6136-843">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6136-843">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="a6136-844">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="a6136-844">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="a6136-845">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="a6136-845">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-846">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-846">CosmosDB</span></span>

* <span data-ttu-id="a6136-847">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="a6136-847">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="a6136-848">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="a6136-848">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="a6136-849">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-849">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="a6136-850">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="a6136-850">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="a6136-851">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-851">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="a6136-852">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="a6136-852">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="a6136-853">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-853">Fixed typo in help message</span></span>
* <span data-ttu-id="a6136-854">base de données : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="a6136-854">database: Added deprecation information</span></span>
* <span data-ttu-id="a6136-855">collection : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="a6136-855">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-856">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-856">IoT</span></span>

* <span data-ttu-id="a6136-857">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="a6136-857">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="a6136-858">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="a6136-858">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-859">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-859">Key Vault</span></span>

* <span data-ttu-id="a6136-860">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a6136-860">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="a6136-861">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-861">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="a6136-862">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="a6136-862">NetAppFiles</span></span>

* <span data-ttu-id="a6136-863">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="a6136-863">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="a6136-864">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a6136-864">This new API version includes:</span></span>

    - <span data-ttu-id="a6136-865">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="a6136-865">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="a6136-866">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="a6136-866">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="a6136-867">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="a6136-867">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="a6136-868">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="a6136-868">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="a6136-869">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-869">Network</span></span>

* <span data-ttu-id="a6136-870">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="a6136-870">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="a6136-871">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="a6136-871">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="a6136-872">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="a6136-872">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="a6136-873">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="a6136-873">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="a6136-874">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="a6136-874">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="a6136-875">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="a6136-875">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-876">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-876">Profile</span></span>

* <span data-ttu-id="a6136-877">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-877">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="a6136-878">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="a6136-878">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-879">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-879">RBAC</span></span>

* <span data-ttu-id="a6136-880">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-880">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a6136-881">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a6136-881">ServiceFabric</span></span>

* <span data-ttu-id="a6136-882">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="a6136-882">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-883">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-883">SQL</span></span>

* <span data-ttu-id="a6136-884">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="a6136-884">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-885">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-885">Storage</span></span>

* <span data-ttu-id="a6136-886">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="a6136-886">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="a6136-887">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="a6136-887">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="a6136-888">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-888">October 15, 2019</span></span>

<span data-ttu-id="a6136-889">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="a6136-889">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-890">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-890">AKS</span></span>

* <span data-ttu-id="a6136-891">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-891">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="a6136-892">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-892">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-893">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-893">AMS</span></span>

* <span data-ttu-id="a6136-894">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="a6136-894">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="a6136-895">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="a6136-895">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-896">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-896">AppService</span></span>

* <span data-ttu-id="a6136-897">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="a6136-897">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="a6136-898">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-898">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="a6136-899">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="a6136-899">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-900">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-900">ARM</span></span>

* <span data-ttu-id="a6136-901">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="a6136-901">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-902">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-902">Compute</span></span>

* <span data-ttu-id="a6136-903">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-903">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="a6136-904">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="a6136-904">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="a6136-905">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-905">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="a6136-906">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="a6136-906">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="a6136-907">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-907">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="a6136-908">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="a6136-908">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="a6136-909">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-909">Core</span></span>

* <span data-ttu-id="a6136-910">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a6136-910">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-911">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-911">IoT</span></span>

* <span data-ttu-id="a6136-912">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="a6136-912">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-913">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-913">Monitor</span></span>

* <span data-ttu-id="a6136-914">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="a6136-914">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-915">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-915">Network</span></span>

* <span data-ttu-id="a6136-916">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-916">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="a6136-917">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-917">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-918">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-918">SQL</span></span>

* <span data-ttu-id="a6136-919">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="a6136-919">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-920">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-920">Storage</span></span>

* <span data-ttu-id="a6136-921">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="a6136-921">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="a6136-922">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-922">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="a6136-923">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-923">September 24, 2019</span></span>

<span data-ttu-id="a6136-924">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="a6136-924">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-925">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-925">ACR</span></span>

* <span data-ttu-id="a6136-926">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="a6136-926">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="a6136-927">[CHANGEMENT CASSANT] Renommage du paramètre `--name -n` en `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="a6136-927">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-928">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-928">AKS</span></span>

* <span data-ttu-id="a6136-929">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="a6136-929">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="a6136-930">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="a6136-930">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="a6136-931">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="a6136-931">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-932">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-932">ARM</span></span>

* <span data-ttu-id="a6136-933">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="a6136-933">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-934">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-934">Compute</span></span>

* <span data-ttu-id="a6136-935">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="a6136-935">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="a6136-936">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="a6136-936">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="a6136-937">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-937">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="a6136-938">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="a6136-938">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="a6136-939">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="a6136-939">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-940">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-940">Cosmos DB</span></span>

* <span data-ttu-id="a6136-941">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="a6136-941">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="a6136-942">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="a6136-942">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="a6136-943">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="a6136-943">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6136-944">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a6136-944">EventGrid</span></span>

* <span data-ttu-id="a6136-945">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="a6136-945">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-946">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-946">Key Vault</span></span>

* <span data-ttu-id="a6136-947">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="a6136-947">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-948">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-948">Monitor</span></span>

* <span data-ttu-id="a6136-949">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="a6136-949">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="a6136-950">Stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-950">Policy</span></span>

* <span data-ttu-id="a6136-951">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="a6136-951">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="a6136-952">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="a6136-952">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-953">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-953">Storage</span></span>

* <span data-ttu-id="a6136-954">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="a6136-954">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="a6136-955">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-955">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-956">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-956">ACR</span></span>

* <span data-ttu-id="a6136-957">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="a6136-957">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-958">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-958">AKS</span></span>

* <span data-ttu-id="a6136-959">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a6136-959">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="a6136-960">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-960">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="a6136-961">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-961">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-962">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-962">ARM</span></span>

* <span data-ttu-id="a6136-963">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="a6136-963">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-964">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-964">Batch</span></span>

* <span data-ttu-id="a6136-965">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="a6136-965">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="a6136-966">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="a6136-966">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="a6136-967">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="a6136-967">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="a6136-968">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="a6136-968">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="a6136-969">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="a6136-969">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="a6136-970">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="a6136-970">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="a6136-971">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="a6136-971">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-972">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-972">HDInsight</span></span>

* <span data-ttu-id="a6136-973">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="a6136-973">GA release</span></span>
* <span data-ttu-id="a6136-974">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a6136-974">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-975">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-975">Key Vault</span></span>

* <span data-ttu-id="a6136-976">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-976">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="a6136-977">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-977">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="a6136-978">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-978">Network</span></span>

* <span data-ttu-id="a6136-979">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="a6136-979">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="a6136-980">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="a6136-980">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="a6136-981">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="a6136-981">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="a6136-982">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="a6136-982">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="a6136-983">Stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-983">Policy</span></span>

* <span data-ttu-id="a6136-984">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a6136-984">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="a6136-985">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-985">August 27, 2019</span></span>

<span data-ttu-id="a6136-986">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="a6136-986">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-987">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-987">ACR</span></span>

* <span data-ttu-id="a6136-988">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="a6136-988">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="a6136-989">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="a6136-989">API Management</span></span>

* <span data-ttu-id="a6136-990">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="a6136-990">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-991">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-991">AppService</span></span>

* <span data-ttu-id="a6136-992">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="a6136-992">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="a6136-993">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-993">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-994">Keyvault</span></span>

* <span data-ttu-id="a6136-995">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="a6136-995">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="a6136-996">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-996">Network</span></span>

* <span data-ttu-id="a6136-997">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="a6136-997">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="a6136-998">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="a6136-998">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="a6136-999">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="a6136-999">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="a6136-1000">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1000">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-1001">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-1001">RBAC</span></span>

* <span data-ttu-id="a6136-1002">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-1002">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a6136-1003">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a6136-1003">ServiceFabric</span></span>

* <span data-ttu-id="a6136-1004">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="a6136-1004">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="a6136-1005">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-1005">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="a6136-1006">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="a6136-1006">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="a6136-1007">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a6136-1007">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="a6136-1008">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1008">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="a6136-1009">SignalR</span><span class="sxs-lookup"><span data-stu-id="a6136-1009">SignalR</span></span>

* <span data-ttu-id="a6136-1010">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="a6136-1010">Added new commands:</span></span>
  * <span data-ttu-id="a6136-1011">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="a6136-1011">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="a6136-1012">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="a6136-1012">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="a6136-1013">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="a6136-1013">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="a6136-1014">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1014">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1015">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1015">Storage</span></span>

* <span data-ttu-id="a6136-1016">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="a6136-1016">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="a6136-1017">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1017">August 13, 2019</span></span>

<span data-ttu-id="a6136-1018">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="a6136-1018">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1019">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1019">AppService</span></span>

* <span data-ttu-id="a6136-1020">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="a6136-1020">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1021">BotService</span><span class="sxs-lookup"><span data-stu-id="a6136-1021">BotService</span></span>

* <span data-ttu-id="a6136-1022">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="a6136-1022">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="a6136-1023">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a6136-1023">CognitiveServices</span></span>

* <span data-ttu-id="a6136-1024">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1024">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-1025">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-1025">Cosmos DB</span></span>

* <span data-ttu-id="a6136-1026">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="a6136-1026">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="a6136-1027">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1027">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1028">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1028">HDInsight</span></span>

<span data-ttu-id="a6136-1029">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="a6136-1029">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="a6136-1030">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1030">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="a6136-1031">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="a6136-1031">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="a6136-1032">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="a6136-1032">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="a6136-1033">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="a6136-1033">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="a6136-1034">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="a6136-1034">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="a6136-1035">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1035">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="a6136-1036">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="a6136-1036">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="a6136-1037">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="a6136-1037">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="a6136-1038">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="a6136-1038">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="a6136-1039">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="a6136-1039">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="a6136-1040">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1040">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="a6136-1041">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="a6136-1041">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="a6136-1042">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="a6136-1042">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="a6136-1043">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="a6136-1043">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="a6136-1044">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="a6136-1044">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="a6136-1045">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="a6136-1045">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="a6136-1046">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="a6136-1046">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="a6136-1047">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="a6136-1047">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="a6136-1048">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="a6136-1048">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="a6136-1049">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="a6136-1049">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="a6136-1050">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-1050">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="a6136-1051">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="a6136-1051">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="a6136-1052">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-1052">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-1053">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-1053">Interactive</span></span>

* <span data-ttu-id="a6136-1054">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="a6136-1054">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="a6136-1055">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-1055">Kubernetes</span></span>

* <span data-ttu-id="a6136-1056">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="a6136-1056">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1057">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1057">Network</span></span>

* <span data-ttu-id="a6136-1058">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-1058">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-1059">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-1059">Profile</span></span>

* <span data-ttu-id="a6136-1060">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-1060">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a6136-1061">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a6136-1061">ServiceFabric</span></span>

* <span data-ttu-id="a6136-1062">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="a6136-1062">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="a6136-1063">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="a6136-1063">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1064">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1064">Storage</span></span>

* <span data-ttu-id="a6136-1065">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="a6136-1065">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="a6136-1066">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1066">July 30, 2019</span></span>

<span data-ttu-id="a6136-1067">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="a6136-1067">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1068">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1068">ACR</span></span>

* <span data-ttu-id="a6136-1069">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="a6136-1069">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="a6136-1070">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="a6136-1070">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1071">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1071">Appservice</span></span>

* <span data-ttu-id="a6136-1072">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="a6136-1072">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="a6136-1073">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="a6136-1073">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="a6136-1074">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="a6136-1074">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1075">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1075">Network</span></span>

* <span data-ttu-id="a6136-1076">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="a6136-1076">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="a6136-1077">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="a6136-1077">Fixes #9604.</span></span> <span data-ttu-id="a6136-1078">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a6136-1078">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="a6136-1079">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="a6136-1079">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-1080">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-1080">RBAC</span></span>

* <span data-ttu-id="a6136-1081">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1081">Added `user update` command</span></span>
* <span data-ttu-id="a6136-1082">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a6136-1082">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="a6136-1083">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="a6136-1083">Use replacement argument `--id`</span></span>
* <span data-ttu-id="a6136-1084">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a6136-1084">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1085">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1085">SQL</span></span>

* <span data-ttu-id="a6136-1086">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="a6136-1086">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1087">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1087">Storage</span></span>

* <span data-ttu-id="a6136-1088">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="a6136-1088">Added `storage remove` command</span></span>
* <span data-ttu-id="a6136-1089">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1089">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1090">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1090">VM</span></span>

* <span data-ttu-id="a6136-1091">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="a6136-1091">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="a6136-1092">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1092">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="a6136-1093">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1093">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="a6136-1094">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="a6136-1094">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="a6136-1095">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1095">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="a6136-1096">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1096">July 16, 2019</span></span>

<span data-ttu-id="a6136-1097">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="a6136-1097">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1098">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1098">Appservice</span></span>

* <span data-ttu-id="a6136-1099">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="a6136-1099">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="a6136-1100">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-1100">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="a6136-1101">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1101">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1102">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1102">Core</span></span>

* <span data-ttu-id="a6136-1103">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1103">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-1104">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-1104">Batch</span></span>

* <span data-ttu-id="a6136-1105">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="a6136-1105">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="a6136-1106">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="a6136-1106">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="a6136-1107">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1107">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="a6136-1108">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1108">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a6136-1109">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="a6136-1109">Eventhubs</span></span>

* <span data-ttu-id="a6136-1110">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1110">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1111">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-1111">RDBMS</span></span>

* <span data-ttu-id="a6136-1112">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="a6136-1112">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="a6136-1113">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1113">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="a6136-1114">Relais</span><span class="sxs-lookup"><span data-stu-id="a6136-1114">Relay</span></span>

* <span data-ttu-id="a6136-1115">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="a6136-1115">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="a6136-1116">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1116">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="a6136-1117">Servicebus</span><span class="sxs-lookup"><span data-stu-id="a6136-1117">Servicebus</span></span>

* <span data-ttu-id="a6136-1118">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1118">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1119">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1119">Storage</span></span>

* <span data-ttu-id="a6136-1120">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1120">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="a6136-1121">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="a6136-1121">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="a6136-1122">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1122">July 2, 2019</span></span>

<span data-ttu-id="a6136-1123">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="a6136-1123">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1124">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1124">Core</span></span>

* <span data-ttu-id="a6136-1125">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="a6136-1125">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="a6136-1126">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="a6136-1126">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="a6136-1127">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1127">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1128">ACR</span></span>

* <span data-ttu-id="a6136-1129">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="a6136-1129">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1130">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1130">Appservice</span></span>

* <span data-ttu-id="a6136-1131">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1131">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="a6136-1132">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="a6136-1132">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="a6136-1133">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="a6136-1133">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="a6136-1134">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="a6136-1134">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-1135">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-1135">Cosmos DB</span></span>

* <span data-ttu-id="a6136-1136">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="a6136-1136">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="a6136-1137">DLS</span><span class="sxs-lookup"><span data-stu-id="a6136-1137">DLS</span></span>

* <span data-ttu-id="a6136-1138">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="a6136-1138">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="a6136-1139">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a6136-1139">Feedback</span></span>

* <span data-ttu-id="a6136-1140">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="a6136-1140">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1141">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1141">HDInsight</span></span>

* <span data-ttu-id="a6136-1142">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="a6136-1142">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="a6136-1143">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="a6136-1143">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="a6136-1144">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="a6136-1144">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="a6136-1145">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="a6136-1145">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="a6136-1146">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="a6136-1146">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="a6136-1147">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1147">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="a6136-1148">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="a6136-1148">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="a6136-1149">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="a6136-1149">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="a6136-1150">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1150">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="a6136-1151">Services gérés</span><span class="sxs-lookup"><span data-stu-id="a6136-1151">Managed Services</span></span>

* <span data-ttu-id="a6136-1152">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-1152">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-1153">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-1153">Profile</span></span>
* <span data-ttu-id="a6136-1154">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="a6136-1154">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-1155">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-1155">RBAC</span></span>

* <span data-ttu-id="a6136-1156">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a6136-1156">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="a6136-1157">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="a6136-1157">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="a6136-1158">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="a6136-1158">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="a6136-1159">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="a6136-1159">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1160">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-1160">RDBMS</span></span>

* <span data-ttu-id="a6136-1161">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1161">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1162">SQL</span></span>

* <span data-ttu-id="a6136-1163">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-1163">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1164">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1164">Storage</span></span>

* <span data-ttu-id="a6136-1165">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="a6136-1165">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="a6136-1166">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="a6136-1166">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="a6136-1167">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1167">VM</span></span>

* <span data-ttu-id="a6136-1168">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1168">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="a6136-1169">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1169">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="a6136-1170">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-1170">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="a6136-1171">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="a6136-1171">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="a6136-1172">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1172">June 18, 2019</span></span>

<span data-ttu-id="a6136-1173">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="a6136-1173">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1174">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1174">Core</span></span>

<span data-ttu-id="a6136-1175">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="a6136-1175">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="a6136-1176">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="a6136-1176">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="a6136-1177">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="a6136-1177">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="a6136-1178">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="a6136-1178">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="a6136-1179">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="a6136-1179">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="a6136-1180">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="a6136-1180">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="a6136-1181">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="a6136-1181">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1182">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1182">ACR</span></span>
* <span data-ttu-id="a6136-1183">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="a6136-1183">Added 'acr check-health' command</span></span>
* <span data-ttu-id="a6136-1184">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="a6136-1184">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1185">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1185">ACS</span></span>
* <span data-ttu-id="a6136-1186">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-1186">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1187">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1187">AMS</span></span>
* <span data-ttu-id="a6136-1188">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="a6136-1188">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1189">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1189">AppService</span></span>
* <span data-ttu-id="a6136-1190">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="a6136-1190">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="a6136-1191">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-1191">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="a6136-1192">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="a6136-1192">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="a6136-1193">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1193">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="a6136-1194">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="a6136-1194">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="a6136-1195">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="a6136-1195">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-1196">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-1196">Batch</span></span>
* <span data-ttu-id="a6136-1197">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="a6136-1197">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-1198">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-1198">BatchAI</span></span>
* <span data-ttu-id="a6136-1199">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="a6136-1199">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1200">BotService</span><span class="sxs-lookup"><span data-stu-id="a6136-1200">BotService</span></span>
* <span data-ttu-id="a6136-1201">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="a6136-1201">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1202">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1202">CosmosDB</span></span>
* <span data-ttu-id="a6136-1203">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="a6136-1203">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="a6136-1204">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="a6136-1204">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="a6136-1205">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="a6136-1205">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="a6136-1206">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="a6136-1206">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6136-1207">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a6136-1207">EventGrid</span></span>
* <span data-ttu-id="a6136-1208">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="a6136-1208">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="a6136-1209">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="a6136-1209">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="a6136-1210">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="a6136-1210">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="a6136-1211">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="a6136-1211">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="a6136-1212">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1212">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1213">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1213">HDInsight</span></span>
* <span data-ttu-id="a6136-1214">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1214">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-1215">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-1215">IoT</span></span>
* <span data-ttu-id="a6136-1216">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="a6136-1216">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="a6136-1217">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="a6136-1217">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1218">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1218">Network</span></span>
* <span data-ttu-id="a6136-1219">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="a6136-1219">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="a6136-1220">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="a6136-1220">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="a6136-1221">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="a6136-1221">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="a6136-1222">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="a6136-1222">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1223">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1223">Resource</span></span>
* <span data-ttu-id="a6136-1224">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="a6136-1224">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="a6136-1225">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="a6136-1225">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="a6136-1226">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a6136-1226">ServiceBus</span></span>
* <span data-ttu-id="a6136-1227">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="a6136-1227">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1228">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1228">SQL</span></span>
* <span data-ttu-id="a6136-1229">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a6136-1229">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="a6136-1230">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="a6136-1230">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="a6136-1231">SQLVm</span><span class="sxs-lookup"><span data-stu-id="a6136-1231">SQLVm</span></span>
* <span data-ttu-id="a6136-1232">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="a6136-1232">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="a6136-1233">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1233">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1234">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1234">Storage</span></span>
* <span data-ttu-id="a6136-1235">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="a6136-1235">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="a6136-1236">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-1236">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1237">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1237">VM</span></span>
* <span data-ttu-id="a6136-1238">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1238">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="a6136-1239">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1239">June 4, 2019</span></span>

<span data-ttu-id="a6136-1240">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="a6136-1240">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1241">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1241">Core</span></span>
* <span data-ttu-id="a6136-1242">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="a6136-1242">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1243">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1243">ACR</span></span>
* <span data-ttu-id="a6136-1244">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="a6136-1244">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1245">ACS</span></span>
* <span data-ttu-id="a6136-1246">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-1246">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="a6136-1247">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="a6136-1247">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-1248">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-1248">Batch</span></span>
* <span data-ttu-id="a6136-1249">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="a6136-1249">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-1250">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-1250">IoT</span></span>
* <span data-ttu-id="a6136-1251">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="a6136-1251">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1252">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1252">Network</span></span>
* <span data-ttu-id="a6136-1253">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="a6136-1253">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="a6136-1254">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1254">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="a6136-1255">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1255">Resource</span></span>
* <span data-ttu-id="a6136-1256">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="a6136-1256">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1257">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1257">Role</span></span>
* <span data-ttu-id="a6136-1258">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-1258">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-1259">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-1259">Compute</span></span>
* <span data-ttu-id="a6136-1260">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="a6136-1260">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="a6136-1261">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1261">May 21, 2019</span></span>

<span data-ttu-id="a6136-1262">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="a6136-1262">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1263">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1263">Core</span></span>
* <span data-ttu-id="a6136-1264">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="a6136-1264">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="a6136-1265">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="a6136-1265">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="a6136-1266">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="a6136-1266">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1267">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1267">ACR</span></span>
* <span data-ttu-id="a6136-1268">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="a6136-1268">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1269">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1269">ACS</span></span>
* <span data-ttu-id="a6136-1270">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="a6136-1270">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1271">AppService</span></span>
* <span data-ttu-id="a6136-1272">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="a6136-1272">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="a6136-1273">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="a6136-1273">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="a6136-1274">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="a6136-1274">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="a6136-1275">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="a6136-1275">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="a6136-1276">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-1276">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="a6136-1277">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="a6136-1277">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="a6136-1278">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1278">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1279">BotService</span><span class="sxs-lookup"><span data-stu-id="a6136-1279">BotService</span></span>
* <span data-ttu-id="a6136-1280">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-1280">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="a6136-1281">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-1281">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-1282">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-1282">Consumption</span></span>
* <span data-ttu-id="a6136-1283">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-1283">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-1284">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-1284">IoT</span></span>
* <span data-ttu-id="a6136-1285">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="a6136-1285">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1286">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1286">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="a6136-1288">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="a6136-1288">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="a6136-1289">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="a6136-1289">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1290">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-1290">RDBMS</span></span>
* <span data-ttu-id="a6136-1291">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="a6136-1291">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-1292">RBAC</span><span class="sxs-lookup"><span data-stu-id="a6136-1292">RBAC</span></span>
* <span data-ttu-id="a6136-1293">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="a6136-1293">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1294">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1294">Storage</span></span>
* <span data-ttu-id="a6136-1295">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1295">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="a6136-1296">Calcul</span><span class="sxs-lookup"><span data-stu-id="a6136-1296">Compute</span></span>
* <span data-ttu-id="a6136-1297">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1297">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="a6136-1298">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="a6136-1298">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="a6136-1299">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="a6136-1299">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="a6136-1300">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1300">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="a6136-1301">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1301">May 6, 2019</span></span>

<span data-ttu-id="a6136-1302">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="a6136-1302">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1303">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1303">ACS</span></span>
* <span data-ttu-id="a6136-1304">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="a6136-1304">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="a6136-1305">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="a6136-1305">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="a6136-1306">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1306">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="a6136-1307">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-1307">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1308">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1308">Appservice</span></span>
* <span data-ttu-id="a6136-1309">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="a6136-1309">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="a6136-1310">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="a6136-1310">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="a6136-1311">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-1311">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="a6136-1312">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="a6136-1312">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="a6136-1313">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-1313">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="a6136-1314">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="a6136-1314">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="a6136-1315">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="a6136-1315">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="a6136-1316">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="a6136-1316">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="a6136-1317">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-1317">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="a6136-1318">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="a6136-1318">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-1319">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-1319">Batch</span></span>
* <span data-ttu-id="a6136-1320">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="a6136-1320">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1321">Botservice</span><span class="sxs-lookup"><span data-stu-id="a6136-1321">Botservice</span></span>
* <span data-ttu-id="a6136-1322">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="a6136-1322">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="a6136-1323">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="a6136-1323">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="a6136-1324">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="a6136-1324">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="a6136-1325">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1325">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="a6136-1326">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1326">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="a6136-1327">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-1327">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="a6136-1328">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1328">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="a6136-1329">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="a6136-1329">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="a6136-1330">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-1330">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="a6136-1331">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="a6136-1331">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="a6136-1332">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="a6136-1332">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="a6136-1333">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="a6136-1333">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="a6136-1334">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="a6136-1334">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="a6136-1335">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="a6136-1335">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="a6136-1336">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1336">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="a6136-1337">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="a6136-1337">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="a6136-1338">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="a6136-1338">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="a6136-1339">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="a6136-1339">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="a6136-1340">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a6136-1340">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="a6136-1341">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="a6136-1341">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="a6136-1342">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="a6136-1342">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="a6136-1343">Configurer</span><span class="sxs-lookup"><span data-stu-id="a6136-1343">Configure</span></span>
* <span data-ttu-id="a6136-1344">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="a6136-1344">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a6136-1345">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="a6136-1345">Eventhubs</span></span>
* <span data-ttu-id="a6136-1346">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1346">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="a6136-1347">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1347">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1348">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1348">Network</span></span>
* <span data-ttu-id="a6136-1349">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1349">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="a6136-1350">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-1350">Policy Insights</span></span>
* <span data-ttu-id="a6136-1351">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1351">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1352">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1352">Role</span></span>
* <span data-ttu-id="a6136-1353">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1353">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6136-1354">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-1354">Service Bus</span></span>
* <span data-ttu-id="a6136-1355">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1355">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="a6136-1356">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1356">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="a6136-1357">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="a6136-1357">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1358">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1358">SQL</span></span>
* <span data-ttu-id="a6136-1359">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1359">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1360">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1360">VM</span></span>
* <span data-ttu-id="a6136-1361">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="a6136-1361">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="a6136-1362">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="a6136-1362">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="a6136-1363">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1363">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="a6136-1364">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="a6136-1364">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="a6136-1365">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="a6136-1365">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="a6136-1366">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1366">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="a6136-1367">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1367">April 23, 2019</span></span>

<span data-ttu-id="a6136-1368">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="a6136-1368">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1369">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1369">ACS</span></span>
* <span data-ttu-id="a6136-1370">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="a6136-1370">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="a6136-1371">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="a6136-1371">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1372">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1372">AMS</span></span>
* <span data-ttu-id="a6136-1373">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="a6136-1373">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1374">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1374">AppService</span></span>
* <span data-ttu-id="a6136-1375">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="a6136-1375">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="a6136-1376">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="a6136-1376">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="a6136-1377">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="a6136-1377">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="a6136-1378">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="a6136-1378">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="a6136-1379">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="a6136-1379">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="a6136-1380">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-1380">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="a6136-1381">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="a6136-1381">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="a6136-1382">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="a6136-1382">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="a6136-1383">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="a6136-1383">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="a6136-1384">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-1384">Deployment Manager</span></span>
* <span data-ttu-id="a6136-1385">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="a6136-1385">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="a6136-1386">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-1386">Lab</span></span>
* <span data-ttu-id="a6136-1387">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="a6136-1387">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1388">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1388">Network</span></span>
* <span data-ttu-id="a6136-1389">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="a6136-1389">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1390">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1390">Resource</span></span>
* <span data-ttu-id="a6136-1391">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="a6136-1391">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="a6136-1392">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="a6136-1392">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="a6136-1393">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1393">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="a6136-1394">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-1394">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1395">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1395">SQL</span></span>
* <span data-ttu-id="a6136-1396">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="a6136-1396">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="a6136-1397">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1397">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="a6136-1398">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1398">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="a6136-1399">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1399">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1400">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1400">Storage</span></span>
* <span data-ttu-id="a6136-1401">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="a6136-1401">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1402">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1402">VM</span></span>
* <span data-ttu-id="a6136-1403">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="a6136-1403">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="a6136-1404">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="a6136-1404">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="a6136-1405">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="a6136-1405">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="a6136-1406">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1406">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1407">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1407">Core</span></span>
* <span data-ttu-id="a6136-1408">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-1408">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1409">ACR</span></span>
* <span data-ttu-id="a6136-1410">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="a6136-1410">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1411">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1411">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="a6136-1414">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1414">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="a6136-1415">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1415">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1416">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1416">AppService</span></span>
* <span data-ttu-id="a6136-1417">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-1417">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="a6136-1418">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1418">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="a6136-1419">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1419">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="a6136-1420">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a6136-1420">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="a6136-1421">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-1421">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="a6136-1422">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="a6136-1422">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="a6136-1423">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="a6136-1423">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-1424">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-1424">CDN</span></span>
* <span data-ttu-id="a6136-1425">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="a6136-1425">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="a6136-1426">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a6136-1426">Feedback</span></span>
* <span data-ttu-id="a6136-1427">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="a6136-1427">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="a6136-1428">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="a6136-1428">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="a6136-1429">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="a6136-1429">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1430">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1430">Monitor</span></span>
* <span data-ttu-id="a6136-1431">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1431">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="a6136-1432">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1432">Network</span></span>
* <span data-ttu-id="a6136-1433">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="a6136-1433">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="a6136-1434">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-1434">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="a6136-1435">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="a6136-1435">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="a6136-1436">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1436">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="a6136-1437">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="a6136-1437">PrivateDNS</span></span>
* <span data-ttu-id="a6136-1438">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="a6136-1438">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1439">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1439">Resource</span></span>
* <span data-ttu-id="a6136-1440">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1440">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1441">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1441">Role</span></span>
* <span data-ttu-id="a6136-1442">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-1442">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="a6136-1443">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-1443">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1444">SQL</span></span>
* <span data-ttu-id="a6136-1445">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="a6136-1445">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1446">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1446">Storage</span></span>
* <span data-ttu-id="a6136-1447">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-1447">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="a6136-1448">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="a6136-1448">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="a6136-1449">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="a6136-1449">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="a6136-1450">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="a6136-1450">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="a6136-1451">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1451">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="a6136-1452">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1452">Core</span></span>
* <span data-ttu-id="a6136-1453">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="a6136-1453">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="a6136-1454">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="a6136-1454">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="a6136-1455">Cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-1455">Cloud</span></span>
* <span data-ttu-id="a6136-1456">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="a6136-1456">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1457">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1457">ACR</span></span>
* <span data-ttu-id="a6136-1458">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="a6136-1458">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="a6136-1459">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1459">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="a6136-1460">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="a6136-1460">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="a6136-1461">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="a6136-1461">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1462">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1462">AppService</span></span>
* <span data-ttu-id="a6136-1463">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="a6136-1463">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="a6136-1464">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="a6136-1464">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="a6136-1465">Service BOT</span><span class="sxs-lookup"><span data-stu-id="a6136-1465">BOT Service</span></span>
* <span data-ttu-id="a6136-1466">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="a6136-1466">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="a6136-1467">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-1467">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="a6136-1468">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="a6136-1468">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="a6136-1469">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a6136-1469">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-1470">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-1470">CDN</span></span>
* <span data-ttu-id="a6136-1471">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1471">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="a6136-1472">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1472">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="a6136-1473">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="a6136-1473">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a6136-1474">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="a6136-1474">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1475">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a6136-1475">Cosmosdb</span></span>
* <span data-ttu-id="a6136-1476">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="a6136-1476">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="a6136-1477">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-1477">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-1478">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-1478">Interactive</span></span>
* <span data-ttu-id="a6136-1479">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="a6136-1479">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1480">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1480">Monitor</span></span>
* <span data-ttu-id="a6136-1481">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1481">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1482">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1482">Network</span></span>
* <span data-ttu-id="a6136-1483">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="a6136-1483">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-1484">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-1484">Profile</span></span>
* <span data-ttu-id="a6136-1485">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="a6136-1485">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="a6136-1486">Postgres</span><span class="sxs-lookup"><span data-stu-id="a6136-1486">Postgres</span></span> 
* <span data-ttu-id="a6136-1487">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="a6136-1487">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="a6136-1488">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="a6136-1488">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1489">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1489">Resource</span></span>
* <span data-ttu-id="a6136-1490">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1490">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="a6136-1491">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="a6136-1491">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="a6136-1492">Graph</span><span class="sxs-lookup"><span data-stu-id="a6136-1492">Graph</span></span>
* <span data-ttu-id="a6136-1493">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="a6136-1493">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="a6136-1494">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="a6136-1494">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="a6136-1495">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="a6136-1495">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="a6136-1496">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-1496">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="a6136-1497">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-1497">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1498">storage</span><span class="sxs-lookup"><span data-stu-id="a6136-1498">storage</span></span>
* <span data-ttu-id="a6136-1499">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="a6136-1499">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="a6136-1500">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="a6136-1500">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="a6136-1501">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="a6136-1501">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="a6136-1502">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="a6136-1502">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1503">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1503">VM</span></span>
* <span data-ttu-id="a6136-1504">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1504">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="a6136-1505">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1505">March 12, 2019</span></span>

<span data-ttu-id="a6136-1506">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="a6136-1506">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1507">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1507">Core</span></span>

* <span data-ttu-id="a6136-1508">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="a6136-1508">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1509">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1509">ACR</span></span>

* <span data-ttu-id="a6136-1510">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="a6136-1510">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1511">ACS</span></span>

* <span data-ttu-id="a6136-1512">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="a6136-1512">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="a6136-1513">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1513">AppService</span></span>

* <span data-ttu-id="a6136-1514">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="a6136-1514">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="a6136-1515">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1515">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="a6136-1516">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-1516">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="a6136-1517">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="a6136-1517">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1518">Botservice</span><span class="sxs-lookup"><span data-stu-id="a6136-1518">Botservice</span></span>

* <span data-ttu-id="a6136-1519">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a6136-1519">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a6136-1520">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a6136-1520">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a6136-1521">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1521">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="a6136-1522">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="a6136-1522">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="a6136-1523">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1523">Container</span></span>

* <span data-ttu-id="a6136-1524">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1524">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="a6136-1525">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a6136-1525">EventHub</span></span>

* <span data-ttu-id="a6136-1526">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="a6136-1526">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="a6136-1527">Rechercher</span><span class="sxs-lookup"><span data-stu-id="a6136-1527">Find</span></span>

* <span data-ttu-id="a6136-1528">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a6136-1528">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1529">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1529">HDInsight</span></span>

* <span data-ttu-id="a6136-1530">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="a6136-1530">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1531">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1531">Network</span></span>

* <span data-ttu-id="a6136-1532">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="a6136-1532">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1533">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6136-1533">Rdbms</span></span>

* <span data-ttu-id="a6136-1534">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="a6136-1534">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1535">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1535">Role</span></span>

* <span data-ttu-id="a6136-1536">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="a6136-1536">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="a6136-1537">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="a6136-1537">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6136-1538">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-1538">Service Fabric</span></span>

* <span data-ttu-id="a6136-1539">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="a6136-1539">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="a6136-1540">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1540">February 26, 2019</span></span>

<span data-ttu-id="a6136-1541">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="a6136-1541">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1542">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1542">Core</span></span>

* <span data-ttu-id="a6136-1543">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="a6136-1543">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1544">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1544">ACR</span></span>

* <span data-ttu-id="a6136-1545">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1545">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="a6136-1546">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="a6136-1546">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1547">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1547">ACS</span></span>

* <span data-ttu-id="a6136-1548">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="a6136-1548">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1549">AppService</span></span>

* <span data-ttu-id="a6136-1550">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="a6136-1550">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-1551">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-1551">Batch</span></span>
* <span data-ttu-id="a6136-1552">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="a6136-1552">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="a6136-1553">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="a6136-1553">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="a6136-1554">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="a6136-1554">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="a6136-1555">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="a6136-1555">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="a6136-1556">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="a6136-1556">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="a6136-1557">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="a6136-1557">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1558">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1558">CosmosDB</span></span>

* <span data-ttu-id="a6136-1559">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-1559">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="a6136-1560">Kusto</span><span class="sxs-lookup"><span data-stu-id="a6136-1560">Kusto</span></span>

* <span data-ttu-id="a6136-1561">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="a6136-1561">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1562">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1562">Network</span></span>

* <span data-ttu-id="a6136-1563">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1563">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="a6136-1564">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="a6136-1564">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="a6136-1565">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="a6136-1565">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="a6136-1566">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1566">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="a6136-1567">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1567">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="a6136-1568">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1568">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="a6136-1569">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="a6136-1569">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1570">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1570">Resource</span></span>

* <span data-ttu-id="a6136-1571">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-1571">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="a6136-1572">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1572">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="a6136-1573">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1573">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="a6136-1574">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1574">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="a6136-1575">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-1575">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1576">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1576">Role</span></span>

* <span data-ttu-id="a6136-1577">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1577">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1578">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1578">VM</span></span>

* <span data-ttu-id="a6136-1579">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="a6136-1579">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="a6136-1580">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1580">February 12, 2019</span></span>

<span data-ttu-id="a6136-1581">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="a6136-1581">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1582">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1582">Core</span></span>

* <span data-ttu-id="a6136-1583">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-1583">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="a6136-1584">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="a6136-1584">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1585">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1585">ACR</span></span>
* <span data-ttu-id="a6136-1586">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="a6136-1586">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="a6136-1587">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-1587">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1588">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1588">ACS</span></span>
* <span data-ttu-id="a6136-1589">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1589">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="a6136-1590">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="a6136-1590">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="a6136-1591">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a6136-1591">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1592">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1592">AMS</span></span>
* <span data-ttu-id="a6136-1593">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1593">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="a6136-1594">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1594">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1595">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1595">Appservice</span></span>
* <span data-ttu-id="a6136-1596">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1596">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="a6136-1597">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="a6136-1597">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="a6136-1598">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1598">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="a6136-1599">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="a6136-1599">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="a6136-1600">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="a6136-1600">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1601">Botservice</span><span class="sxs-lookup"><span data-stu-id="a6136-1601">Botservice</span></span>
* <span data-ttu-id="a6136-1602">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="a6136-1602">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="a6136-1603">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="a6136-1603">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="a6136-1604">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1604">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="a6136-1605">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-1605">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="a6136-1606">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="a6136-1606">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="a6136-1607">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="a6136-1607">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="a6136-1608">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="a6136-1608">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="a6136-1609">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="a6136-1609">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="a6136-1610">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="a6136-1610">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="a6136-1611">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="a6136-1611">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-1612">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-1612">Key Vault</span></span>
* <span data-ttu-id="a6136-1613">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="a6136-1613">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1614">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1614">Monitor</span></span>
* <span data-ttu-id="a6136-1615">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="a6136-1615">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1616">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1616">Network</span></span>
* <span data-ttu-id="a6136-1617">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="a6136-1617">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="a6136-1618">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a6136-1618">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="a6136-1619">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-1619">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="a6136-1620">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1620">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a6136-1621">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-1621">Policy Insights</span></span>
* <span data-ttu-id="a6136-1622">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-1622">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1623">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-1623">RDBMS</span></span>
* <span data-ttu-id="a6136-1624">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-1624">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="a6136-1625">Redis</span><span class="sxs-lookup"><span data-stu-id="a6136-1625">Redis</span></span>
* <span data-ttu-id="a6136-1626">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="a6136-1626">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="a6136-1627">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="a6136-1627">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="a6136-1628">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="a6136-1628">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="a6136-1629">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="a6136-1629">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="a6136-1630">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="a6136-1630">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="a6136-1631">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="a6136-1631">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="a6136-1632">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="a6136-1632">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1633">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1633">Role</span></span>
* <span data-ttu-id="a6136-1634">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="a6136-1634">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="a6136-1635">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1635">SQL VM</span></span>
* <span data-ttu-id="a6136-1636">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="a6136-1636">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1637">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1637">VM</span></span>
* <span data-ttu-id="a6136-1638">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="a6136-1638">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="a6136-1639">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1639">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="a6136-1640">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="a6136-1640">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="a6136-1641">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="a6136-1641">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="a6136-1642">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1642">January 31, 2019</span></span>

<span data-ttu-id="a6136-1643">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="a6136-1643">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1644">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1644">Core</span></span>

* <span data-ttu-id="a6136-1645">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="a6136-1645">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="a6136-1646">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1646">January 28, 2019</span></span>

<span data-ttu-id="a6136-1647">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="a6136-1647">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1648">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1648">ACR</span></span>
* <span data-ttu-id="a6136-1649">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="a6136-1649">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1650">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1650">ACS</span></span>
* <span data-ttu-id="a6136-1651">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="a6136-1651">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a6136-1652">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="a6136-1652">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="a6136-1653">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="a6136-1653">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1654">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1654">AMS</span></span>
* <span data-ttu-id="a6136-1655">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="a6136-1655">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="a6136-1656">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="a6136-1656">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1657">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1657">Appservice</span></span>
* <span data-ttu-id="a6136-1658">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1658">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="a6136-1659">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="a6136-1659">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="a6136-1660">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="a6136-1660">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="a6136-1661">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1661">Container</span></span>
* <span data-ttu-id="a6136-1662">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="a6136-1662">Added `container start` command</span></span>
* <span data-ttu-id="a6136-1663">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1663">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6136-1664">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a6136-1664">EventGrid</span></span>
* <span data-ttu-id="a6136-1665">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1665">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="a6136-1666">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="a6136-1666">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="a6136-1667">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="a6136-1667">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="a6136-1668">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="a6136-1668">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="a6136-1669">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="a6136-1669">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1670">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1670">HDInsight</span></span>
* <span data-ttu-id="a6136-1671">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1671">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="a6136-1672">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="a6136-1672">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="a6136-1673">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1673">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="a6136-1674">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1674">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="a6136-1675">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="a6136-1675">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="a6136-1676">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1676">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-1677">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-1677">IoT</span></span>
* <span data-ttu-id="a6136-1678">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="a6136-1678">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="a6136-1679">Kusto</span><span class="sxs-lookup"><span data-stu-id="a6136-1679">Kusto</span></span>
* <span data-ttu-id="a6136-1680">Préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-1680">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1681">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1681">Monitor</span></span>
* <span data-ttu-id="a6136-1682">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-1682">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-1683">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-1683">Profile</span></span>
* <span data-ttu-id="a6136-1684">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="a6136-1684">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1685">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1685">Network</span></span>
* <span data-ttu-id="a6136-1686">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="a6136-1686">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="a6136-1687">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="a6136-1687">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1688">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1688">Resource</span></span>
* <span data-ttu-id="a6136-1689">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1689">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="a6136-1690">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1690">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="a6136-1691">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1691">SQL Virtual Machine</span></span>
* <span data-ttu-id="a6136-1692">Préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-1692">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1693">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1693">Storage</span></span>
* <span data-ttu-id="a6136-1694">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="a6136-1694">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="a6136-1695">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="a6136-1695">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1696">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1696">VM</span></span>
* <span data-ttu-id="a6136-1697">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="a6136-1697">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="a6136-1698">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a6136-1698">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="a6136-1699">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a6136-1699">January 15, 2019</span></span>

<span data-ttu-id="a6136-1700">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="a6136-1700">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1701">ACR</span></span>
* <span data-ttu-id="a6136-1702">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1702">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="a6136-1703">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-1703">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="a6136-1704">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="a6136-1704">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="a6136-1705">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1705">ACS</span></span>
* <span data-ttu-id="a6136-1706">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="a6136-1706">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1707">Appservice</span></span>
* <span data-ttu-id="a6136-1708">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="a6136-1708">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="a6136-1709">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-1709">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="a6136-1710">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-1710">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="a6136-1711">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="a6136-1711">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1712">Botservice</span><span class="sxs-lookup"><span data-stu-id="a6136-1712">Botservice</span></span>
* <span data-ttu-id="a6136-1713">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1713">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="a6136-1714">Configurer</span><span class="sxs-lookup"><span data-stu-id="a6136-1714">Configure</span></span>
* <span data-ttu-id="a6136-1715">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="a6136-1715">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1716">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1716">CosmosDB</span></span>
* <span data-ttu-id="a6136-1717">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="a6136-1717">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1718">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1718">HDInsight</span></span>
* <span data-ttu-id="a6136-1719">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="a6136-1719">Added commands for managing applications</span></span>
* <span data-ttu-id="a6136-1720">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="a6136-1720">Added commands for managing script actions</span></span>
* <span data-ttu-id="a6136-1721">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="a6136-1721">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="a6136-1722">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="a6136-1722">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="a6136-1723">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1723">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1724">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1724">Network</span></span>
* <span data-ttu-id="a6136-1725">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1725">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="a6136-1726">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="a6136-1726">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="a6136-1727">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1727">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="a6136-1728">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-1728">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1729">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1729">Role</span></span>
* <span data-ttu-id="a6136-1730">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1730">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="a6136-1731">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="a6136-1731">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="a6136-1732">Sécurité</span><span class="sxs-lookup"><span data-stu-id="a6136-1732">Security</span></span>
* <span data-ttu-id="a6136-1733">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-1733">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1734">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1734">Storage</span></span>
* <span data-ttu-id="a6136-1735">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="a6136-1735">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="a6136-1736">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="a6136-1736">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="a6136-1737">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="a6136-1737">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="a6136-1738">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="a6136-1738">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="a6136-1739">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="a6136-1739">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1740">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1740">VM</span></span>
* <span data-ttu-id="a6136-1741">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="a6136-1741">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="a6136-1742">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1742">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6136-1743">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="a6136-1743">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="a6136-1744">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="a6136-1744">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="a6136-1745">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1745">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="a6136-1746">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-1746">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="a6136-1747">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1747">December 20, 2018</span></span>

<span data-ttu-id="a6136-1748">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="a6136-1748">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="a6136-1749">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1749">Appservice</span></span>
* <span data-ttu-id="a6136-1750">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a6136-1750">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="a6136-1751">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="a6136-1751">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="a6136-1752">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-1752">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a6136-1753">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a6136-1753">IoTCentral</span></span>
* <span data-ttu-id="a6136-1754">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-1754">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1755">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1755">Role</span></span>
* <span data-ttu-id="a6136-1756">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="a6136-1756">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1757">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1757">SQL</span></span>
* <span data-ttu-id="a6136-1758">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="a6136-1758">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1759">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1759">VM</span></span>
* <span data-ttu-id="a6136-1760">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1760">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="a6136-1761">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1761">December 18, 2018</span></span>

<span data-ttu-id="a6136-1762">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="a6136-1762">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="a6136-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1763">ACR</span></span>
* <span data-ttu-id="a6136-1764">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="a6136-1764">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="a6136-1765">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="a6136-1765">Condensed the table layout for task list</span></span>
* <span data-ttu-id="a6136-1766">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a6136-1766">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1767">ACS</span></span>
* <span data-ttu-id="a6136-1768">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="a6136-1768">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a6136-1769">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1769">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="a6136-1770">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1770">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="a6136-1771">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="a6136-1771">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="a6136-1772">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-1772">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="a6136-1773">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="a6136-1773">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1774">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1774">Appservice</span></span>
* <span data-ttu-id="a6136-1775">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="a6136-1775">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="a6136-1776">Botservice</span><span class="sxs-lookup"><span data-stu-id="a6136-1776">Botservice</span></span>
* <span data-ttu-id="a6136-1777">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="a6136-1777">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="a6136-1778">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="a6136-1778">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="a6136-1779">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="a6136-1779">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="a6136-1780">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="a6136-1780">Reduced Kudu network calls</span></span>
* <span data-ttu-id="a6136-1781">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="a6136-1781">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-1782">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-1782">Consumption</span></span>
* <span data-ttu-id="a6136-1783">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="a6136-1783">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1784">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1784">CosmosDB</span></span>
* <span data-ttu-id="a6136-1785">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="a6136-1785">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="a6136-1786">Cartes</span><span class="sxs-lookup"><span data-stu-id="a6136-1786">Maps</span></span>
* <span data-ttu-id="a6136-1787">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1787">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1788">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1788">Network</span></span>
* <span data-ttu-id="a6136-1789">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="a6136-1789">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="a6136-1790">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-1790">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1791">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1791">Resource</span></span>
* <span data-ttu-id="a6136-1792">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1792">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="a6136-1793">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1793">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1794">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1794">Storage</span></span>
*  <span data-ttu-id="a6136-1795">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1795">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1796">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1796">VM</span></span>
* <span data-ttu-id="a6136-1797">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="a6136-1797">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="a6136-1798">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1798">December 4, 2018</span></span>

<span data-ttu-id="a6136-1799">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="a6136-1799">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="a6136-1800">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1800">Core</span></span>
* <span data-ttu-id="a6136-1801">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="a6136-1801">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="a6136-1802">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="a6136-1802">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1803">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1803">Appservice</span></span>
* <span data-ttu-id="a6136-1804">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="a6136-1804">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="a6136-1805">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="a6136-1805">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1806">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1806">Network</span></span>
* <span data-ttu-id="a6136-1807">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="a6136-1807">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1808">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1808">Role</span></span>
* <span data-ttu-id="a6136-1809">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="a6136-1809">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="a6136-1810">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1810">VM</span></span>
* <span data-ttu-id="a6136-1811">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="a6136-1811">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="a6136-1812">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="a6136-1812">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="a6136-1813">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="a6136-1813">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="a6136-1814">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="a6136-1814">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="a6136-1815">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1815">November 20, 2018</span></span>

<span data-ttu-id="a6136-1816">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="a6136-1816">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="a6136-1817">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1817">Core</span></span>
* <span data-ttu-id="a6136-1818">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="a6136-1818">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1819">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1819">ACR</span></span>
* <span data-ttu-id="a6136-1820">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="a6136-1820">Added context token to task step</span></span>
* <span data-ttu-id="a6136-1821">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="a6136-1821">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="a6136-1822">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="a6136-1822">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1823">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1823">Appservice</span></span>
* <span data-ttu-id="a6136-1824">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="a6136-1824">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="a6136-1825">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1825">Updated the default `node_version`.</span></span> <span data-ttu-id="a6136-1826">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="a6136-1826">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="a6136-1827">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-1827">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="a6136-1828">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="a6136-1828">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a6136-1829">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a6136-1829">IotCentral</span></span>
* <span data-ttu-id="a6136-1830">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6136-1830">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-1831">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-1831">KeyVault</span></span>
* <span data-ttu-id="a6136-1832">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="a6136-1832">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1833">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1833">Network</span></span>
* <span data-ttu-id="a6136-1834">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="a6136-1834">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="a6136-1835">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1835">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="a6136-1836">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1836">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="a6136-1837">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="a6136-1837">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1838">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6136-1838">Rdbms</span></span>
* <span data-ttu-id="a6136-1839">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="a6136-1839">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="a6136-1840">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="a6136-1840">Rbac</span></span>
* <span data-ttu-id="a6136-1841">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1841">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="a6136-1842">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="a6136-1842">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="a6136-1843">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1843">Storage</span></span>
* <span data-ttu-id="a6136-1844">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1844">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="a6136-1845">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="a6136-1845">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="a6136-1846">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="a6136-1846">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="a6136-1847">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="a6136-1847">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1848">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1848">VM</span></span>
* <span data-ttu-id="a6136-1849">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="a6136-1849">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="a6136-1850">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="a6136-1850">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="a6136-1851">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="a6136-1851">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="a6136-1852">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="a6136-1852">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="a6136-1853">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1853">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="a6136-1854">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-1854">Added `snapshot wait` command</span></span>
* <span data-ttu-id="a6136-1855">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-1855">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="a6136-1856">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1856">November 6, 2018</span></span>

<span data-ttu-id="a6136-1857">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="a6136-1857">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1858">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1858">Core</span></span>
* <span data-ttu-id="a6136-1859">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="a6136-1859">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1860">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1860">ACR</span></span>
* <span data-ttu-id="a6136-1861">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="a6136-1861">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="a6136-1862">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="a6136-1862">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1863">ACS</span></span>
* <span data-ttu-id="a6136-1864">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-1864">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="a6136-1865">Advisor</span><span class="sxs-lookup"><span data-stu-id="a6136-1865">Advisor</span></span>
* <span data-ttu-id="a6136-1866">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="a6136-1866">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-1867">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-1867">AMS</span></span>
* <span data-ttu-id="a6136-1868">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="a6136-1868">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="a6136-1869">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="a6136-1869">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="a6136-1870">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1870">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="a6136-1871">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="a6136-1871">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="a6136-1872">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="a6136-1872">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="a6136-1873">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="a6136-1873">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="a6136-1874">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="a6136-1874">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="a6136-1875">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="a6136-1875">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="a6136-1876">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="a6136-1876">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="a6136-1877">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="a6136-1877">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="a6136-1878">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-1878">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="a6136-1879">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1879">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="a6136-1880">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="a6136-1880">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="a6136-1881">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="a6136-1881">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="a6136-1882">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="a6136-1882">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="a6136-1883">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="a6136-1883">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="a6136-1884">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="a6136-1884">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-1885">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-1885">AppService</span></span>
* <span data-ttu-id="a6136-1886">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="a6136-1886">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="a6136-1887">Configurer</span><span class="sxs-lookup"><span data-stu-id="a6136-1887">Configure</span></span>
* <span data-ttu-id="a6136-1888">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="a6136-1888">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="a6136-1889">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1889">Container</span></span>
* <span data-ttu-id="a6136-1890">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="a6136-1890">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="a6136-1891">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a6136-1891">EventHub</span></span>
* <span data-ttu-id="a6136-1892">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1892">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-1893">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-1893">Interactive</span></span>
* <span data-ttu-id="a6136-1894">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="a6136-1894">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1895">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1895">Monitor</span></span>
* <span data-ttu-id="a6136-1896">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-1896">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1897">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1897">Network</span></span>
* <span data-ttu-id="a6136-1898">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="a6136-1898">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="a6136-1899">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1899">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="a6136-1900">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1900">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="a6136-1901">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-1901">Profile</span></span>
* <span data-ttu-id="a6136-1902">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="a6136-1902">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-1903">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-1903">RDBMS</span></span>
* <span data-ttu-id="a6136-1904">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="a6136-1904">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-1905">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-1905">Resource</span></span>
* <span data-ttu-id="a6136-1906">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="a6136-1906">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="a6136-1907">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-1907">Role</span></span>
* <span data-ttu-id="a6136-1908">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="a6136-1908">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="a6136-1909">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="a6136-1909">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="a6136-1910">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="a6136-1910">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1911">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1911">Storage</span></span>
* <span data-ttu-id="a6136-1912">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="a6136-1912">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1913">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1913">VM</span></span>
* <span data-ttu-id="a6136-1914">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="a6136-1914">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="a6136-1915">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="a6136-1915">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="a6136-1916">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="a6136-1916">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="a6136-1917">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="a6136-1917">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="a6136-1918">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="a6136-1918">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="a6136-1919">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="a6136-1919">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="a6136-1920">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1920">October 23, 2018</span></span>

<span data-ttu-id="a6136-1921">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="a6136-1921">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1922">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1922">Core</span></span>
* <span data-ttu-id="a6136-1923">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="a6136-1923">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="a6136-1924">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="a6136-1924">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1925">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1925">ACR</span></span>
* <span data-ttu-id="a6136-1926">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="a6136-1926">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-1927">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-1927">CDN</span></span>
* <span data-ttu-id="a6136-1928">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="a6136-1928">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a6136-1929">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="a6136-1929">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="a6136-1930">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1930">Container</span></span>
* <span data-ttu-id="a6136-1931">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="a6136-1931">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="a6136-1932">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-1932">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="a6136-1933">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="a6136-1933">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="a6136-1934">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-1934">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="a6136-1935">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="a6136-1935">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="a6136-1936">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="a6136-1936">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="a6136-1937">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="a6136-1937">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-1938">CosmosDB</span></span>
* <span data-ttu-id="a6136-1939">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1939">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-1940">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-1940">Interactive</span></span>
* <span data-ttu-id="a6136-1941">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="a6136-1941">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6136-1942">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6136-1942">IoT Central</span></span>
* <span data-ttu-id="a6136-1943">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="a6136-1943">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="a6136-1944">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="a6136-1944">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-1945">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-1945">Monitor</span></span>
* <span data-ttu-id="a6136-1946">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1946">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="a6136-1947">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-1947">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="a6136-1948">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="a6136-1948">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a6136-1949">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="a6136-1949">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="a6136-1950">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="a6136-1950">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="a6136-1951">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="a6136-1951">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="a6136-1952">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="a6136-1952">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="a6136-1953">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="a6136-1953">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a6136-1954">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="a6136-1954">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="a6136-1955">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1955">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1956">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1956">Network</span></span>
* <span data-ttu-id="a6136-1957">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1957">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="a6136-1958">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1958">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="a6136-1959">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a6136-1959">ServiceBus</span></span>
* <span data-ttu-id="a6136-1960">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-1960">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-1961">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-1961">SQL</span></span>
* <span data-ttu-id="a6136-1962">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="a6136-1962">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-1963">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-1963">Storage</span></span>
* <span data-ttu-id="a6136-1964">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="a6136-1964">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="a6136-1965">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="a6136-1965">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1966">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1966">VM</span></span>
* <span data-ttu-id="a6136-1967">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1967">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6136-1968">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1968">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="a6136-1969">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="a6136-1969">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="a6136-1970">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1970">October 16, 2018</span></span>

<span data-ttu-id="a6136-1971">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="a6136-1971">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-1972">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-1972">VM</span></span>
* <span data-ttu-id="a6136-1973">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="a6136-1973">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="a6136-1974">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-1974">October 9, 2018</span></span>

<span data-ttu-id="a6136-1975">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="a6136-1975">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="a6136-1976">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-1976">Core</span></span>
* <span data-ttu-id="a6136-1977">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="a6136-1977">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-1978">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-1978">ACR</span></span>
* <span data-ttu-id="a6136-1979">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="a6136-1979">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-1980">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-1980">ACS</span></span>
* <span data-ttu-id="a6136-1981">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="a6136-1981">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="a6136-1982">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="a6136-1982">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="a6136-1983">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="a6136-1983">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="a6136-1984">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="a6136-1984">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="a6136-1985">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-1985">Container</span></span>
* <span data-ttu-id="a6136-1986">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="a6136-1986">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="a6136-1987">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-1987">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="a6136-1988">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a6136-1988">Event Hub</span></span>
* <span data-ttu-id="a6136-1989">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="a6136-1989">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="a6136-1990">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="a6136-1990">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="a6136-1991">Extensions</span><span class="sxs-lookup"><span data-stu-id="a6136-1991">Extensions</span></span>
* <span data-ttu-id="a6136-1992">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="a6136-1992">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6136-1993">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6136-1993">HDInsight</span></span>
* <span data-ttu-id="a6136-1994">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-1994">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-1995">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-1995">IoT</span></span>
* <span data-ttu-id="a6136-1996">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="a6136-1996">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-1997">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-1997">KeyVault</span></span>
* <span data-ttu-id="a6136-1998">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="a6136-1998">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="a6136-1999">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-1999">Network</span></span>
* <span data-ttu-id="a6136-2000">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="a6136-2000">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="a6136-2001">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="a6136-2001">See #6052</span></span>
* <span data-ttu-id="a6136-2002">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2002">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="a6136-2003">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="a6136-2003">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="a6136-2004">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="a6136-2004">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="a6136-2005">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="a6136-2005">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="a6136-2006">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="a6136-2006">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="a6136-2007">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2007">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2008">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2008">Role</span></span>
* <span data-ttu-id="a6136-2009">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="a6136-2009">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="a6136-2010">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="a6136-2010">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="a6136-2011">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="a6136-2011">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="a6136-2012">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="a6136-2012">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6136-2013">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-2013">Service Bus</span></span>
* <span data-ttu-id="a6136-2014">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="a6136-2014">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2015">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2015">VM</span></span>
* <span data-ttu-id="a6136-2016">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="a6136-2016">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="a6136-2017">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2017">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="a6136-2018">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="a6136-2018">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="a6136-2019">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="a6136-2019">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="a6136-2020">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2020">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="a6136-2021">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="a6136-2021">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="a6136-2022">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2022">September 21, 2018</span></span>

<span data-ttu-id="a6136-2023">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="a6136-2023">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2024">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2024">ACR</span></span>
* <span data-ttu-id="a6136-2025">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2025">Added ACR Task commands</span></span>
* <span data-ttu-id="a6136-2026">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="a6136-2026">Added quick run command</span></span>
* <span data-ttu-id="a6136-2027">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a6136-2027">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="a6136-2028">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2028">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="a6136-2029">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="a6136-2029">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="a6136-2030">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="a6136-2030">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2031">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2031">ACS</span></span>
* <span data-ttu-id="a6136-2032">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2032">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="a6136-2033">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="a6136-2033">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2034">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2034">AppService</span></span>

* <span data-ttu-id="a6136-2035">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="a6136-2035">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="a6136-2036">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="a6136-2036">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="a6136-2037">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="a6136-2037">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="a6136-2038">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="a6136-2038">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2039">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2039">Batch</span></span>
* <span data-ttu-id="a6136-2040">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="a6136-2040">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="a6136-2041">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="a6136-2041">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="a6136-2042">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2042">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="a6136-2043">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="a6136-2043">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6136-2044">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2044">Batch AI</span></span> 
* <span data-ttu-id="a6136-2045">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2045">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6136-2046">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2046">Cognitive Services</span></span>
* <span data-ttu-id="a6136-2047">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="a6136-2047">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="a6136-2048">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="a6136-2048">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="a6136-2049">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="a6136-2049">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="a6136-2050">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2050">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="a6136-2051">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a6136-2051">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="a6136-2052">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="a6136-2052">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2053">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2053">Container</span></span>
* <span data-ttu-id="a6136-2054">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="a6136-2054">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="a6136-2055">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2055">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="a6136-2056">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a6136-2056">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="a6136-2057">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2057">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="a6136-2058">DataLake</span><span class="sxs-lookup"><span data-stu-id="a6136-2058">Datalake</span></span>
* <span data-ttu-id="a6136-2059">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a6136-2059">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="a6136-2060">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="a6136-2060">Interactive Shell</span></span>
* <span data-ttu-id="a6136-2061">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-2061">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="a6136-2062">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="a6136-2062">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-2063">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2063">IoT</span></span>
* <span data-ttu-id="a6136-2064">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2064">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-2065">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6136-2065">Key Vault</span></span>
* <span data-ttu-id="a6136-2066">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="a6136-2066">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2067">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2067">Network</span></span>
* <span data-ttu-id="a6136-2068">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2068">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="a6136-2069">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="a6136-2069">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="a6136-2070">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="a6136-2070">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="a6136-2071">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2071">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="a6136-2072">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2072">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="a6136-2073">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2073">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="a6136-2074">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2074">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="a6136-2075">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="a6136-2075">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="a6136-2076">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="a6136-2076">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="a6136-2077">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="a6136-2077">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="a6136-2078">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="a6136-2078">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="a6136-2079">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="a6136-2079">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="a6136-2080">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="a6136-2080">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="a6136-2081">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="a6136-2081">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="a6136-2082">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="a6136-2082">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="a6136-2083">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="a6136-2083">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="a6136-2084">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2084">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="a6136-2085">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="a6136-2085">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-2086">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-2086">RDBMS</span></span>
* <span data-ttu-id="a6136-2087">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="a6136-2087">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="a6136-2088">Réservation</span><span class="sxs-lookup"><span data-stu-id="a6136-2088">Reservation</span></span>
* <span data-ttu-id="a6136-2089">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="a6136-2089">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="a6136-2090">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="a6136-2090">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="a6136-2091">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="a6136-2091">Manage App</span></span>
* <span data-ttu-id="a6136-2092">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="a6136-2092">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="a6136-2093">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="a6136-2093">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2094">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2094">Role</span></span>
* <span data-ttu-id="a6136-2095">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="a6136-2095">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="a6136-2096">SignalR</span><span class="sxs-lookup"><span data-stu-id="a6136-2096">SignalR</span></span>
* <span data-ttu-id="a6136-2097">Première version</span><span class="sxs-lookup"><span data-stu-id="a6136-2097">First release</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2098">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2098">Storage</span></span>
* <span data-ttu-id="a6136-2099">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="a6136-2099">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="a6136-2100">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="a6136-2100">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2101">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2101">VM</span></span>
* <span data-ttu-id="a6136-2102">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="a6136-2102">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="a6136-2103">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="a6136-2103">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="a6136-2104">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2104">August 28, 2018</span></span>

<span data-ttu-id="a6136-2105">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a6136-2105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2106">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2106">Core</span></span>

* <span data-ttu-id="a6136-2107">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="a6136-2107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a6136-2108">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a6136-2108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2109">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2109">ACR</span></span>

* <span data-ttu-id="a6136-2110">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-2110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a6136-2111">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="a6136-2111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2112">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2112">ACS</span></span>

* <span data-ttu-id="a6136-2113">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="a6136-2113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a6136-2114">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="a6136-2114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2115">AppService</span></span>

* <span data-ttu-id="a6136-2116">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="a6136-2116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a6136-2117">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="a6136-2117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a6136-2118">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-2119">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-2119">Backup</span></span>

* <span data-ttu-id="a6136-2120">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a6136-2121">Service de robot</span><span class="sxs-lookup"><span data-stu-id="a6136-2121">Bot Service</span></span>

* <span data-ttu-id="a6136-2122">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="a6136-2122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6136-2123">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2123">Cognitive Services</span></span>

* <span data-ttu-id="a6136-2124">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="a6136-2124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-2125">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2125">IoT</span></span>

* <span data-ttu-id="a6136-2126">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="a6136-2126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2127">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2127">Monitor</span></span>

* <span data-ttu-id="a6136-2128">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="a6136-2128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a6136-2129">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="a6136-2129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2130">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2130">Network</span></span>

* <span data-ttu-id="a6136-2131">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2132">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2132">Resource</span></span>

* <span data-ttu-id="a6136-2133">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2134">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2134">Storage</span></span>

* <span data-ttu-id="a6136-2135">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2136">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2136">VM</span></span>

* <span data-ttu-id="a6136-2137">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a6136-2138">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="a6136-2139">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2139">Auguest 14, 2018</span></span>

<span data-ttu-id="a6136-2140">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a6136-2140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2141">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2141">Core</span></span>

* <span data-ttu-id="a6136-2142">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="a6136-2142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a6136-2143">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="a6136-2143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a6136-2144">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="a6136-2144">Telemetry</span></span>

* <span data-ttu-id="a6136-2145">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a6136-2145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2146">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2146">ACR</span></span>

* <span data-ttu-id="a6136-2147">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-2147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a6136-2148">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="a6136-2148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2149">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2149">ACS</span></span>

* <span data-ttu-id="a6136-2150">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-2150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a6136-2151">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-2151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a6136-2152">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="a6136-2152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a6136-2153">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="a6136-2153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a6136-2154">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="a6136-2154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a6136-2155">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2155">AppService</span></span>

* <span data-ttu-id="a6136-2156">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="a6136-2156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a6136-2157">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="a6136-2157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-2158">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2158">BatchAI</span></span>

* <span data-ttu-id="a6136-2159">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="a6136-2159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a6136-2160">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2160">Container</span></span>

* <span data-ttu-id="a6136-2161">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a6136-2162">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2162">IoT</span></span>

* <span data-ttu-id="a6136-2163">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="a6136-2163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a6136-2164">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="a6136-2164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6136-2165">Iot Central</span><span class="sxs-lookup"><span data-stu-id="a6136-2165">Iot Central</span></span>

* <span data-ttu-id="a6136-2166">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6136-2166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-2167">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-2167">KeyVault</span></span>


* <span data-ttu-id="a6136-2168">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="a6136-2168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a6136-2169">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a6136-2170">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="a6136-2170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a6136-2171">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="a6136-2171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a6136-2172">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="a6136-2172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a6136-2173">Relais</span><span class="sxs-lookup"><span data-stu-id="a6136-2173">Relay</span></span>

* <span data-ttu-id="a6136-2174">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-2174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2175">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2175">Sql</span></span>

* <span data-ttu-id="a6136-2176">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="a6136-2176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2177">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2177">Storage</span></span>

* <span data-ttu-id="a6136-2178">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="a6136-2178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a6136-2179">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="a6136-2179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a6136-2180">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="a6136-2180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a6136-2181">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="a6136-2181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a6136-2182">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2183">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2183">VM</span></span>

* <span data-ttu-id="a6136-2184">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="a6136-2184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a6136-2185">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2185">July 31, 2018</span></span>

<span data-ttu-id="a6136-2186">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a6136-2186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2187">ACR</span></span>

* <span data-ttu-id="a6136-2188">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a6136-2189">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="a6136-2189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2190">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2190">ACS</span></span>

* <span data-ttu-id="a6136-2191">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="a6136-2191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2192">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2192">Batch</span></span>

* <span data-ttu-id="a6136-2193">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-2193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2194">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2194">Container</span></span>

* <span data-ttu-id="a6136-2195">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="a6136-2195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2196">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2196">Network</span></span>

* <span data-ttu-id="a6136-2197">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a6136-2197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a6136-2198">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2198">Resource</span></span>

* <span data-ttu-id="a6136-2199">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-2199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a6136-2200">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-2200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2201">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2201">Role</span></span>

* <span data-ttu-id="a6136-2202">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="a6136-2202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a6136-2203">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-2203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a6136-2204">Recherche</span><span class="sxs-lookup"><span data-stu-id="a6136-2204">Search</span></span>

* <span data-ttu-id="a6136-2205">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="a6136-2205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6136-2206">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-2206">Service Bus</span></span>

* <span data-ttu-id="a6136-2207">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="a6136-2207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a6136-2208">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="a6136-2209">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="a6136-2209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="a6136-2210">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="a6136-2210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2211">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2211">Storage</span></span>

* <span data-ttu-id="a6136-2212">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="a6136-2212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a6136-2213">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2214">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2214">VM</span></span>

* <span data-ttu-id="a6136-2215">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a6136-2216">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="a6136-2216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="a6136-2217">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="a6136-2217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a6136-2218">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="a6136-2218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a6136-2219">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2219">July 18, 2018</span></span>

<span data-ttu-id="a6136-2220">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a6136-2220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2221">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2221">Core</span></span>

* <span data-ttu-id="a6136-2222">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-2222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a6136-2223">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a6136-2223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a6136-2224">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a6136-2224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2225">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2225">ACR</span></span>

* <span data-ttu-id="a6136-2226">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="a6136-2226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a6136-2227">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="a6136-2227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a6136-2228">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="a6136-2228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a6136-2229">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="a6136-2229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2230">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2230">ACS</span></span>

* <span data-ttu-id="a6136-2231">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="a6136-2231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2232">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2232">AppService</span></span>

* <span data-ttu-id="a6136-2233">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="a6136-2233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2234">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2234">Batch</span></span>

* <span data-ttu-id="a6136-2235">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-2235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a6136-2236">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-2236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6136-2237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2237">Batch AI</span></span>

* <span data-ttu-id="a6136-2238">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="a6136-2238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2239">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2239">Container</span></span>

* <span data-ttu-id="a6136-2240">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="a6136-2240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a6136-2241">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="a6136-2241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2242">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2242">Network</span></span>

* <span data-ttu-id="a6136-2243">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="a6136-2244">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-2244">Added `network nic wait`</span></span>
* <span data-ttu-id="a6136-2245">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="a6136-2246">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="a6136-2247">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2247">Resource</span></span>

* <span data-ttu-id="a6136-2248">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-2248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="a6136-2249">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-2249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="a6136-2250">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-2250">Added `deployment wait` command</span></span>
* <span data-ttu-id="a6136-2251">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="a6136-2251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2252">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2252">SQL</span></span>

* <span data-ttu-id="a6136-2253">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a6136-2254">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="a6136-2254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="a6136-2255">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="a6136-2255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2256">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2256">Storage</span></span>

* <span data-ttu-id="a6136-2257">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="a6136-2257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2258">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2258">VM</span></span>

* <span data-ttu-id="a6136-2259">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a6136-2260">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="a6136-2261">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="a6136-2261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a6136-2262">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2262">July 3, 2018</span></span>

<span data-ttu-id="a6136-2263">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a6136-2263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-2264">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2264">AKS</span></span>

* <span data-ttu-id="a6136-2265">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a6136-2266">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2266">July 3, 2018</span></span>

<span data-ttu-id="a6136-2267">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a6136-2267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2268">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2268">Core</span></span>

* <span data-ttu-id="a6136-2269">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2270">ACR</span></span>

* <span data-ttu-id="a6136-2271">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="a6136-2271">Added polling build status</span></span>
* <span data-ttu-id="a6136-2272">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-2272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a6136-2273">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="a6136-2273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2274">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2274">ACS</span></span>

* <span data-ttu-id="a6136-2275">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a6136-2276">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a6136-2277">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a6136-2278">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="a6136-2278">Added `--listen-port` support</span></span>
* <span data-ttu-id="a6136-2279">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a6136-2280">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="a6136-2280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a6136-2281">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="a6136-2281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2282">AppService</span></span>

* <span data-ttu-id="a6136-2283">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="a6136-2283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="a6136-2284">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="a6136-2284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-2285">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-2285">Backup</span></span>

* <span data-ttu-id="a6136-2286">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="a6136-2286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-2287">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2287">BatchAI</span></span>

* <span data-ttu-id="a6136-2288">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a6136-2289">Cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-2289">Cloud</span></span>

* <span data-ttu-id="a6136-2290">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-2290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2291">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2291">Container</span></span>

* <span data-ttu-id="a6136-2292">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="a6136-2292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a6136-2293">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="a6136-2293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="a6136-2294">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="a6136-2294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2295">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2295">Extension</span></span>

* <span data-ttu-id="a6136-2296">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="a6136-2296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2297">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2297">Network</span></span>

* <span data-ttu-id="a6136-2298">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="a6136-2298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-2299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6136-2299">Rdbms</span></span>

* <span data-ttu-id="a6136-2300">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-2300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2301">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2301">Resource</span></span>

* <span data-ttu-id="a6136-2302">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="a6136-2302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2303">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2303">VM</span></span>

* <span data-ttu-id="a6136-2304">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="a6136-2304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a6136-2305">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2305">June 25, 2018</span></span>

<span data-ttu-id="a6136-2306">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a6136-2306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a6136-2307">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-2307">CLI</span></span>

* <span data-ttu-id="a6136-2308">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a6136-2309">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2309">June 19, 2018</span></span>

<span data-ttu-id="a6136-2310">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a6136-2310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2311">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2311">Core</span></span>

* <span data-ttu-id="a6136-2312">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2313">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2313">ACR</span></span>

* <span data-ttu-id="a6136-2314">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="a6136-2314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a6136-2315">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2316">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2316">ACS</span></span>

* <span data-ttu-id="a6136-2317">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a6136-2318">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2318">Added `--update` support</span></span>
* <span data-ttu-id="a6136-2319">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="a6136-2319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="a6136-2320">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="a6136-2320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a6136-2321">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="a6136-2321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a6136-2322">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a6136-2322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="a6136-2323">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a6136-2323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="a6136-2324">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a6136-2324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2325">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2325">AppService</span></span>

* <span data-ttu-id="a6136-2326">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="a6136-2326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a6136-2327">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="a6136-2327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2328">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2328">Batch</span></span>

* <span data-ttu-id="a6136-2329">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="a6136-2329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6136-2330">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2330">Batch AI</span></span>

* <span data-ttu-id="a6136-2331">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="a6136-2331">Added support for workspaces.</span></span> <span data-ttu-id="a6136-2332">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="a6136-2332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a6136-2333">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="a6136-2333">Added support for experiments.</span></span> <span data-ttu-id="a6136-2334">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="a6136-2334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a6136-2335">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="a6136-2335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a6136-2336">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a6136-2337">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="a6136-2337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a6136-2338">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="a6136-2338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a6136-2339">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="a6136-2339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a6136-2340">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="a6136-2340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a6136-2341">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a6136-2342">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="a6136-2342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a6136-2343">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a6136-2344">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="a6136-2344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a6136-2345">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="a6136-2345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a6136-2346">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="a6136-2346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a6136-2347">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a6136-2348">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="a6136-2348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="a6136-2349">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="a6136-2349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="a6136-2350">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a6136-2350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a6136-2351">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a6136-2351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a6136-2352">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="a6136-2352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a6136-2353">Cartes</span><span class="sxs-lookup"><span data-stu-id="a6136-2353">Maps</span></span>

* <span data-ttu-id="a6136-2354">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="a6136-2354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2355">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2355">Network</span></span>

* <span data-ttu-id="a6136-2356">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="a6136-2356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a6136-2357">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="a6136-2357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a6136-2358">#6502</span><span class="sxs-lookup"><span data-stu-id="a6136-2358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a6136-2359">Réservations</span><span class="sxs-lookup"><span data-stu-id="a6136-2359">Reservations</span></span>

* <span data-ttu-id="a6136-2360">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="a6136-2361">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="a6136-2362">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="a6136-2362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="a6136-2363">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="a6136-2363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="a6136-2364">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="a6136-2364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="a6136-2365">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2366">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2366">Role</span></span>

* <span data-ttu-id="a6136-2367">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2368">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2368">SQL</span></span>

* <span data-ttu-id="a6136-2369">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2370">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2370">Storage</span></span>

* <span data-ttu-id="a6136-2371">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="a6136-2371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2372">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2372">VM</span></span>

* <span data-ttu-id="a6136-2373">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="a6136-2374">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="a6136-2374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="a6136-2375">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="a6136-2375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a6136-2376">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2376">June 13, 2018</span></span>

<span data-ttu-id="a6136-2377">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a6136-2377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2378">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2378">Core</span></span>

* <span data-ttu-id="a6136-2379">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a6136-2380">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2380">June 13, 2018</span></span>

<span data-ttu-id="a6136-2381">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a6136-2381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-2382">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2382">AKS</span></span>

* <span data-ttu-id="a6136-2383">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a6136-2384">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="a6136-2384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a6136-2385">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a6136-2386">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a6136-2387">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2388">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2388">AppService</span></span>

* <span data-ttu-id="a6136-2389">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="a6136-2389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a6136-2390">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2390">June 5, 2018</span></span>

<span data-ttu-id="a6136-2391">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a6136-2391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2392">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2392">Interactive</span></span>

* <span data-ttu-id="a6136-2393">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a6136-2393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a6136-2394">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2394">June 5, 2018</span></span>

<span data-ttu-id="a6136-2395">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a6136-2395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2396">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2396">Core</span></span>

* <span data-ttu-id="a6136-2397">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="a6136-2397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a6136-2398">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a6136-2398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2399">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2399">ACR</span></span>

* <span data-ttu-id="a6136-2400">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="a6136-2400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a6136-2401">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="a6136-2401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a6136-2402">AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2402">AKS</span></span>

* <span data-ttu-id="a6136-2403">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="a6136-2403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2404">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2404">Batch</span></span>

* <span data-ttu-id="a6136-2405">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a6136-2405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-2406">IOT</span><span class="sxs-lookup"><span data-stu-id="a6136-2406">IOT</span></span>

* <span data-ttu-id="a6136-2407">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="a6136-2407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2408">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2408">Network</span></span>

* <span data-ttu-id="a6136-2409">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="a6136-2409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a6136-2410">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a6136-2410">Policy Insights</span></span>

* <span data-ttu-id="a6136-2411">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-2411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a6136-2412">ARM</span><span class="sxs-lookup"><span data-stu-id="a6136-2412">ARM</span></span>

* <span data-ttu-id="a6136-2413">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2414">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2414">SQL</span></span>

* <span data-ttu-id="a6136-2415">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="a6136-2415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a6136-2416">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="a6136-2416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a6136-2417">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2417">Storage</span></span>

* <span data-ttu-id="a6136-2418">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="a6136-2418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2419">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2419">VM</span></span>

* <span data-ttu-id="a6136-2420">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="a6136-2420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a6136-2421">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a6136-2422">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a6136-2423">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2423">May 22, 2018</span></span>

<span data-ttu-id="a6136-2424">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a6136-2424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2425">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2425">Core</span></span>

* <span data-ttu-id="a6136-2426">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="a6136-2426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2427">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2427">ACS</span></span>

* <span data-ttu-id="a6136-2428">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="a6136-2428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a6136-2429">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-2429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2430">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2430">AppService</span></span>

* <span data-ttu-id="a6136-2431">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a6136-2431">Improved generic update commands</span></span>
* <span data-ttu-id="a6136-2432">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="a6136-2432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2433">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2433">Container</span></span>

* <span data-ttu-id="a6136-2434">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="a6136-2434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a6136-2435">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2436">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2436">Extension</span></span>

* <span data-ttu-id="a6136-2437">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="a6136-2437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2438">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2438">Interactive</span></span>

* <span data-ttu-id="a6136-2439">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a6136-2440">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="a6136-2440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-2441">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-2441">KeyVault</span></span>

* <span data-ttu-id="a6136-2442">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a6136-2442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2443">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2443">Network</span></span>

* <span data-ttu-id="a6136-2444">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a6136-2444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a6136-2445">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a6136-2445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2446">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2446">SQL</span></span>

* <span data-ttu-id="a6136-2447">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="a6136-2447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a6136-2448">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="a6136-2448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a6136-2449">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="a6136-2449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a6136-2450">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a6136-2450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a6136-2451">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a6136-2451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a6136-2452">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a6136-2453">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="a6136-2453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a6136-2454">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2454">`edition`.</span></span> <span data-ttu-id="a6136-2455">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="a6136-2455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a6136-2456">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2456">`elasticPoolName`.</span></span> <span data-ttu-id="a6136-2457">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="a6136-2457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a6136-2458">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a6136-2458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a6136-2459">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2459">`edition`.</span></span> <span data-ttu-id="a6136-2460">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="a6136-2460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a6136-2461">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2461">`dtu`.</span></span> <span data-ttu-id="a6136-2462">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="a6136-2462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a6136-2463">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2463">`databaseDtuMin`.</span></span> <span data-ttu-id="a6136-2464">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="a6136-2464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a6136-2465">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2465">`databaseDtuMax`.</span></span> <span data-ttu-id="a6136-2466">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="a6136-2466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a6136-2467">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a6136-2467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a6136-2468">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a6136-2468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2469">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2469">Storage</span></span>

* <span data-ttu-id="a6136-2470">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-2470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a6136-2471">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="a6136-2471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2472">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2472">VM</span></span>

* <span data-ttu-id="a6136-2473">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a6136-2474">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="a6136-2474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a6136-2475">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="a6136-2475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a6136-2476">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="a6136-2476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a6136-2477">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a6136-2478">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2478">May 7, 2018</span></span>

<span data-ttu-id="a6136-2479">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a6136-2479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2480">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2480">Core</span></span>

* <span data-ttu-id="a6136-2481">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="a6136-2481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a6136-2482">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="a6136-2482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a6136-2483">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a6136-2484">#5591</span><span class="sxs-lookup"><span data-stu-id="a6136-2484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a6136-2485">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a6136-2486">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="a6136-2486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a6136-2487">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a6136-2488">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="a6136-2488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a6136-2489">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-2489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2490">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2490">ACR</span></span>

* <span data-ttu-id="a6136-2491">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2491">Added ACR Build commands</span></span>
* <span data-ttu-id="a6136-2492">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="a6136-2492">Improved resource not found error messages</span></span>
* <span data-ttu-id="a6136-2493">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a6136-2494">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="a6136-2494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a6136-2495">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="a6136-2495">Improved repository commands error messages</span></span>
* <span data-ttu-id="a6136-2496">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="a6136-2496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2497">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2497">ACS</span></span>

* <span data-ttu-id="a6136-2498">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-2498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a6136-2499">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a6136-2499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a6136-2500">AMS</span><span class="sxs-lookup"><span data-stu-id="a6136-2500">AMS</span></span>

* <span data-ttu-id="a6136-2501">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2502">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2502">Appservice</span></span>

* <span data-ttu-id="a6136-2503">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="a6136-2503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a6136-2504">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a6136-2505">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="a6136-2505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a6136-2506">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6136-2507">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2507">Batch AI</span></span>

* <span data-ttu-id="a6136-2508">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="a6136-2508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6136-2509">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2509">Cognitive Services</span></span>

* <span data-ttu-id="a6136-2510">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="a6136-2510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-2511">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-2511">Consumption</span></span>

* <span data-ttu-id="a6136-2512">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="a6136-2512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2513">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2513">Container</span></span>

* <span data-ttu-id="a6136-2514">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="a6136-2514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6136-2515">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-2515">Cosmos DB</span></span>

* <span data-ttu-id="a6136-2516">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6136-2516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a6136-2517">DMS</span><span class="sxs-lookup"><span data-stu-id="a6136-2517">DMS</span></span>

* <span data-ttu-id="a6136-2518">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="a6136-2518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2519">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2519">Extension</span></span>

* <span data-ttu-id="a6136-2520">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="a6136-2520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2521">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2521">Interactive</span></span>

* <span data-ttu-id="a6136-2522">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="a6136-2522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a6136-2523">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="a6136-2523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a6136-2524">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="a6136-2524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a6136-2525">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a6136-2526">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-2526">Lab</span></span>

* <span data-ttu-id="a6136-2527">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="a6136-2527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2528">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2528">Network</span></span>

* <span data-ttu-id="a6136-2529">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="a6136-2529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a6136-2530">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2530">Profile</span></span>

* <span data-ttu-id="a6136-2531">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a6136-2532">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="a6136-2532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a6136-2533">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="a6136-2533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a6136-2534">Redis</span><span class="sxs-lookup"><span data-stu-id="a6136-2534">Redis</span></span>

* <span data-ttu-id="a6136-2535">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a6136-2536">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="a6136-2536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a6136-2537">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a6136-2538">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="a6136-2538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a6136-2539">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2540">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2540">Role</span></span>

* <span data-ttu-id="a6136-2541">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a6136-2541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2542">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2542">Storage</span></span>

* <span data-ttu-id="a6136-2543">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="a6136-2543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a6136-2544">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="a6136-2544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a6136-2545">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="a6136-2545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a6136-2546">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="a6136-2546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a6136-2547">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2548">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2548">VM</span></span>

* <span data-ttu-id="a6136-2549">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="a6136-2549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a6136-2550">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a6136-2550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a6136-2551">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="a6136-2551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a6136-2552">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="a6136-2552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a6136-2553">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="a6136-2553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a6136-2554">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="a6136-2554">Added write accelerator support</span></span>
* <span data-ttu-id="a6136-2555">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a6136-2555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a6136-2556">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a6136-2557">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="a6136-2557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a6136-2558">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2558">April 10, 2018</span></span>

<span data-ttu-id="a6136-2559">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a6136-2559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2560">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2560">ACR</span></span>

* <span data-ttu-id="a6136-2561">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="a6136-2561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2562">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2562">ACS</span></span>

* <span data-ttu-id="a6136-2563">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="a6136-2563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2564">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2564">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a6136-2566">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="a6136-2566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-2567">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2567">BatchAI</span></span>

* <span data-ttu-id="a6136-2568">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="a6136-2568">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="a6136-2569">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="a6136-2569">Job level mounting</span></span>
  - <span data-ttu-id="a6136-2570">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="a6136-2570">Environment variables with secret values</span></span>
  - <span data-ttu-id="a6136-2571">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="a6136-2571">Performance counters settings</span></span>
  - <span data-ttu-id="a6136-2572">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="a6136-2572">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="a6136-2573">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="a6136-2573">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="a6136-2574">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="a6136-2574">Usage and limits reporting</span></span>
  - <span data-ttu-id="a6136-2575">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="a6136-2575">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="a6136-2576">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="a6136-2576">Support for custom images</span></span>
  - <span data-ttu-id="a6136-2577">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="a6136-2577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a6136-2578">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="a6136-2578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a6136-2579">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="a6136-2579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a6136-2580">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="a6136-2580">National clouds are supported</span></span>
* <span data-ttu-id="a6136-2581">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="a6136-2581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a6136-2582">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="a6136-2582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a6136-2583">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-2583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a6136-2584">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="a6136-2584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a6136-2585">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="a6136-2585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a6136-2586">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="a6136-2586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a6136-2587">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a6136-2588">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="a6136-2588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a6136-2589">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="a6136-2589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a6136-2590">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a6136-2591">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-2591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a6136-2592">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="a6136-2592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a6136-2593">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a6136-2594">Facturation</span><span class="sxs-lookup"><span data-stu-id="a6136-2594">Billing</span></span>

* <span data-ttu-id="a6136-2595">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="a6136-2595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-2596">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-2596">Consumption</span></span>

* <span data-ttu-id="a6136-2597">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="a6136-2597">Added `marketplace` commands</span></span>
* <span data-ttu-id="a6136-2598">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a6136-2598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a6136-2599">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="a6136-2599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a6136-2600">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="a6136-2600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a6136-2601">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a6136-2601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a6136-2602">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="a6136-2602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2603">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2603">Container</span></span>

* <span data-ttu-id="a6136-2604">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="a6136-2604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a6136-2605">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="a6136-2605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2606">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2606">Extension</span></span>

* <span data-ttu-id="a6136-2607">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="a6136-2607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2608">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2608">Interactive</span></span>

* <span data-ttu-id="a6136-2609">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="a6136-2609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a6136-2610">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-2610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a6136-2611">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="a6136-2611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2612">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2612">Network</span></span>

* <span data-ttu-id="a6136-2613">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="a6136-2613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a6136-2614">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a6136-2615">#4910</span><span class="sxs-lookup"><span data-stu-id="a6136-2615">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a6136-2616">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a6136-2616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a6136-2617">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a6136-2617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a6136-2618">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a6136-2619">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a6136-2620">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="a6136-2620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-2621">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2621">Profile</span></span>

* <span data-ttu-id="a6136-2622">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a6136-2623">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="a6136-2623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-2624">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-2624">RDBMS</span></span>

* <span data-ttu-id="a6136-2625">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="a6136-2625">Added `georestore` command</span></span>
* <span data-ttu-id="a6136-2626">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2627">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2627">Resource</span></span>

* <span data-ttu-id="a6136-2628">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a6136-2629">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2630">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2630">SQL</span></span>

* <span data-ttu-id="a6136-2631">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="a6136-2631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2632">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2632">Storage</span></span>

* <span data-ttu-id="a6136-2633">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="a6136-2633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2634">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2634">VM</span></span>

* <span data-ttu-id="a6136-2635">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a6136-2636">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="a6136-2636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a6136-2638">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a6136-2639">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="a6136-2639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a6136-2640">#5718</span><span class="sxs-lookup"><span data-stu-id="a6136-2640">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a6136-2641">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="a6136-2641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a6136-2642">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2642">March 27, 2018</span></span>

<span data-ttu-id="a6136-2643">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a6136-2643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2644">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2644">Core</span></span>

* <span data-ttu-id="a6136-2645">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="a6136-2645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2646">ACS</span></span>

* <span data-ttu-id="a6136-2647">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-2647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2648">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2648">Appservice</span></span>

* <span data-ttu-id="a6136-2649">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a6136-2650">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-2651">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-2651">Backup</span></span>

* <span data-ttu-id="a6136-2652">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="a6136-2652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a6136-2653">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-2653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a6136-2654">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a6136-2654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a6136-2655">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2656">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2656">Container</span></span>

* <span data-ttu-id="a6136-2657">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="a6136-2657">Added `container exec` command.</span></span> <span data-ttu-id="a6136-2658">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="a6136-2658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a6136-2659">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2660">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2660">Extension</span></span>

* <span data-ttu-id="a6136-2661">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-2661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a6136-2662">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="a6136-2662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a6136-2663">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2664">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2664">Interactive</span></span>

* <span data-ttu-id="a6136-2665">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-2665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a6136-2666">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="a6136-2666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a6136-2667">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="a6136-2667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a6136-2668">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="a6136-2668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a6136-2669">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-2669">Lab</span></span>

* <span data-ttu-id="a6136-2670">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="a6136-2670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2671">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2671">Monitor</span></span>

* <span data-ttu-id="a6136-2672">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a6136-2672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a6136-2673">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="a6136-2673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a6136-2674">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a6136-2674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2675">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2675">Network</span></span>

* <span data-ttu-id="a6136-2676">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="a6136-2676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-2677">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2677">Profile</span></span>

* <span data-ttu-id="a6136-2678">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="a6136-2678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-2679">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-2679">RDBMS</span></span>

* <span data-ttu-id="a6136-2680">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a6136-2680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2681">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2681">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a6136-2683">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2683">Role</span></span>

* <span data-ttu-id="a6136-2684">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a6136-2685">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="a6136-2685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a6136-2686">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a6136-2687">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a6136-2688">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="a6136-2688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2689">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2689">Storage</span></span>

* <span data-ttu-id="a6136-2690">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="a6136-2690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a6136-2691">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="a6136-2691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2692">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2692">VM</span></span>

* <span data-ttu-id="a6136-2693">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="a6136-2693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a6136-2694">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a6136-2695">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="a6136-2695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a6136-2696">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="a6136-2696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a6136-2697">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2697">March 13, 2018</span></span>

<span data-ttu-id="a6136-2698">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a6136-2698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2699">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2699">ACR</span></span>

* <span data-ttu-id="a6136-2700">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-2700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a6136-2701">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="a6136-2701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a6136-2702">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="a6136-2702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2703">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2703">ACS</span></span>

* <span data-ttu-id="a6136-2704">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="a6136-2704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a6136-2705">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="a6136-2705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a6136-2706">Advisor</span><span class="sxs-lookup"><span data-stu-id="a6136-2706">Advisor</span></span>

* <span data-ttu-id="a6136-2707">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a6136-2708">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a6136-2709">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="a6136-2709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="a6136-2710">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a6136-2711">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2712">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2712">Appservice</span></span>

* <span data-ttu-id="a6136-2713">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a6136-2713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a6136-2714">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a6136-2715">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="a6136-2715">Eventhubs</span></span>

* <span data-ttu-id="a6136-2716">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-2716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2717">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2717">Extension</span></span>

* <span data-ttu-id="a6136-2718">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2719">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2719">Interactive</span></span>

* <span data-ttu-id="a6136-2720">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="a6136-2720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a6136-2721">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="a6136-2721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a6136-2722">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="a6136-2722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a6136-2723">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="a6136-2723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2724">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2724">Monitor</span></span>

* <span data-ttu-id="a6136-2725">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="a6136-2725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a6136-2726">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="a6136-2726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a6136-2727">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="a6136-2727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a6136-2728">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-2728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2729">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2729">Network</span></span>

* <span data-ttu-id="a6136-2730">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a6136-2731">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a6136-2731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a6136-2732">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="a6136-2732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a6136-2733">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="a6136-2733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-2734">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2734">Profile</span></span>

* <span data-ttu-id="a6136-2735">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="a6136-2735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a6136-2736">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="a6136-2736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-2737">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-2737">RDBMS</span></span>

* <span data-ttu-id="a6136-2738">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-2738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6136-2739">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a6136-2739">Service Bus</span></span>

* <span data-ttu-id="a6136-2740">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-2740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2741">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2741">Storage</span></span>

* <span data-ttu-id="a6136-2742">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="a6136-2742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a6136-2743">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="a6136-2743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2744">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2744">VM</span></span>

* <span data-ttu-id="a6136-2745">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="a6136-2745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a6136-2746">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="a6136-2746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a6136-2747">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="a6136-2747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a6136-2748">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="a6136-2748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a6136-2749">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2749">February 27, 2018</span></span>

<span data-ttu-id="a6136-2750">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a6136-2750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2751">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2751">Core</span></span>

* <span data-ttu-id="a6136-2752">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="a6136-2752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a6136-2753">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="a6136-2753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a6136-2754">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="a6136-2754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2755">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2755">ACS</span></span>

* <span data-ttu-id="a6136-2756">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a6136-2757">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="a6136-2757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a6136-2758">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a6136-2758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a6136-2759">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="a6136-2759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2760">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2760">Appservice</span></span>

* <span data-ttu-id="a6136-2761">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a6136-2761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a6136-2762">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="a6136-2762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6136-2763">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2763">Cognitive Services</span></span>

* <span data-ttu-id="a6136-2764">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-2764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-2765">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-2765">Consumption</span></span>

* <span data-ttu-id="a6136-2766">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="a6136-2766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a6136-2767">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="a6136-2767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2768">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2768">Container</span></span>

* <span data-ttu-id="a6136-2769">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="a6136-2769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2770">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2770">Network</span></span>

* <span data-ttu-id="a6136-2771">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="a6136-2771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2772">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2772">Resource</span></span>

* <span data-ttu-id="a6136-2773">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="a6136-2773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2774">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2774">Role</span></span>

* <span data-ttu-id="a6136-2775">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="a6136-2775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2776">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2776">SQL</span></span>

* <span data-ttu-id="a6136-2777">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="a6136-2777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2778">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2778">Storage</span></span>

* <span data-ttu-id="a6136-2779">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2780">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2780">VM</span></span>

* <span data-ttu-id="a6136-2781">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="a6136-2781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a6136-2782">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2782">February 13, 2018</span></span>

<span data-ttu-id="a6136-2783">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a6136-2783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2784">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2784">Core</span></span>

* <span data-ttu-id="a6136-2785">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="a6136-2785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2786">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2786">ACS</span></span>

* <span data-ttu-id="a6136-2787">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="a6136-2787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a6136-2788">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a6136-2789">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-2789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a6136-2790">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a6136-2791">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="a6136-2791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a6136-2792">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="a6136-2792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a6136-2793">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-2793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a6136-2794">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="a6136-2794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2795">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2795">Appservice</span></span>

* <span data-ttu-id="a6136-2796">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="a6136-2796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a6136-2797">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="a6136-2797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-2798">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-2798">CDN</span></span>

* <span data-ttu-id="a6136-2799">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2800">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2800">Container</span></span>

* <span data-ttu-id="a6136-2801">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="a6136-2801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a6136-2802">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-2803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-2803">CosmosDB</span></span>

* <span data-ttu-id="a6136-2804">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a6136-2804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-2805">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-2805">Extension</span></span>

* <span data-ttu-id="a6136-2806">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a6136-2807">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a6136-2808">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a6136-2808">Feedback</span></span>

* <span data-ttu-id="a6136-2809">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a6136-2809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2810">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2810">Interactive</span></span>

* <span data-ttu-id="a6136-2811">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a6136-2811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a6136-2812">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="a6136-2812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-2813">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2813">IoT</span></span>

* <span data-ttu-id="a6136-2814">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a6136-2814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a6136-2815">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a6136-2815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a6136-2816">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a6136-2817">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="a6136-2817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2818">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2818">Monitor</span></span>

* <span data-ttu-id="a6136-2819">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2820">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2820">Network</span></span>

* <span data-ttu-id="a6136-2821">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a6136-2821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a6136-2822">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2822">Profile</span></span>

* <span data-ttu-id="a6136-2823">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a6136-2823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2824">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2824">Resource</span></span>

* <span data-ttu-id="a6136-2825">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2826">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2826">Role</span></span>

* <span data-ttu-id="a6136-2827">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2828">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2828">SQL</span></span>

* <span data-ttu-id="a6136-2829">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="a6136-2829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a6136-2830">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="a6136-2830">Added `sql db rename`</span></span>
* <span data-ttu-id="a6136-2831">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="a6136-2831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2832">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2832">Storage</span></span>

* <span data-ttu-id="a6136-2833">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="a6136-2833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2834">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2834">VM</span></span>

* <span data-ttu-id="a6136-2835">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="a6136-2835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a6136-2836">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="a6136-2836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a6136-2837">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="a6136-2837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a6136-2838">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2838">January 31, 2018</span></span>

<span data-ttu-id="a6136-2839">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a6136-2839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2840">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2840">Core</span></span>

* <span data-ttu-id="a6136-2841">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="a6136-2841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a6136-2842">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-2842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a6136-2843">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="a6136-2843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a6136-2844">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="a6136-2844">Use `--verbose` to see</span></span>
* <span data-ttu-id="a6136-2845">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="a6136-2845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2846">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2846">ACS</span></span>

* <span data-ttu-id="a6136-2847">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="a6136-2847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a6136-2848">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="a6136-2848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2849">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2849">Appservice</span></span>

* <span data-ttu-id="a6136-2850">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="a6136-2850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a6136-2851">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="a6136-2851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-2852">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-2852">CDN</span></span>

* <span data-ttu-id="a6136-2853">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-2854">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-2854">CosmosDB</span></span>

* <span data-ttu-id="a6136-2855">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="a6136-2855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2856">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2856">Interactive</span></span>

* <span data-ttu-id="a6136-2857">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="a6136-2857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2858">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2858">Network</span></span>

* <span data-ttu-id="a6136-2859">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a6136-2860">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a6136-2861">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a6136-2862">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a6136-2863">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="a6136-2863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a6136-2864">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="a6136-2864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a6136-2865">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="a6136-2865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a6136-2866">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="a6136-2866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a6136-2867">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="a6136-2867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="a6136-2868">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="a6136-2868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-2869">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2869">Profile</span></span>

* <span data-ttu-id="a6136-2870">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a6136-2870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2871">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2871">Resource</span></span>

* <span data-ttu-id="a6136-2872">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="a6136-2872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2873">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2873">Storage</span></span>

* <span data-ttu-id="a6136-2874">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="a6136-2874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a6136-2875">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="a6136-2875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a6136-2876">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-2876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="a6136-2877">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a6136-2878">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="a6136-2878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2879">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2879">VM</span></span>

* <span data-ttu-id="a6136-2880">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="a6136-2880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a6136-2881">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="a6136-2881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a6136-2882">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="a6136-2882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a6136-2883">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a6136-2884">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a6136-2884">January 17, 2018</span></span>

<span data-ttu-id="a6136-2885">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a6136-2885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2886">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2886">ACR</span></span>

* <span data-ttu-id="a6136-2887">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-2887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a6136-2888">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="a6136-2888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2889">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2889">ACS</span></span>

* <span data-ttu-id="a6136-2890">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a6136-2890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a6136-2891">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="a6136-2891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2892">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2892">Appservice</span></span>

* <span data-ttu-id="a6136-2893">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="a6136-2893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a6136-2894">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="a6136-2894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a6136-2895">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="a6136-2895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-2896">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-2896">Backup</span></span>

* <span data-ttu-id="a6136-2897">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="a6136-2897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a6136-2898">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="a6136-2898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a6136-2899">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-2899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a6136-2900">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="a6136-2900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a6136-2901">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-2902">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-2902">Batch</span></span>

* <span data-ttu-id="a6136-2903">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="a6136-2903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a6136-2904">Cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-2904">Cloud</span></span>

* <span data-ttu-id="a6136-2905">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-2905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-2906">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-2906">Consumption</span></span>

* <span data-ttu-id="a6136-2907">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="a6136-2907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6136-2908">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a6136-2908">Event Grid</span></span>

* <span data-ttu-id="a6136-2909">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a6136-2909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a6136-2910">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a6136-2910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a6136-2911">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="a6136-2911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a6136-2912">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="a6136-2912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a6136-2913">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a6136-2914">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a6136-2915">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="a6136-2915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a6136-2916">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="a6136-2916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-2917">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-2917">Interactive</span></span>

* <span data-ttu-id="a6136-2918">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="a6136-2918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a6136-2919">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="a6136-2919">Fixed errors on startup</span></span>
* <span data-ttu-id="a6136-2920">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="a6136-2920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-2921">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2921">IoT</span></span>

* <span data-ttu-id="a6136-2922">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="a6136-2922">Added support for device provisioning service</span></span>
* <span data-ttu-id="a6136-2923">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a6136-2924">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-2924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2925">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2925">Monitor</span></span>

* <span data-ttu-id="a6136-2926">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="a6136-2926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a6136-2927">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a6136-2928">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="a6136-2928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2929">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2929">Network</span></span>

* <span data-ttu-id="a6136-2930">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a6136-2931">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-2932">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-2932">Profile</span></span>

* <span data-ttu-id="a6136-2933">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2934">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2934">Role</span></span>

* <span data-ttu-id="a6136-2935">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="a6136-2935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6136-2936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-2936">Service Fabric</span></span>

* <span data-ttu-id="a6136-2937">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="a6136-2937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a6136-2938">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-2938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2939">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2939">VM</span></span>

* <span data-ttu-id="a6136-2940">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="a6136-2940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a6136-2941">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="a6136-2941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a6136-2942">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="a6136-2942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a6136-2943">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="a6136-2943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a6136-2944">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="a6136-2944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a6136-2945">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6136-2946">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6136-2947">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="a6136-2947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a6136-2948">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-2948">December 19, 2017</span></span>

<span data-ttu-id="a6136-2949">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a6136-2949">Version 2.0.23</span></span>

* <span data-ttu-id="a6136-2950">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a6136-2950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2951">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2951">Container</span></span>

* <span data-ttu-id="a6136-2952">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a6136-2953">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-2953">Network</span></span>

* <span data-ttu-id="a6136-2954">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a6136-2955">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-2955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-2956">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-2956">Storage</span></span>

* <span data-ttu-id="a6136-2957">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="a6136-2957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2958">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2958">VM</span></span>

* <span data-ttu-id="a6136-2959">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="a6136-2959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a6136-2960">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-2960">December 5, 2017</span></span>

<span data-ttu-id="a6136-2961">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a6136-2961">Version 2.0.22</span></span>

* <span data-ttu-id="a6136-2962">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="a6136-2962">Removed `az component` commands.</span></span> <span data-ttu-id="a6136-2963">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="a6136-2963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a6136-2964">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-2964">Core</span></span>
* <span data-ttu-id="a6136-2965">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="a6136-2965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a6136-2966">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="a6136-2966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-2967">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2967">ACS</span></span>

* <span data-ttu-id="a6136-2968">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a6136-2968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a6136-2969">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="a6136-2969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a6136-2970">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="a6136-2970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a6136-2971">Advisor</span><span class="sxs-lookup"><span data-stu-id="a6136-2971">Advisor</span></span>

* <span data-ttu-id="a6136-2972">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-2972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-2973">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-2973">Appservice</span></span>

* <span data-ttu-id="a6136-2974">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="a6136-2974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a6136-2975">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="a6136-2975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a6136-2976">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="a6136-2976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a6136-2977">Consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-2977">Consumption</span></span>

* <span data-ttu-id="a6136-2978">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="a6136-2978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a6136-2979">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-2979">Container</span></span>

* <span data-ttu-id="a6136-2980">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-2980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-2981">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-2981">Monitor</span></span>

* <span data-ttu-id="a6136-2982">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="a6136-2982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-2983">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-2983">Resource</span></span>

* <span data-ttu-id="a6136-2984">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="a6136-2984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a6136-2985">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-2985">Role</span></span>

* <span data-ttu-id="a6136-2986">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="a6136-2986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a6136-2987">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="a6136-2987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a6136-2988">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a6136-2988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-2989">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-2989">SQL</span></span>

* <span data-ttu-id="a6136-2990">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="a6136-2990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a6136-2991">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="a6136-2991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-2992">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-2992">VM</span></span>

* <span data-ttu-id="a6136-2993">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="a6136-2993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a6136-2994">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-2994">November 14, 2017</span></span>

<span data-ttu-id="a6136-2995">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a6136-2995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-2996">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-2996">ACR</span></span>

* <span data-ttu-id="a6136-2997">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="a6136-2997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a6136-2998">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-2998">ACS</span></span>

* <span data-ttu-id="a6136-2999">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="a6136-2999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a6136-3000">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a6136-3001">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="a6136-3001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a6136-3002">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-3002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a6136-3003">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a6136-3003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3004">Appservice</span></span>

* <span data-ttu-id="a6136-3005">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="a6136-3005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a6136-3006">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a6136-3006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a6136-3007">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a6136-3007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a6136-3008">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="a6136-3008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a6136-3009">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="a6136-3009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a6136-3010">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="a6136-3010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-3011">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-3011">Batch</span></span>

* <span data-ttu-id="a6136-3012">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="a6136-3012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-3013">Batchai</span><span class="sxs-lookup"><span data-stu-id="a6136-3013">Batchai</span></span>

* <span data-ttu-id="a6136-3014">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a6136-3015">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a6136-3016">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="a6136-3016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a6136-3017">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a6136-3018">Cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-3018">Cloud</span></span>

* <span data-ttu-id="a6136-3019">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="a6136-3019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a6136-3020">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-3020">Container</span></span>

* <span data-ttu-id="a6136-3021">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="a6136-3021">Added support to open multiple ports</span></span>
* <span data-ttu-id="a6136-3022">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a6136-3022">Added container group restart policy</span></span>
* <span data-ttu-id="a6136-3023">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="a6136-3023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a6136-3024">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="a6136-3024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6136-3025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-3025">Data Lake Analytics</span></span>

* <span data-ttu-id="a6136-3026">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a6136-3026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6136-3027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3027">Data Lake Store</span></span>

* <span data-ttu-id="a6136-3028">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a6136-3028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-3029">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-3029">Extension</span></span>

* <span data-ttu-id="a6136-3030">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="a6136-3030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a6136-3031">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="a6136-3031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-3032">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-3032">IoT</span></span>

* <span data-ttu-id="a6136-3033">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="a6136-3033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-3034">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-3034">Monitor</span></span>

* <span data-ttu-id="a6136-3035">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="a6136-3035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3036">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3036">Network</span></span>

* <span data-ttu-id="a6136-3037">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="a6136-3037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a6136-3038">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a6136-3039">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a6136-3039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a6136-3040">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="a6136-3040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a6136-3041">Réservations</span><span class="sxs-lookup"><span data-stu-id="a6136-3041">Reservations</span></span>

* <span data-ttu-id="a6136-3042">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-3042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3043">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3043">Resource</span></span>

* <span data-ttu-id="a6136-3044">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-3044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3045">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3045">SQL</span></span>

* <span data-ttu-id="a6136-3046">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3047">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3047">Storage</span></span>

* <span data-ttu-id="a6136-3048">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-3048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a6136-3049">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="a6136-3049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a6136-3050">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="a6136-3050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a6136-3051">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="a6136-3051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a6136-3052">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a6136-3053">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="a6136-3053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a6136-3054">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3055">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3055">VM</span></span>

* <span data-ttu-id="a6136-3056">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="a6136-3056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a6136-3057">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="a6136-3057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a6136-3058">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="a6136-3058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a6136-3059">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="a6136-3059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a6136-3060">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a6136-3060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a6136-3061">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3061">October 24, 2017</span></span>

<span data-ttu-id="a6136-3062">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a6136-3062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a6136-3063">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3063">Core</span></span>

* <span data-ttu-id="a6136-3064">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="a6136-3064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-3065">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-3065">ACR</span></span>

* <span data-ttu-id="a6136-3066">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a6136-3066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a6136-3067">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="a6136-3067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a6136-3068">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="a6136-3068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3069">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3069">ACS</span></span>

* <span data-ttu-id="a6136-3070">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="a6136-3070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a6136-3071">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a6136-3071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3072">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3072">Appservice</span></span>

* <span data-ttu-id="a6136-3073">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="a6136-3073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a6136-3074">Composant</span><span class="sxs-lookup"><span data-stu-id="a6136-3074">Component</span></span>

* <span data-ttu-id="a6136-3075">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="a6136-3075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-3076">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-3076">Monitor</span></span>

* <span data-ttu-id="a6136-3077">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="a6136-3077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3078">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3078">Resource</span></span>

* <span data-ttu-id="a6136-3079">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="a6136-3079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a6136-3080">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="a6136-3080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3081">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3081">VM</span></span>

* <span data-ttu-id="a6136-3082">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a6136-3083">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3083">October 9, 2017</span></span>

<span data-ttu-id="a6136-3084">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a6136-3084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a6136-3085">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3085">Core</span></span>

* <span data-ttu-id="a6136-3086">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a6136-3086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3087">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3087">Appservice</span></span>

* <span data-ttu-id="a6136-3088">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-3089">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-3089">Batch</span></span>

* <span data-ttu-id="a6136-3090">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-3090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a6136-3091">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="a6136-3091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a6136-3092">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-3092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a6136-3093">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="a6136-3093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a6136-3094">Batchai</span><span class="sxs-lookup"><span data-stu-id="a6136-3094">Batchai</span></span>

* <span data-ttu-id="a6136-3095">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6136-3095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-3096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-3096">Keyvault</span></span>

* <span data-ttu-id="a6136-3097">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6136-3097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a6136-3098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a6136-3098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a6136-3099">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3099">Network</span></span>

* <span data-ttu-id="a6136-3100">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="a6136-3100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a6136-3101">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="a6136-3101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3102">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3102">Resource</span></span>

* <span data-ttu-id="a6136-3103">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="a6136-3103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a6136-3104">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-3104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a6136-3105">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="a6136-3105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a6136-3106">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-3106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3107">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3107">Sql</span></span>

* <span data-ttu-id="a6136-3108">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="a6136-3108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a6136-3109">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="a6136-3109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a6136-3110">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="a6136-3110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3111">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3111">Storage</span></span>

* <span data-ttu-id="a6136-3112">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="a6136-3112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3113">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3113">Vm</span></span>

* <span data-ttu-id="a6136-3114">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="a6136-3114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a6136-3115">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a6136-3116">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a6136-3116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a6136-3117">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a6136-3118">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a6136-3119">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3119">September 22, 2017</span></span>

<span data-ttu-id="a6136-3120">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a6136-3120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3121">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3121">Resource</span></span>

* <span data-ttu-id="a6136-3122">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="a6136-3122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a6136-3123">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="a6136-3123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a6136-3124">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a6136-3125">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="a6136-3125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3126">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3126">Network</span></span>

* <span data-ttu-id="a6136-3127">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a6136-3127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a6136-3128">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="a6136-3128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a6136-3129">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="a6136-3129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a6136-3130">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a6136-3131">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a6136-3132">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a6136-3133">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3134">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3134">Storage</span></span>

* <span data-ttu-id="a6136-3135">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a6136-3135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6136-3136">Événement</span><span class="sxs-lookup"><span data-stu-id="a6136-3136">Eventgrid</span></span>

* <span data-ttu-id="a6136-3137">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="a6136-3137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3138">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3138">SQL</span></span>

* <span data-ttu-id="a6136-3139">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="a6136-3139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a6136-3140">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="a6136-3140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a6136-3141">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-3142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-3142">Keyvault</span></span>

* <span data-ttu-id="a6136-3143">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="a6136-3143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3144">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3144">VM</span></span>

* <span data-ttu-id="a6136-3145">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a6136-3146">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="a6136-3146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a6136-3147">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a6136-3148">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a6136-3148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a6136-3149">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a6136-3149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a6136-3150">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a6136-3150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3151">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3151">ACS</span></span>

* <span data-ttu-id="a6136-3152">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-3152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3153">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3153">Appservice</span></span>

* <span data-ttu-id="a6136-3154">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a6136-3155">Backup</span><span class="sxs-lookup"><span data-stu-id="a6136-3155">Backup</span></span>

* <span data-ttu-id="a6136-3156">Préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-3156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a6136-3157">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3157">September 11, 2017</span></span>

<span data-ttu-id="a6136-3158">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a6136-3158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a6136-3159">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3159">Core</span></span>

* <span data-ttu-id="a6136-3160">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="a6136-3160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a6136-3161">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="a6136-3161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3162">Acs</span><span class="sxs-lookup"><span data-stu-id="a6136-3162">Acs</span></span>

* <span data-ttu-id="a6136-3163">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="a6136-3163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a6136-3164">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="a6136-3164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3165">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3165">Appservice</span></span>

* <span data-ttu-id="a6136-3166">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="a6136-3166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-3167">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-3167">CDN</span></span>

* <span data-ttu-id="a6136-3168">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a6136-3169">Extension</span><span class="sxs-lookup"><span data-stu-id="a6136-3169">Extension</span></span>

* <span data-ttu-id="a6136-3170">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-3170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-3171">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-3171">Keyvault</span></span>

* <span data-ttu-id="a6136-3172">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-3172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3173">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3173">Network</span></span>

* <span data-ttu-id="a6136-3174">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="a6136-3174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a6136-3175">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a6136-3176">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a6136-3177">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a6136-3178">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3179">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3179">Resource</span></span>

* <span data-ttu-id="a6136-3180">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a6136-3181">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a6136-3182">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="a6136-3182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a6136-3183">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="a6136-3183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3184">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3184">SQL</span></span>

* <span data-ttu-id="a6136-3185">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-3185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3186">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3186">VM</span></span>

* <span data-ttu-id="a6136-3187">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="a6136-3187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a6136-3188">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="a6136-3188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a6136-3189">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a6136-3190">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="a6136-3190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a6136-3191">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="a6136-3191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a6136-3192">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3192">August 31, 2017</span></span>

<span data-ttu-id="a6136-3193">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a6136-3193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-3194">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-3194">Keyvault</span></span>

* <span data-ttu-id="a6136-3195">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="a6136-3195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a6136-3196">Sf</span><span class="sxs-lookup"><span data-stu-id="a6136-3196">Sf</span></span>

* <span data-ttu-id="a6136-3197">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="a6136-3197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3198">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3198">Storage</span></span>

* <span data-ttu-id="a6136-3199">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="a6136-3199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a6136-3200">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="a6136-3200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a6136-3201">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3201">August 28, 2017</span></span>

<span data-ttu-id="a6136-3202">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a6136-3202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a6136-3203">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a6136-3203">CLI</span></span>

* <span data-ttu-id="a6136-3204">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="a6136-3204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3205">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3205">ACS</span></span>

* <span data-ttu-id="a6136-3206">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a6136-3206">Corrected preview regions</span></span>
* <span data-ttu-id="a6136-3207">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-3207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a6136-3208">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3209">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3209">Appservice</span></span>

* <span data-ttu-id="a6136-3210">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a6136-3211">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-3211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a6136-3212">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="a6136-3212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a6136-3213">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="a6136-3213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a6136-3214">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-3214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-3215">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-3215">IoT</span></span>

* <span data-ttu-id="a6136-3216">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="a6136-3216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3217">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3217">Network</span></span>

* <span data-ttu-id="a6136-3218">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="a6136-3218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a6136-3219">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a6136-3220">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6136-3220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a6136-3221">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a6136-3222">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-3223">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-3223">Profile</span></span>

* <span data-ttu-id="a6136-3224">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6136-3225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-3225">Service Fabric</span></span>

* <span data-ttu-id="a6136-3226">Préversion</span><span class="sxs-lookup"><span data-stu-id="a6136-3226">Preview release</span></span>
* <span data-ttu-id="a6136-3227">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="a6136-3227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a6136-3228">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="a6136-3228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a6136-3229">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="a6136-3229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3230">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3230">Storage</span></span>

* <span data-ttu-id="a6136-3231">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="a6136-3231">Enabled setting blob tier</span></span>
* <span data-ttu-id="a6136-3232">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="a6136-3232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a6136-3233">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="a6136-3233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a6136-3234">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="a6136-3234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a6136-3235">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a6136-3236">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="a6136-3236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3237">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3237">VM</span></span>

* <span data-ttu-id="a6136-3238">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="a6136-3238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a6136-3239">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="a6136-3239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a6136-3240">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6136-3241">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="a6136-3241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a6136-3242">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="a6136-3242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a6136-3243">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a6136-3244">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3244">August 15, 2017</span></span>

<span data-ttu-id="a6136-3245">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a6136-3245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3246">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3246">ACS</span></span>

* <span data-ttu-id="a6136-3247">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="a6136-3247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3248">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3248">Appservice</span></span>

* <span data-ttu-id="a6136-3249">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="a6136-3249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6136-3250">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a6136-3250">Event Grid</span></span>

* <span data-ttu-id="a6136-3251">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a6136-3251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a6136-3252">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3252">August 11, 2017</span></span>

<span data-ttu-id="a6136-3253">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a6136-3253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3254">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3254">ACS</span></span>

* <span data-ttu-id="a6136-3255">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a6136-3255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-3256">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-3256">Batch</span></span>

* <span data-ttu-id="a6136-3257">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a6136-3257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a6136-3258">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="a6136-3258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a6136-3259">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="a6136-3259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a6136-3260">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="a6136-3260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a6136-3261">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="a6136-3261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a6136-3262">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="a6136-3262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a6136-3263">Composant</span><span class="sxs-lookup"><span data-stu-id="a6136-3263">Component</span></span>

* <span data-ttu-id="a6136-3264">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="a6136-3264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a6136-3265">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-3265">Container</span></span>

* <span data-ttu-id="a6136-3266">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="a6136-3266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a6136-3267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3267">Data Lake Store</span></span>

* <span data-ttu-id="a6136-3268">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="a6136-3268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6136-3269">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a6136-3269">Event Grid</span></span>

* <span data-ttu-id="a6136-3270">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a6136-3270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3271">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3271">Network</span></span>

* <span data-ttu-id="a6136-3272">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="a6136-3272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a6136-3273">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="a6136-3273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a6136-3274">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="a6136-3274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a6136-3275">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="a6136-3275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-3276">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-3276">Profile</span></span>

* <span data-ttu-id="a6136-3277">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="a6136-3277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3278">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3278">Storage</span></span>

* <span data-ttu-id="a6136-3279">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="a6136-3279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3280">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3280">VM</span></span>

* <span data-ttu-id="a6136-3281">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="a6136-3281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a6136-3282">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="a6136-3282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a6136-3283">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="a6136-3283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a6136-3284">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="a6136-3284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a6136-3285">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="a6136-3285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a6136-3286">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3286">July 28, 2017</span></span>

<span data-ttu-id="a6136-3287">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a6136-3287">Version 2.0.12</span></span>

* <span data-ttu-id="a6136-3288">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="a6136-3288">Added container commands</span></span>
* <span data-ttu-id="a6136-3289">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="a6136-3289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a6136-3290">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3290">Core</span></span>

* <span data-ttu-id="a6136-3291">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="a6136-3291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a6136-3292">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="a6136-3292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a6136-3293">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a6136-3293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a6136-3294">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="a6136-3294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a6136-3295">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="a6136-3295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a6136-3296">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="a6136-3296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a6136-3297">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="a6136-3297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a6136-3298">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="a6136-3298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a6136-3299">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="a6136-3299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a6136-3300">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a6136-3300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a6136-3301">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="a6136-3301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a6136-3302">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="a6136-3302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a6136-3303">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-3303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a6136-3304">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a6136-3304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a6136-3305">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a6136-3305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a6136-3306">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="a6136-3306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a6136-3307">ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-3307">ACR</span></span>

* <span data-ttu-id="a6136-3308">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a6136-3308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a6136-3309">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a6136-3309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a6136-3310">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="a6136-3310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a6136-3311">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="a6136-3311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a6136-3312">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="a6136-3312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a6136-3313">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="a6136-3313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3314">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3314">ACS</span></span>

* <span data-ttu-id="a6136-3315">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="a6136-3315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3316">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3316">Appservice</span></span>

* <span data-ttu-id="a6136-3317">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="a6136-3317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a6136-3318">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="a6136-3318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a6136-3319">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="a6136-3319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a6136-3320">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="a6136-3320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a6136-3321">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="a6136-3321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a6136-3322">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="a6136-3322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a6136-3323">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="a6136-3323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a6136-3324">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="a6136-3324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a6136-3325">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="a6136-3325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a6136-3326">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="a6136-3326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a6136-3327">Batch</span><span class="sxs-lookup"><span data-stu-id="a6136-3327">Batch</span></span>

* <span data-ttu-id="a6136-3328">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="a6136-3328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a6136-3329">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="a6136-3329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a6136-3330">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="a6136-3330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a6136-3331">CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-3331">CDN</span></span>

* <span data-ttu-id="a6136-3332">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a6136-3332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a6136-3333">Cloud</span><span class="sxs-lookup"><span data-stu-id="a6136-3333">Cloud</span></span>

* <span data-ttu-id="a6136-3334">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="a6136-3334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a6136-3335">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="a6136-3335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a6136-3336">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="a6136-3336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a6136-3337">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="a6136-3337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a6136-3338">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="a6136-3338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-3339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-3339">CosmosDB</span></span>

* <span data-ttu-id="a6136-3340">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="a6136-3340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a6136-3341">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="a6136-3341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6136-3342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-3342">Data Lake Analytics</span></span>

* <span data-ttu-id="a6136-3343">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="a6136-3343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a6136-3344">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="a6136-3344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a6136-3345">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="a6136-3345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6136-3346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3346">Data Lake Store</span></span>

* <span data-ttu-id="a6136-3347">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a6136-3348">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="a6136-3348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a6136-3349">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a6136-3349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a6136-3350">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a6136-3351">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6136-3351">Interactive</span></span>

* <span data-ttu-id="a6136-3352">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="a6136-3352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a6136-3353">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="a6136-3353">Increased test coverage</span></span>
* <span data-ttu-id="a6136-3354">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="a6136-3354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a6136-3355">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="a6136-3355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a6136-3356">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="a6136-3356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a6136-3357">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="a6136-3357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a6136-3358">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="a6136-3358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a6136-3359">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="a6136-3359">Added `--progress` flag</span></span>
* <span data-ttu-id="a6136-3360">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="a6136-3360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a6136-3361">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="a6136-3361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a6136-3362">IoT</span><span class="sxs-lookup"><span data-stu-id="a6136-3362">IoT</span></span>

* <span data-ttu-id="a6136-3363">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="a6136-3363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a6136-3364">(#3934)</span><span class="sxs-lookup"><span data-stu-id="a6136-3364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6136-3365">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="a6136-3365">Key vault</span></span>

* <span data-ttu-id="a6136-3366">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="a6136-3366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a6136-3367">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a6136-3367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a6136-3368">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a6136-3368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a6136-3369">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a6136-3369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a6136-3370">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a6136-3370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a6136-3371">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="a6136-3371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a6136-3372">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="a6136-3372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a6136-3373">(#3307)</span><span class="sxs-lookup"><span data-stu-id="a6136-3373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a6136-3374">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3374">Lab</span></span>

* <span data-ttu-id="a6136-3375">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="a6136-3375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a6136-3376">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="a6136-3376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-3377">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-3377">Monitor</span></span>

* <span data-ttu-id="a6136-3378">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="a6136-3378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a6136-3379">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="a6136-3379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a6136-3380">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="a6136-3380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a6136-3381">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="a6136-3381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a6136-3382">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="a6136-3382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a6136-3383">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="a6136-3383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a6136-3384">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="a6136-3384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a6136-3385">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="a6136-3385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a6136-3386">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a6136-3386">`location` no longer required</span></span>
  * <span data-ttu-id="a6136-3387">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="a6136-3387">Add name and ID support for target</span></span>
  * <span data-ttu-id="a6136-3388">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-3388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a6136-3389">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a6136-3389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a6136-3390">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="a6136-3390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a6136-3391">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="a6136-3391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a6136-3392">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="a6136-3392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a6136-3393">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3394">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3394">Network</span></span>

* <span data-ttu-id="a6136-3395">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="a6136-3395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a6136-3396">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a6136-3397">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="a6136-3397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a6136-3398">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="a6136-3398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a6136-3399">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a6136-3400">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a6136-3400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a6136-3401">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="a6136-3401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a6136-3402">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="a6136-3402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a6136-3403">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a6136-3403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a6136-3404">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a6136-3404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a6136-3405">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a6136-3406">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="a6136-3406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a6136-3407">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="a6136-3407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a6136-3408">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a6136-3409">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a6136-3410">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a6136-3411">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="a6136-3411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a6136-3412">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="a6136-3412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a6136-3413">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a6136-3414">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a6136-3415">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a6136-3416">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-3416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a6136-3417">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="a6136-3417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a6136-3418">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a6136-3418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a6136-3419">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a6136-3419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a6136-3420">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a6136-3420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a6136-3421">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a6136-3421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-3422">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-3422">Profile</span></span>

* <span data-ttu-id="a6136-3423">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="a6136-3423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a6136-3424">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a6136-3424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a6136-3425">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="a6136-3425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a6136-3426">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="a6136-3426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a6136-3427">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="a6136-3427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6136-3428">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a6136-3428">RDBMS</span></span>

* <span data-ttu-id="a6136-3429">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="a6136-3429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a6136-3430">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="a6136-3430">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a6136-3431">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="a6136-3431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a6136-3432">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="a6136-3432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3433">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3433">Resource</span></span>

* <span data-ttu-id="a6136-3434">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a6136-3435">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a6136-3435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a6136-3436">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a6136-3436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a6136-3437">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="a6136-3437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a6136-3438">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="a6136-3438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a6136-3439">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="a6136-3439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a6136-3440">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="a6136-3440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a6136-3441">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a6136-3441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a6136-3442">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-3442">Role</span></span>

* <span data-ttu-id="a6136-3443">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a6136-3443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a6136-3444">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="a6136-3444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a6136-3445">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="a6136-3445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a6136-3446">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="a6136-3446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a6136-3447">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="a6136-3447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6136-3448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-3448">Service Fabric</span></span>
* <span data-ttu-id="a6136-3449">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="a6136-3449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a6136-3450">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="a6136-3450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a6136-3451">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="a6136-3451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3452">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3452">SQL</span></span>

* <span data-ttu-id="a6136-3453">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="a6136-3453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a6136-3454">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="a6136-3454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a6136-3455">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="a6136-3455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3456">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3456">Storage</span></span>

* <span data-ttu-id="a6136-3457">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="a6136-3457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a6136-3458">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="a6136-3458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a6136-3459">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="a6136-3459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a6136-3460">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="a6136-3460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a6136-3461">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="a6136-3461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a6136-3462">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="a6136-3462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3463">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3463">VM</span></span>

* <span data-ttu-id="a6136-3464">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3464">Support configuring nsg</span></span>
* <span data-ttu-id="a6136-3465">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="a6136-3465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a6136-3466">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="a6136-3466">Support managed service identities</span></span>
* <span data-ttu-id="a6136-3467">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="a6136-3467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a6136-3468">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="a6136-3468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a6136-3469">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3469">May 10, 2017</span></span>

<span data-ttu-id="a6136-3470">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a6136-3470">Version 2.0.6</span></span>

* <span data-ttu-id="a6136-3471">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a6136-3471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a6136-3472">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="a6136-3472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a6136-3473">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a6136-3474">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6136-3474">Include Cognitive Services module</span></span>
* <span data-ttu-id="a6136-3475">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6136-3475">Include Service Fabric module</span></span>
* <span data-ttu-id="a6136-3476">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="a6136-3476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a6136-3477">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="a6136-3477">Add support for CDN commands</span></span>
* <span data-ttu-id="a6136-3478">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="a6136-3478">Remove Container module</span></span>
* <span data-ttu-id="a6136-3479">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="a6136-3479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a6136-3480">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a6136-3480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a6136-3481">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3481">Core</span></span>

* <span data-ttu-id="a6136-3482">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="a6136-3482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a6136-3483">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a6136-3483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a6136-3484">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a6136-3484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a6136-3485">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a6136-3485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a6136-3486">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a6136-3486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a6136-3487">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a6136-3487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a6136-3488">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a6136-3488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a6136-3489">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a6136-3489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a6136-3490">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a6136-3490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a6136-3491">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="a6136-3491">core: Improved performance</span></span>
* <span data-ttu-id="a6136-3492">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="a6136-3492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a6136-3493">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="a6136-3493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3494">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3494">ACS</span></span>

* <span data-ttu-id="a6136-3495">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a6136-3495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a6136-3496">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="a6136-3496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a6136-3497">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="a6136-3497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a6136-3498">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a6136-3498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3499">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3499">AppService</span></span>

* <span data-ttu-id="a6136-3500">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="a6136-3500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a6136-3501">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="a6136-3501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a6136-3502">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="a6136-3502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a6136-3503">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="a6136-3503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a6136-3504">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="a6136-3504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a6136-3505">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a6136-3505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a6136-3506">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="a6136-3506">support slot swap with preview</span></span>
* <span data-ttu-id="a6136-3507">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a6136-3507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a6136-3508">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a6136-3508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6136-3509">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a6136-3509">CosmosDB</span></span>

* <span data-ttu-id="a6136-3510">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a6136-3510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a6136-3511">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="a6136-3511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a6136-3512">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="a6136-3512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a6136-3513">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="a6136-3513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6136-3514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-3514">Data Lake Analytics</span></span>

* <span data-ttu-id="a6136-3515">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="a6136-3515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a6136-3516">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="a6136-3516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a6136-3517">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="a6136-3517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a6136-3518">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="a6136-3518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a6136-3519">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="a6136-3519">Table</span></span>
  * <span data-ttu-id="a6136-3520">Fonction table</span><span class="sxs-lookup"><span data-stu-id="a6136-3520">Table valued function</span></span>
  * <span data-ttu-id="a6136-3521">Affichage</span><span class="sxs-lookup"><span data-stu-id="a6136-3521">View</span></span>
  * <span data-ttu-id="a6136-3522">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="a6136-3522">Table Statistics.</span></span> <span data-ttu-id="a6136-3523">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="a6136-3523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6136-3524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3524">Data Lake Store</span></span>

* <span data-ttu-id="a6136-3525">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="a6136-3525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a6136-3526">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a6136-3526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a6136-3527">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="a6136-3527">missed help for access show.</span></span> <span data-ttu-id="a6136-3528">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="a6136-3528">adding it.</span></span> <span data-ttu-id="a6136-3529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a6136-3529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a6136-3530">Rechercher</span><span class="sxs-lookup"><span data-stu-id="a6136-3530">Find</span></span>

* <span data-ttu-id="a6136-3531">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="a6136-3531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6136-3532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a6136-3532">KeyVault</span></span>

* <span data-ttu-id="a6136-3533">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="a6136-3533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a6136-3534">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="a6136-3534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a6136-3535">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="a6136-3535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a6136-3536">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="a6136-3536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a6136-3537">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a6136-3537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a6136-3538">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3538">Lab</span></span>

* <span data-ttu-id="a6136-3539">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a6136-3540">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a6136-3541">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a6136-3542">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a6136-3543">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="a6136-3543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a6136-3544">Superviser</span><span class="sxs-lookup"><span data-stu-id="a6136-3544">Monitor</span></span>

* <span data-ttu-id="a6136-3545">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a6136-3545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a6136-3546">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a6136-3546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a6136-3547">Réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3547">Network</span></span>

* <span data-ttu-id="a6136-3548">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="a6136-3548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a6136-3549">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a6136-3550">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a6136-3550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a6136-3551">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a6136-3551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a6136-3552">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="a6136-3552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a6136-3553">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a6136-3553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a6136-3554">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a6136-3554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a6136-3555">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a6136-3555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a6136-3556">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="a6136-3556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a6136-3557">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="a6136-3557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a6136-3558">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="a6136-3558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a6136-3559">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a6136-3560">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-3560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a6136-3561">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="a6136-3561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a6136-3562">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a6136-3562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a6136-3563">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="a6136-3563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a6136-3564">Profil</span><span class="sxs-lookup"><span data-stu-id="a6136-3564">Profile</span></span>

* <span data-ttu-id="a6136-3565">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a6136-3565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a6136-3566">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a6136-3566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a6136-3567">Redis</span><span class="sxs-lookup"><span data-stu-id="a6136-3567">Redis</span></span>

* <span data-ttu-id="a6136-3568">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="a6136-3568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a6136-3569">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="a6136-3569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a6136-3570">Ressource</span><span class="sxs-lookup"><span data-stu-id="a6136-3570">Resource</span></span>

* <span data-ttu-id="a6136-3571">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a6136-3571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a6136-3572">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a6136-3572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a6136-3573">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a6136-3573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a6136-3574">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="a6136-3574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a6136-3575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a6136-3575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a6136-3576">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="a6136-3576">Add docs for az lock update.</span></span> <span data-ttu-id="a6136-3577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a6136-3577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a6136-3578">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="a6136-3578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a6136-3579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a6136-3579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a6136-3580">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="a6136-3580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a6136-3581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a6136-3581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a6136-3582">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a6136-3582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a6136-3583">Role</span><span class="sxs-lookup"><span data-stu-id="a6136-3583">Role</span></span>

* <span data-ttu-id="a6136-3584">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a6136-3584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a6136-3585">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a6136-3585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a6136-3586">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a6136-3586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a6136-3587">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="a6136-3587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a6136-3588">SQL</span><span class="sxs-lookup"><span data-stu-id="a6136-3588">SQL</span></span>

* <span data-ttu-id="a6136-3589">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="a6136-3589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a6136-3590">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a6136-3590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a6136-3591">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3591">Storage</span></span>

* <span data-ttu-id="a6136-3592">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="a6136-3592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a6136-3593">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="a6136-3593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a6136-3594">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="a6136-3594">Add support for large block blob upload</span></span>
* <span data-ttu-id="a6136-3595">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="a6136-3595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3596">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3596">VM</span></span>

* <span data-ttu-id="a6136-3597">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="a6136-3597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a6136-3598">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="a6136-3598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a6136-3599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a6136-3599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a6136-3600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a6136-3600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a6136-3601">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="a6136-3601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a6136-3602">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="a6136-3602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a6136-3603">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a6136-3603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a6136-3604">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3604">April 3, 2017</span></span>

<span data-ttu-id="a6136-3605">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a6136-3605">Version 2.0.2</span></span>

<span data-ttu-id="a6136-3606">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="a6136-3606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a6136-3607">Core</span><span class="sxs-lookup"><span data-stu-id="a6136-3607">Core</span></span>

* <span data-ttu-id="a6136-3608">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-3608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a6136-3609">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a6136-3609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a6136-3610">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a6136-3610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a6136-3611">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a6136-3611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a6136-3612">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a6136-3612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a6136-3613">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="a6136-3613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a6136-3614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a6136-3614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a6136-3615">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="a6136-3615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a6136-3616">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="a6136-3616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a6136-3617">ACS</span><span class="sxs-lookup"><span data-stu-id="a6136-3617">ACS</span></span>

* <span data-ttu-id="a6136-3618">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a6136-3618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a6136-3619">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="a6136-3619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a6136-3620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a6136-3620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a6136-3621">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="a6136-3621">Add support for windows clusters.</span></span> <span data-ttu-id="a6136-3622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a6136-3622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a6136-3623">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="a6136-3623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a6136-3624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a6136-3624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a6136-3625">AppService</span><span class="sxs-lookup"><span data-stu-id="a6136-3625">AppService</span></span>

* <span data-ttu-id="a6136-3626">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a6136-3626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a6136-3627">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a6136-3627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a6136-3628">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a6136-3628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a6136-3629">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a6136-3629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a6136-3630">DataLake</span><span class="sxs-lookup"><span data-stu-id="a6136-3630">DataLake</span></span>

* <span data-ttu-id="a6136-3631">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6136-3631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a6136-3632">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6136-3632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a6136-3633">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a6136-3633">DocuemntDB</span></span>

* <span data-ttu-id="a6136-3634">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a6136-3634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a6136-3635">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a6136-3635">VM</span></span>

* <span data-ttu-id="a6136-3636">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a6136-3636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a6136-3637">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a6136-3637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a6136-3638">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a6136-3638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a6136-3639">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a6136-3639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a6136-3640">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a6136-3640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a6136-3641">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="a6136-3641">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="a6136-3642">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a6136-3642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a6136-3643">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="a6136-3643">February 27, 2017</span></span>

<span data-ttu-id="a6136-3644">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a6136-3644">Version 2.0.0</span></span>

<span data-ttu-id="a6136-3645">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="a6136-3645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a6136-3646">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="a6136-3646">Container Service (acs)</span></span>
- <span data-ttu-id="a6136-3647">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="a6136-3647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a6136-3648">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="a6136-3648">Networking</span></span>
- <span data-ttu-id="a6136-3649">Stockage</span><span class="sxs-lookup"><span data-stu-id="a6136-3649">Storage</span></span>

<span data-ttu-id="a6136-3650">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a6136-3650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a6136-3651">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="a6136-3651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a6136-3652">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="a6136-3652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a6136-3653">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="a6136-3653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a6136-3654">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a6136-3654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a6136-3655">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="a6136-3655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a6136-3656">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="a6136-3656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a6136-3657">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a6136-3657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a6136-3658">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a6136-3658">Provide feedback from the command line with the `az feedback` command</span></span>
