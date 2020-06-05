---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/02/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: be0db24ca312825aba03256119d1b5e43afbd902
ms.sourcegitcommit: 62355a77ca59addf7b19db6b95027676e52fd936
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "84275060"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="14cc9-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="14cc9-103">Azure CLI release notes</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="14cc9-104">2 juin 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-104">June 02, 2020</span></span>

<span data-ttu-id="14cc9-105">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-105">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-106">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-106">ACR</span></span>

* <span data-ttu-id="14cc9-107">Correction d’une faute de frappe dans un message d’erreur de création de jeton</span><span class="sxs-lookup"><span data-stu-id="14cc9-107">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-108">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-108">AKS</span></span>

* <span data-ttu-id="14cc9-109">Remplacement de la référence SKU de machine virtuelle par défaut par Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="14cc9-109">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="14cc9-110">Correction de la création d’attribution de rôle pour le cluster MSI plus le sous-réseau personnalisé</span><span class="sxs-lookup"><span data-stu-id="14cc9-110">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-111">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-111">AppService</span></span>

* <span data-ttu-id="14cc9-112">Correctif #12739 az appservice list-locations retourne des emplacements non valides</span><span class="sxs-lookup"><span data-stu-id="14cc9-112">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-113">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-113">ARM</span></span>

* <span data-ttu-id="14cc9-114">`az deployment`: Correction du problème #13159 concernant un message JSON incorrect après la suppression de commentaires et la compression</span><span class="sxs-lookup"><span data-stu-id="14cc9-114">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="14cc9-115">`az resource tag`: Correction du problème #13255 concernant l’étiquetage des ressources avec le type de ressource `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="14cc9-115">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="14cc9-116">Amélioration des exemples pour le module de ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-116">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="14cc9-117">ARO</span><span class="sxs-lookup"><span data-stu-id="14cc9-117">ARO</span></span>

* <span data-ttu-id="14cc9-118">Remplacement de CLIError par un indicateur correct pour --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="14cc9-118">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="14cc9-119">Event Hub</span><span class="sxs-lookup"><span data-stu-id="14cc9-119">EventHub</span></span>

* <span data-ttu-id="14cc9-120">Correction du problème #12406 où l’argument --capture-interval ne mettait pas à jour « intervalInSeconds »</span><span class="sxs-lookup"><span data-stu-id="14cc9-120">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-121">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-121">HDInsight</span></span>

* <span data-ttu-id="14cc9-122">Remplacement de get_json_object par shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="14cc9-122">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-123">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-123">Monitor</span></span>

* <span data-ttu-id="14cc9-124">`az monitor metrics alert` : amélioration de plusieurs messages d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-124">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="14cc9-125">`az monitor diagnostic-settings create` : prise en charge de l’argument --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="14cc9-125">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="14cc9-126">Prise en charge de la récupération de l’espace de travail LA</span><span class="sxs-lookup"><span data-stu-id="14cc9-126">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-127">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-127">Network</span></span>

* <span data-ttu-id="14cc9-128">`az network dns zone` : prise en charge du caractère -</span><span class="sxs-lookup"><span data-stu-id="14cc9-128">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="14cc9-129">`az network vpn-connection ipsec-policy` : remplacement de --sa-lifetime et --sa-max-size par de plus grandes valeurs dans l’exemple</span><span class="sxs-lookup"><span data-stu-id="14cc9-129">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="14cc9-130">Passage du réseau à 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-130">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="14cc9-131">`az network private-endpoint-connection` : prise en charge de la grille d’événement</span><span class="sxs-lookup"><span data-stu-id="14cc9-131">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="14cc9-132">`az network express-route list-route-tables` : correction du bogue qui empêchait de lister les routes sous forme de table</span><span class="sxs-lookup"><span data-stu-id="14cc9-132">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-133">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-133">Packaging</span></span>

* <span data-ttu-id="14cc9-134">Ajout du package Ubuntu Focal</span><span class="sxs-lookup"><span data-stu-id="14cc9-134">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-135">RBAC</span></span>

* <span data-ttu-id="14cc9-136">`az ad sp credential reset` : modification de la génération d’informations d’identification pour éviter des caractères spéciaux posant problème</span><span class="sxs-lookup"><span data-stu-id="14cc9-136">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-137">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-137">Redis</span></span>

* <span data-ttu-id="14cc9-138">Correctif #13529 : Modification de la documentation du paramètre enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="14cc9-138">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-139">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-139">Storage</span></span>

* <span data-ttu-id="14cc9-140">`az storage copy`: Ajout du paramètre `--follow-symlinks` pour prendre en charge les symlinks</span><span class="sxs-lookup"><span data-stu-id="14cc9-140">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="14cc9-141">Activer le contexte local pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-141">Enable local context for storage account</span></span>
* <span data-ttu-id="14cc9-142">`az storage logging`: Correction du problème #11969 pour améliorer le message d’erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-142">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="14cc9-143">19 mai 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-143">May 19, 2020</span></span>

<span data-ttu-id="14cc9-144">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-144">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-145">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-145">ACR</span></span>

* <span data-ttu-id="14cc9-146">Ajout du délai d’expiration par défaut de 5 minutes pour toute demande à ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-146">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="14cc9-147">Prise en charge de la désactivation de l’accès au réseau public</span><span class="sxs-lookup"><span data-stu-id="14cc9-147">Support disable public network access</span></span>
* <span data-ttu-id="14cc9-148">`az acr token create` : exposition de l’argument --days</span><span class="sxs-lookup"><span data-stu-id="14cc9-148">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="14cc9-149">`az acr import` : acceptation des valeurs de l’argument --source qui contiennent le nom du serveur de connexion résultant d’une correction côté du client</span><span class="sxs-lookup"><span data-stu-id="14cc9-149">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-150">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-150">ACS</span></span>

* <span data-ttu-id="14cc9-151">Correctif de bogue : suppression du nettoyage des champs pour les champs qui n’existent plus</span><span class="sxs-lookup"><span data-stu-id="14cc9-151">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-152">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-152">AKS</span></span>

* <span data-ttu-id="14cc9-153">Mise à jour du contexte de l’aide pour la commande uptime-sla</span><span class="sxs-lookup"><span data-stu-id="14cc9-153">Update uptime-sla command help context</span></span>
* <span data-ttu-id="14cc9-154">Suppression de la vérification de plage pour la mise à jour du nombre minimal pour l’autoscaler</span><span class="sxs-lookup"><span data-stu-id="14cc9-154">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="14cc9-155">Correction de l’interface CLI qui n’échoue pas quand l’utilisateur spécifie uniquement un mot de passe Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-155">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-156">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-156">AMS</span></span>

* <span data-ttu-id="14cc9-157">`az ams transform create`: Ajout de la possibilité de créer une transformation avec une présélection FaceDetector</span><span class="sxs-lookup"><span data-stu-id="14cc9-157">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="14cc9-158">`az ams content-key-policy create` : Ajout de la possibilité de créer une stratégie de clé de contenu FairPlay avec une configuration de location hors connexion</span><span class="sxs-lookup"><span data-stu-id="14cc9-158">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-159">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-159">AppConfig</span></span>

* <span data-ttu-id="14cc9-160">Correction de bogue pour les valeurs de clé de liste avec champs</span><span class="sxs-lookup"><span data-stu-id="14cc9-160">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-161">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-161">AppService</span></span>

* <span data-ttu-id="14cc9-162">`az functionapp create`: AzureWebJobsDashboard ne sera défini que si AppInsights est désactivé</span><span class="sxs-lookup"><span data-stu-id="14cc9-162">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="14cc9-163">Correctif #10664 – Intégration de réseau virtuel – Problème de vérification d’emplacement et correctif #13257 – Échec d’az webapp up quand un groupe de ressources doit être créé</span><span class="sxs-lookup"><span data-stu-id="14cc9-163">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="14cc9-164">`az webapp|functionapp config ssl import`: Recherche dans le coffre de clés des groupes de ressources d’un abonnement et amélioration de l’aide et des exemples.</span><span class="sxs-lookup"><span data-stu-id="14cc9-164">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="14cc9-165">Intégration du contexte local pour App Service</span><span class="sxs-lookup"><span data-stu-id="14cc9-165">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-166">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-166">ARM</span></span>

* <span data-ttu-id="14cc9-167">`az deployment`: Correction du problème lié à l’absence de retour de templateLink pendant le déploiement ou la validation de template-uri</span><span class="sxs-lookup"><span data-stu-id="14cc9-167">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="14cc9-168">`az deployment`: Correction du problème lié au fait que les caractères spécialement encodés ne sont pas pris en charge par le déploiement/la validation</span><span class="sxs-lookup"><span data-stu-id="14cc9-168">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="14cc9-169">`az deployment sub/group what-if`: Correction de l’alignement de tableau et gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-169">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="14cc9-170">`az deployment operation`: Modification des informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="14cc9-170">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="14cc9-171">ARO</span><span class="sxs-lookup"><span data-stu-id="14cc9-171">ARO</span></span>

* <span data-ttu-id="14cc9-172">Ajout d’exemples pour az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="14cc9-172">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="14cc9-173">Ajout de la fonction generate_random_id</span><span class="sxs-lookup"><span data-stu-id="14cc9-173">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-174">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-174">Backup</span></span>

* <span data-ttu-id="14cc9-175">Autorisation de FriendlyName dans la commande d’activation de la protection pour AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="14cc9-175">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="14cc9-176">Correction dans la commande IaasVM restore-disks</span><span class="sxs-lookup"><span data-stu-id="14cc9-176">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="14cc9-177">Ajout de BackupManagementType « MAB » à la commande item list</span><span class="sxs-lookup"><span data-stu-id="14cc9-177">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="14cc9-178">Ajout de la prise en charge des nouvelles tentatives de mise à jour de stratégie pour les éléments en échec.</span><span class="sxs-lookup"><span data-stu-id="14cc9-178">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="14cc9-179">Ajout d’une fonctionnalité de reprise de protection pour Machine Virtuelle Azure</span><span class="sxs-lookup"><span data-stu-id="14cc9-179">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="14cc9-180">Ajout d’une prise en charge permettant de spécifier ResourceGroup pour stocker instantRP pendant la création ou la modification d’une stratégie</span><span class="sxs-lookup"><span data-stu-id="14cc9-180">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="14cc9-181">CI</span><span class="sxs-lookup"><span data-stu-id="14cc9-181">CI</span></span>

* <span data-ttu-id="14cc9-182">Prise en charge de flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-182">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-183">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-183">Compute</span></span>

* <span data-ttu-id="14cc9-184">Nouvelle commande az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="14cc9-184">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="14cc9-185">`az vm list-skus`: Mise à jour du comportement de --zone ; retourne désormais tous les types de références SKU</span><span class="sxs-lookup"><span data-stu-id="14cc9-185">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-186">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-186">Core</span></span>

* <span data-ttu-id="14cc9-187">Mise à jour de l’état activé/désactivé du contexte local vers le niveau utilisateur global</span><span class="sxs-lookup"><span data-stu-id="14cc9-187">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-188">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-188">Extension</span></span>

* <span data-ttu-id="14cc9-189">`az extension add`: Ajout de --system pour permettre l’installation d’extensions dans un chemin système</span><span class="sxs-lookup"><span data-stu-id="14cc9-189">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="14cc9-190">Prise en charge de .egg-info pour stocker les métadonnées d’extension de type wheel</span><span class="sxs-lookup"><span data-stu-id="14cc9-190">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-191">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-191">IoT</span></span>

* <span data-ttu-id="14cc9-192">`az iot`: Mise à jour du message de reconnaissance de la première extension exécutée par le module de commande IoT vers l’ID moderne non déconseillé `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-192">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="14cc9-193">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="14cc9-193">IoT Hub</span></span>

* <span data-ttu-id="14cc9-194">Prise en charge des commandes de l’API 2020-03-01 et de l’isolement réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-194">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="14cc9-195">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="14cc9-195">NetAppFiles</span></span>

* <span data-ttu-id="14cc9-196">`az volume create`: Ajout de snapshot-id en tant que paramètre pour créer un volume, permettant ainsi aux utilisateurs de créer un volume à partir d’une capture instantanée existante.</span><span class="sxs-lookup"><span data-stu-id="14cc9-196">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-197">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-197">Network</span></span>

* <span data-ttu-id="14cc9-198">Correction du changement non souhaité de la valeur TTL pour dns add-record</span><span class="sxs-lookup"><span data-stu-id="14cc9-198">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="14cc9-199">`az network public-ip create`: Information à l’intention des clients pour les prévenir d’un changement cassant imminent</span><span class="sxs-lookup"><span data-stu-id="14cc9-199">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="14cc9-200">Prise en charge des commandes génériques pour un scénario de liaison privée</span><span class="sxs-lookup"><span data-stu-id="14cc9-200">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="14cc9-201">`az network private-endpoint-connection`: Prise en charge des types mysql, postgre et mariadb</span><span class="sxs-lookup"><span data-stu-id="14cc9-201">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="14cc9-202">`az network private-endpoint-connection`: Prise en charge des types cosmosdb</span><span class="sxs-lookup"><span data-stu-id="14cc9-202">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="14cc9-203">`az network private-endpoint` : dépréciation de --group-ids et redirection vers --group-id</span><span class="sxs-lookup"><span data-stu-id="14cc9-203">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="14cc9-204">Output</span><span class="sxs-lookup"><span data-stu-id="14cc9-204">Output</span></span>

* <span data-ttu-id="14cc9-205">Affichage de l’instruction update dans find, feedback et --help</span><span class="sxs-lookup"><span data-stu-id="14cc9-205">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-206">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-206">Packaging</span></span>

* <span data-ttu-id="14cc9-207">Génération de packages MSI/Homebrew avec les dépendances résolues selon requirements.txt</span><span class="sxs-lookup"><span data-stu-id="14cc9-207">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-208">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-208">RBAC</span></span>

* <span data-ttu-id="14cc9-209">`az ad sp credential reset` : correction de la génération d’informations d’identification faibles</span><span class="sxs-lookup"><span data-stu-id="14cc9-209">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-210">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-210">Storage</span></span>

* <span data-ttu-id="14cc9-211">`az storage account file-service-properties update/show`: Ajout de la prise en charge des propriétés de fichier pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-211">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="14cc9-212">`az storage container create`: Correction #13373 par l’ajout d’un validateur pour l’accès public</span><span class="sxs-lookup"><span data-stu-id="14cc9-212">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="14cc9-213">Ajout de la prise en charge d’ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="14cc9-213">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="14cc9-214">`az storage blob sync`: Prise en charge d’`--connection-string`</span><span class="sxs-lookup"><span data-stu-id="14cc9-214">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="14cc9-215">`az storage blob sync`: Correction du message d’erreur incorrect quand azcopy ne trouve pas l’emplacement d’installation</span><span class="sxs-lookup"><span data-stu-id="14cc9-215">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="14cc9-216">30 avril 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-216">April 30, 2020</span></span>

<span data-ttu-id="14cc9-217">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="14cc9-217">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-218">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-218">ACR</span></span>

* <span data-ttu-id="14cc9-219">`az acr check-health`: Correction de « DOCKER_PULL_ERROR » sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-219">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-220">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-220">Compute</span></span>

* <span data-ttu-id="14cc9-221">`az vm list-ip-addresses`: Gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-221">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="14cc9-222">Correction d’un bogue de vm create si endpoint_vm_image_alias_doc n’est pas défini dans le profil cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-222">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="14cc9-223">`az vmss create`: Ajout de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="14cc9-223">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-224">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-224">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-225">`az cosmosdb create/update` : ajout de la prise en charge de add --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="14cc9-225">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-226">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-226">Extension</span></span>

* <span data-ttu-id="14cc9-227">Correction du chargement des métadonnées incorrectes pour l’extension du type de roulette</span><span class="sxs-lookup"><span data-stu-id="14cc9-227">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-228">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-228">Packaging</span></span>

* <span data-ttu-id="14cc9-229">Ajout du script az pour Git Bash/Cygwin sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-229">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-230">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-230">SQL</span></span>

* <span data-ttu-id="14cc9-231">`az sql instance-pool`: Ajout d’un groupe de commandes pour les pools d’instances</span><span class="sxs-lookup"><span data-stu-id="14cc9-231">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-232">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-232">Storage</span></span>

* <span data-ttu-id="14cc9-233">Mise à niveau du package azure-multiapi-storage vers 0.3.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-233">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="14cc9-234">Prise en charge de GZRS pour la création et la mise à jour de comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-234">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="14cc9-235">`az storage account failover`: Ajout de la prise en charge du basculement de comptes de stockage grs/gzrs</span><span class="sxs-lookup"><span data-stu-id="14cc9-235">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="14cc9-236">`az storage blob upload`: Ajout du paramètre --encryption-scope pour prendre en charge la spécification des informations d’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-236">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="14cc9-237">28 avril 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-237">April 28, 2020</span></span>

<span data-ttu-id="14cc9-238">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-238">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-239">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-239">ACS</span></span>

* <span data-ttu-id="14cc9-240">[CHANGEMENT CASSANT] du paramètre az openshift create: remove --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="14cc9-240">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="14cc9-241">`az openshift create` : Ajout d’indicateurs pour prendre en charge un cluster privé.</span><span class="sxs-lookup"><span data-stu-id="14cc9-241">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="14cc9-242">`az openshift` : Mise à niveau vers la version d’API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-242">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="14cc9-243">`az openshift` : Ajout de la commande `update`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-243">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-244">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-244">AKS</span></span>

* <span data-ttu-id="14cc9-245">`az aks create`: Ajout de la prise en charge de Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-245">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-246">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-246">AppService</span></span>

* <span data-ttu-id="14cc9-247">`az webapp deployment source config-zip` : Suppression de sleep après request.get()</span><span class="sxs-lookup"><span data-stu-id="14cc9-247">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-248">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-248">ARM</span></span>

* <span data-ttu-id="14cc9-249">Ajout de commandes What-If de déploiement de modèles</span><span class="sxs-lookup"><span data-stu-id="14cc9-249">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="14cc9-250">ARO</span><span class="sxs-lookup"><span data-stu-id="14cc9-250">ARO</span></span>

* <span data-ttu-id="14cc9-251">`az aro`: Correction de la sortie de table</span><span class="sxs-lookup"><span data-stu-id="14cc9-251">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="14cc9-252">CI</span><span class="sxs-lookup"><span data-stu-id="14cc9-252">CI</span></span>

* <span data-ttu-id="14cc9-253">Intégration de pytest et dépréciation de nose pour le test d’automatisation</span><span class="sxs-lookup"><span data-stu-id="14cc9-253">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-254">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-254">Compute</span></span>

* <span data-ttu-id="14cc9-255">`az vmss disk detach` : Correction du problème NoneType du disque de données</span><span class="sxs-lookup"><span data-stu-id="14cc9-255">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="14cc9-256">`az vm availability-set list`: Prise en charge de l’affichage de la liste de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="14cc9-256">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="14cc9-257">`az vm list-skus`: Correction du problème d’affichage du format de table</span><span class="sxs-lookup"><span data-stu-id="14cc9-257">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-258">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-258">KeyVault</span></span>

* <span data-ttu-id="14cc9-259">Ajout d’un nouveau paramètre `--enable-rbac-authorization` lors de la création ou de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-259">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-260">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-260">Monitor</span></span>

* <span data-ttu-id="14cc9-261">Prise en charge des fonctionnalités CMK de cluster LA</span><span class="sxs-lookup"><span data-stu-id="14cc9-261">Support LA cluster CMK features</span></span>
* <span data-ttu-id="14cc9-262">`az monitor log-analytics workspace linked-storage` : Prise en charge des fonctionnalités BYOS</span><span class="sxs-lookup"><span data-stu-id="14cc9-262">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-263">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-263">Network</span></span>

* <span data-ttu-id="14cc9-264">`az network security-partner` : Prise en charge du fournisseur de partenaire de sécurité</span><span class="sxs-lookup"><span data-stu-id="14cc9-264">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="14cc9-265">Privatedns</span><span class="sxs-lookup"><span data-stu-id="14cc9-265">Privatedns</span></span>

* <span data-ttu-id="14cc9-266">Ajout d’une fonctionnalité dans une zone DNS privée pour importer/exporter un fichier de zone</span><span class="sxs-lookup"><span data-stu-id="14cc9-266">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="14cc9-267">21 avril 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-267">April 21, 2020</span></span>

<span data-ttu-id="14cc9-268">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-268">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-269">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-269">ACR</span></span>

* <span data-ttu-id="14cc9-270">`az acr run --cmd` : désactivation du remplacement du répertoire de travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-270">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="14cc9-271">Prise en charge du point de terminaison de données dédié</span><span class="sxs-lookup"><span data-stu-id="14cc9-271">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-272">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-272">AKS</span></span>

* <span data-ttu-id="14cc9-273">`az aks list -o table` doit afficher privateFqdn comme nom de domaine complet pour les clusters privés</span><span class="sxs-lookup"><span data-stu-id="14cc9-273">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="14cc9-274">Ajout de --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="14cc9-274">Add --uptime-sla</span></span>
* <span data-ttu-id="14cc9-275">Mise à jour du package containerservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-275">Update containerservice package</span></span>
* <span data-ttu-id="14cc9-276">Ajout de la prise en charge de l’adresse IP publique de nœud</span><span class="sxs-lookup"><span data-stu-id="14cc9-276">Add node public IP support</span></span>
* <span data-ttu-id="14cc9-277">Correction d’une faute de frappe dans la commande d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-277">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-278">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-278">AppConfig</span></span>

* <span data-ttu-id="14cc9-279">Résolution de la référence du coffre de clés pour la liste Key Vault et les commandes d’exportation</span><span class="sxs-lookup"><span data-stu-id="14cc9-279">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="14cc9-280">Résolution de bogue pour les valeurs de clé de liste</span><span class="sxs-lookup"><span data-stu-id="14cc9-280">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-281">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-281">AppService</span></span>

* <span data-ttu-id="14cc9-282">`az functionapp create`: Modification de la façon dont linuxFxVersion était défini pour les applications de fonction dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="14cc9-282">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="14cc9-283">Cela doit résoudre un bogue qui empêchait la création d’applications de consommation dotnet linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-283">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="14cc9-284">[CHANGEMENT CASSANT] `az webapp create` : correctif pour conserver les paramètres d’application existants avec az webapp create</span><span class="sxs-lookup"><span data-stu-id="14cc9-284">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="14cc9-285">[CHANGEMENT CASSANT] `az webapp up` : correctif pour créer un groupe de ressources pour la commande az webapp up lors de l’utilisation de l’indicateur -g</span><span class="sxs-lookup"><span data-stu-id="14cc9-285">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="14cc9-286">[CHANGEMENT CASSANT] `az webapp config` : correctif pour afficher des valeurs pour la sortie non-JSON avec la liste de chaînes de connexion az webapp config</span><span class="sxs-lookup"><span data-stu-id="14cc9-286">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-287">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-287">ARM</span></span>

* <span data-ttu-id="14cc9-288">`az deployment create/validate`: Ajout d’un paramètre `--no-prompt` pour prendre en charge le saut de l’invite de paramètres manquants pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-288">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="14cc9-289">`az deployment group/mg/sub/tenant validate`: Prise en charge de commentaires dans le fichier de paramètres de déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-289">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="14cc9-290">`az deployment`: Suppression de `is_preview` pour le paramètre `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="14cc9-290">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="14cc9-291">`az deployment group/mg/sub/tenant cancel`: Prise en charge de l’annulation du déploiement pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-291">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="14cc9-292">`az deployment group/mg/sub/tenant validate`: Amélioration du message d’erreur lors de l’échec de la vérification du déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-292">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="14cc9-293">`az deployment-scripts`: Ajout de nouvelles commandes pour DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="14cc9-293">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="14cc9-294">`az resource tag`: Ajout du paramètre `--is-incremental` pour prendre en charge l’ajout incrémentiel de balises aux ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-294">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="14cc9-295">ARO</span><span class="sxs-lookup"><span data-stu-id="14cc9-295">ARO</span></span>

* <span data-ttu-id="14cc9-296">`az aro`:  Ajout du module de commande aro Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="14cc9-296">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-297">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-297">Batch</span></span>

* <span data-ttu-id="14cc9-298">Mise à jour de l’API Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-298">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-299">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-299">Compute</span></span>

* <span data-ttu-id="14cc9-300">`az sig image-version create`: Ajout d’un type de compte de stockage Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="14cc9-300">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="14cc9-301">`az vmss update`: Correction d’un problème de mise à jour de notification d’arrêt</span><span class="sxs-lookup"><span data-stu-id="14cc9-301">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="14cc9-302">`az vm/vmss create`: Ajout de la prise en charge de la version d’image spécialisée</span><span class="sxs-lookup"><span data-stu-id="14cc9-302">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="14cc9-303">Version de l’API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-303">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="14cc9-304">`az sig image-version create`: Ajout de --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="14cc9-304">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="14cc9-305">Correction de l’échec des tests lors d’une exécution en série en raison d’un nom de coffre de clés en double dans le cache en mémoire global</span><span class="sxs-lookup"><span data-stu-id="14cc9-305">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-306">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-306">CosmosDB</span></span>

* <span data-ttu-id="14cc9-307">Prise en charge d’`az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="14cc9-307">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="14cc9-308">IoT Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-308">IoT Central</span></span>

* <span data-ttu-id="14cc9-309">Dépréciation d’`az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="14cc9-309">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="14cc9-310">Ajout du module de commande `az iot central`</span><span class="sxs-lookup"><span data-stu-id="14cc9-310">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-311">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-311">Monitor</span></span>

* <span data-ttu-id="14cc9-312">Prise en charge du scénario de lien privé pour la supervision</span><span class="sxs-lookup"><span data-stu-id="14cc9-312">Support private link scenario for monitor</span></span>
* <span data-ttu-id="14cc9-313">Correction du mode de simulation incorrect dans test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="14cc9-313">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-314">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-314">Network</span></span>

* <span data-ttu-id="14cc9-315">Dépréciation de la référence sku pour la commande de mise à jour de l’adresse IP publique</span><span class="sxs-lookup"><span data-stu-id="14cc9-315">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="14cc9-316">`az network private-endpoint`: Prise en charge du groupe de zones DNS privées</span><span class="sxs-lookup"><span data-stu-id="14cc9-316">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="14cc9-317">Activation de la fonctionnalité de contexte local pour le paramètre de réseau virtuel/sous-réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-317">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="14cc9-318">Correction d’un exemple d’utilisation incorrect dans test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="14cc9-318">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-319">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-319">Packaging</span></span>

* <span data-ttu-id="14cc9-320">Suppression de la prise en charge d’un package Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="14cc9-320">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-321">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-321">RBAC</span></span>

* <span data-ttu-id="14cc9-322">`az ad app create/update` : prise en charge de --optional-claims en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="14cc9-322">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-323">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-323">RDBMS</span></span>

* <span data-ttu-id="14cc9-324">Ajout des commandes d’administrateur Azure Active Directory pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-324">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14cc9-325">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-325">Service Fabric</span></span>

* <span data-ttu-id="14cc9-326">Correctif n  12891 : `az sf application update --application-parameters` supprime les anciens paramètres qui ne sont pas dans la demande</span><span class="sxs-lookup"><span data-stu-id="14cc9-326">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="14cc9-327">Correctif n  12470, az sf create cluster, résolution de bogues dans la durabilité et la fiabilité des mises à jour, et recherche de groupes identiques de machines virtuelles correctement dans le code en fonction d’un nom de type de nœud</span><span class="sxs-lookup"><span data-stu-id="14cc9-327">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-328">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-328">SQL</span></span>

* <span data-ttu-id="14cc9-329">Ajout d’`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="14cc9-329">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="14cc9-330">`az sql midb` : mise à jour/affichage de la stratégie de conservation à long terme, affichage/suppression des sauvegardes de conservation à long terme, restauration de la sauvegarde de conservation à long terme</span><span class="sxs-lookup"><span data-stu-id="14cc9-330">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-331">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-331">Storage</span></span>

* <span data-ttu-id="14cc9-332">Mise à niveau d’azure-mgmt-storage vers 9.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-332">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="14cc9-333">`az storage logging off`: Prise en charge de la désactivation de la journalisation pour un compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-333">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="14cc9-334">`az storage account update`: Activation de la rotation automatique de la clé pour CMK</span><span class="sxs-lookup"><span data-stu-id="14cc9-334">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="14cc9-335">`az storage account encryption-scope create/update/list/show`: Ajout de la prise en charge de la personnalisation de l’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-335">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="14cc9-336">`az storage container create`: Ajout de --default-encryption-scope et --deny-encryption-scope-override pour définir l’étendue du chiffrement de niveau de conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-336">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="14cc9-337">Enquête</span><span class="sxs-lookup"><span data-stu-id="14cc9-337">Survey</span></span>

* <span data-ttu-id="14cc9-338">Ajout d’une instruction switch pour désactiver le lien d’enquête</span><span class="sxs-lookup"><span data-stu-id="14cc9-338">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="14cc9-339">01 avril 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-339">April 01, 2020</span></span>

<span data-ttu-id="14cc9-340">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="14cc9-340">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-341">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-341">ACR</span></span>

* <span data-ttu-id="14cc9-342">Correction d’une version incorrecte d’azure-mgmt-containerregistry pour Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-342">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-343">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-343">Profile</span></span>

* <span data-ttu-id="14cc9-344">az login : Correction des échecs de connexion avec les profils cloud autres que `latest`</span><span class="sxs-lookup"><span data-stu-id="14cc9-344">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="14cc9-345">31 mars 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-345">March 31, 2020</span></span>

<span data-ttu-id="14cc9-346">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-346">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-347">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-347">ACR</span></span>

* <span data-ttu-id="14cc9-348">'az acr task update' : exception du pointeur null</span><span class="sxs-lookup"><span data-stu-id="14cc9-348">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="14cc9-349">`az acr import`: Modification de l’aide et du message d’erreur pour clarifier l’utilisation de --source et --registry</span><span class="sxs-lookup"><span data-stu-id="14cc9-349">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="14cc9-350">Ajout d’un validateur pour l’argument 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="14cc9-350">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="14cc9-351">`az acr login` : Suppression de l’indicateur de préversion sur '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="14cc9-351">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="14cc9-352">[CHANGEMENT CASSANT] Suppression du paramètre de branche 'az acr task create/update'</span><span class="sxs-lookup"><span data-stu-id="14cc9-352">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="14cc9-353">'az acr task update' : Le client peut maintenant mettre à jour le contexte, git-token et/ou les déclencheurs individuellement</span><span class="sxs-lookup"><span data-stu-id="14cc9-353">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="14cc9-354">'az acr agentpool' : nouvelle fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="14cc9-354">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-355">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-355">AKS</span></span>

* <span data-ttu-id="14cc9-356">Correction d’apiServerAccessProfile lors de la mise à jour de --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="14cc9-356">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="14cc9-357">aks update : Remplacement des adresses IP sortantes par des valeurs d’entrée lors de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-357">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="14cc9-358">Pas de création de SPN pour les clusters MSI et prise en charge de l’attachement d’acr à des clusters MSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-358">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-359">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-359">AMS</span></span>

* <span data-ttu-id="14cc9-360">Correctif #12469 : échec de l’ajout de Fairplay content-key-policy en raison de problèmes avec le paramètre « ask »</span><span class="sxs-lookup"><span data-stu-id="14cc9-360">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-361">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-361">AppConfig</span></span>

* <span data-ttu-id="14cc9-362">Ajout de --skip-keyvault pour l’exportation de kv</span><span class="sxs-lookup"><span data-stu-id="14cc9-362">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-363">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-363">AppService</span></span>

* <span data-ttu-id="14cc9-364">Correctif #12509 : Suppression de la balise d’az webapp up par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-364">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="14cc9-365">az functionapp create : Mise à jour du menu d’aide --runtime-version et ajout d’un avertissement quand l’utilisateur spécifie --runtime-version pour dotnet</span><span class="sxs-lookup"><span data-stu-id="14cc9-365">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="14cc9-366">az functionapp create : Mise à jour du mode de définition de javaVersion pour les applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-366">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-367">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-367">ARM</span></span>

* <span data-ttu-id="14cc9-368">az deployment create/validate : Utilisation du --handle-extended-json-format par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-368">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="14cc9-369">az lock create : Ajout d’exemples de création de sous-ressources dans la documentation d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-369">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="14cc9-370">az deployment {group/mg/sub/tenant} list : Prise en charge du filtrage provisioningState</span><span class="sxs-lookup"><span data-stu-id="14cc9-370">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="14cc9-371">az deployment : Correction du bogue d’analyse pour les commentaires sous le dernier argument</span><span class="sxs-lookup"><span data-stu-id="14cc9-371">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-372">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-372">Backup</span></span>

* <span data-ttu-id="14cc9-373">Ajout de plusieurs fonctionnalités de restauration de fichiers</span><span class="sxs-lookup"><span data-stu-id="14cc9-373">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="14cc9-374">Ajout de la prise en charge de la sauvegarde des disques de système d’exploitation uniquement</span><span class="sxs-lookup"><span data-stu-id="14cc9-374">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="14cc9-375">Ajout du paramètre restore-as-unmanaged-disk pour spécifier une restauration non gérée</span><span class="sxs-lookup"><span data-stu-id="14cc9-375">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-376">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-376">Compute</span></span>

* <span data-ttu-id="14cc9-377">az vm create : Ajout de l’option NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="14cc9-377">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="14cc9-378">az vmss create/update : suppression de la balise d’aperçu des réparations automatiques vmss</span><span class="sxs-lookup"><span data-stu-id="14cc9-378">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="14cc9-379">az vm update : Prise en charge de --workspace</span><span class="sxs-lookup"><span data-stu-id="14cc9-379">az vm update: Support --workspace</span></span>
* <span data-ttu-id="14cc9-380">Correction d’un bogue dans le code d’initialisation VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="14cc9-380">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="14cc9-381">Mise à niveau de VMAccessAgent vers la version 2.4</span><span class="sxs-lookup"><span data-stu-id="14cc9-381">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="14cc9-382">az vmss set-orchestration-service-state : prise en charge de l’état de la définition du service d’orchestration vmss</span><span class="sxs-lookup"><span data-stu-id="14cc9-382">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="14cc9-383">Mise à niveau de la version d’API de disque vers la version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-383">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="14cc9-384">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="14cc9-384">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-385">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-385">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-386">Correction de l’option --type manquante pour les redirections de dépréciation</span><span class="sxs-lookup"><span data-stu-id="14cc9-386">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="14cc9-387">Docker</span><span class="sxs-lookup"><span data-stu-id="14cc9-387">Docker</span></span>

* <span data-ttu-id="14cc9-388">Mise à jour vers Alpine 3.11 et Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="14cc9-388">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-389">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-389">Extension</span></span>

* <span data-ttu-id="14cc9-390">Autorisation de charger des extensions dans le chemin système via des packages</span><span class="sxs-lookup"><span data-stu-id="14cc9-390">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-391">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-391">HDInsight</span></span>

* <span data-ttu-id="14cc9-392">(az hdinsight create:) Les clients du support spécifient une version TLS minimale prise en charge à l’aide du paramètre `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-392">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="14cc9-393">La valeur autorisée est 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="14cc9-393">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-394">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-394">IoT</span></span>

* <span data-ttu-id="14cc9-395">Ajout de codeowner</span><span class="sxs-lookup"><span data-stu-id="14cc9-395">Add codeowner</span></span>
* <span data-ttu-id="14cc9-396">az iot hub create : changement de la référence SKU par défaut S1 en F1</span><span class="sxs-lookup"><span data-stu-id="14cc9-396">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="14cc9-397">iot hub : Prise en charge d’IotHub dans le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-397">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="14cc9-398">IotCentral</span><span class="sxs-lookup"><span data-stu-id="14cc9-398">IoTCentral</span></span>

* <span data-ttu-id="14cc9-399">Mise à jour des détails d’erreur, du modèle d’application par défaut et du message d’invite</span><span class="sxs-lookup"><span data-stu-id="14cc9-399">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-400">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-400">KeyVault</span></span>

* <span data-ttu-id="14cc9-401">Prise en charge de la sauvegarde/restauration de certificat</span><span class="sxs-lookup"><span data-stu-id="14cc9-401">Support certificate backup/restore</span></span>
* <span data-ttu-id="14cc9-402">keyvault create/update : Prise en charge de --retention-days</span><span class="sxs-lookup"><span data-stu-id="14cc9-402">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="14cc9-403">Plus d’affichage des clés/secrets managés lors du listing</span><span class="sxs-lookup"><span data-stu-id="14cc9-403">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="14cc9-404">az keyvault create : prise en charge de `--network-acls`, `--network-acls-ips` et `--network-acls-vnets` pour spécifier des règles réseau lors de la création de coffres</span><span class="sxs-lookup"><span data-stu-id="14cc9-404">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="14cc9-405">Verrouillage</span><span class="sxs-lookup"><span data-stu-id="14cc9-405">Lock</span></span>

* <span data-ttu-id="14cc9-406">Correction de bogue pour az lock delete : az lock delete ne fonctionne pas sur Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-406">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-407">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-407">Monitor</span></span>

* <span data-ttu-id="14cc9-408">az monitor clone : prise en charge des règles de clonage de métriques d’une ressource à une autre</span><span class="sxs-lookup"><span data-stu-id="14cc9-408">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="14cc9-409">Correctif IcM179210086 : impossible de créer une alerte de métrique personnalisée pour la métrique Application Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-409">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="14cc9-410">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="14cc9-410">NetAppFiles</span></span>

* <span data-ttu-id="14cc9-411">az volume create : Autorisation des volumes de protection des données à ajouter des opérations de réplication : approuver, suspendre, reprendre, état, supprimer</span><span class="sxs-lookup"><span data-stu-id="14cc9-411">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-412">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-412">Network</span></span>

* <span data-ttu-id="14cc9-413">az network application-gateway waf-policy managed-rule rule-set add : prise en charge de Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="14cc9-413">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="14cc9-414">network watcher flow-log show: correction d’une information de dépréciation fausse</span><span class="sxs-lookup"><span data-stu-id="14cc9-414">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="14cc9-415">Prise en charge des noms d’hôte dans l’écouteur de passerelle d’application</span><span class="sxs-lookup"><span data-stu-id="14cc9-415">support host names in application gateway listener</span></span>
* <span data-ttu-id="14cc9-416">az network nat gateway : prise en charge de la création d’une ressource vide sans IP publique ni préfixe d’IP publique</span><span class="sxs-lookup"><span data-stu-id="14cc9-416">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="14cc9-417">Prise en charge de la génération de passerelles VPN</span><span class="sxs-lookup"><span data-stu-id="14cc9-417">Support vpn gateway generation</span></span>
* <span data-ttu-id="14cc9-418">Prise en charge de `--if-none-match` dans `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="14cc9-418">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-419">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-419">Packaging</span></span>

* <span data-ttu-id="14cc9-420">Arrêt de la prise en charge de Python 3.5</span><span class="sxs-lookup"><span data-stu-id="14cc9-420">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-421">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-421">Profile</span></span>

* <span data-ttu-id="14cc9-422">az login : Affichage d’un avertissement pour l’erreur MFA</span><span class="sxs-lookup"><span data-stu-id="14cc9-422">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-423">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-423">RDBMS</span></span>

* <span data-ttu-id="14cc9-424">Ajout de commandes de gestion de clés de chiffrement de données de serveur pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-424">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="14cc9-425">10 mars 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-425">March 10, 2020</span></span>

<span data-ttu-id="14cc9-426">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-426">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-427">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-427">ACR</span></span>

* <span data-ttu-id="14cc9-428">Correctif : `az acr login` déclenche une erreur de manière erronée</span><span class="sxs-lookup"><span data-stu-id="14cc9-428">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="14cc9-429">Ajout d’une nouvelle commande `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="14cc9-429">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="14cc9-430">Ajout d’un lien privé et de la prise en charge CMK</span><span class="sxs-lookup"><span data-stu-id="14cc9-430">Add private link and CMK support</span></span>
* <span data-ttu-id="14cc9-431">Ajout de la commande « private-link-resource list »</span><span class="sxs-lookup"><span data-stu-id="14cc9-431">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-432">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-432">AKS</span></span>

* <span data-ttu-id="14cc9-433">Correction de la navigation aks dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-433">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="14cc9-434">az aks : correction de la supervision des erreurs NoneType addon et agentpool</span><span class="sxs-lookup"><span data-stu-id="14cc9-434">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="14cc9-435">Ajout de --nodepool-tags au pool de nœuds lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-435">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="14cc9-436">Ajout de --tags lors de l’ajout ou de la mise à jour d’un nodepool à un cluster</span><span class="sxs-lookup"><span data-stu-id="14cc9-436">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="14cc9-437">aks create : ajout de `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="14cc9-437">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="14cc9-438">Ajout de --nodepool-labels lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-438">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="14cc9-439">Ajout de --labels lors de l’ajout d’un nouveau nodepool à un cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-439">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="14cc9-440">Ajout d’un caractère / manquant à l’URL de tableau de bord</span><span class="sxs-lookup"><span data-stu-id="14cc9-440">add missing / in the dashboard url</span></span>
* <span data-ttu-id="14cc9-441">Prise en charge de la création de clusters AKS activant l’identité managée</span><span class="sxs-lookup"><span data-stu-id="14cc9-441">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="14cc9-442">az aks : validation du plug-in réseau pour qu’il soit « azure » ou « kubenet »</span><span class="sxs-lookup"><span data-stu-id="14cc9-442">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="14cc9-443">az aks : Ajout de la prise en charge des clés de session AAD</span><span class="sxs-lookup"><span data-stu-id="14cc9-443">az aks: Add aad session key support</span></span>
* <span data-ttu-id="14cc9-444">[CHANGEMENT CASSANT] az aks : prise en charge des modifications MSI pour GF et BF pour omsagent (supervision de conteneur) (#1)</span><span class="sxs-lookup"><span data-stu-id="14cc9-444">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="14cc9-445">az aks use-dev-spaces : ajout de l’option de type de point de terminaison à la commande use-dev-spaces pour personnaliser le point de terminaison créé sur un contrôleur Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="14cc9-445">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-446">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-446">AppConfig</span></span>

* <span data-ttu-id="14cc9-447">Déblocage de l’utilisation de « kv set » pour ajouter la fonctionnalité et la référence de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-447">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-448">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-448">AppService</span></span>

* <span data-ttu-id="14cc9-449">az webapp create : résolution d’un problème lors de l’exécution de la commande avec --runtime</span><span class="sxs-lookup"><span data-stu-id="14cc9-449">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="14cc9-450">az functionapp deployment source config-zip : ajout d’un message d’erreur si le nom du groupe de ressources ou de la fonction n’est pas valide ou n’existe pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-450">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="14cc9-451">functionapp create : correction du message d’avertissement qui s’affiche aujourd’hui avec `functionapp create`, qui mentionne un indicateur `--functions_version` mais utilise de manière erronée un `_` au lieu d’un `-` dans le nom de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="14cc9-451">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="14cc9-452">az functionapp create : mise à jour de la façon dont linuxFxVersion et le nom de l’image conteneur étaient définis pour les applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-452">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="14cc9-453">az functionapp deployment source config-zip : résolution d’un problème dû à une condition de concurrence en cas de modification des paramètres d’application pendant le déploiement de fichier zip, provoquant des erreurs 5xx lors du déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-453">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="14cc9-454">Correctif 5720946 : az webapp backup ne parvient pas à définir le nom</span><span class="sxs-lookup"><span data-stu-id="14cc9-454">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-455">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-455">ARM</span></span>

* <span data-ttu-id="14cc9-456">az resource : amélioration des exemples du module de ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-456">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="14cc9-457">az policy assignment list : prise en charge de l’énumération des affectations de stratégie au niveau de l’étendue du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="14cc9-457">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="14cc9-458">Ajout de `az deployment group` et `az deployment operation group` pour le déploiement de modèle au niveau des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="14cc9-458">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="14cc9-459">Il s’agit d’un doublon de `az group deployment` et `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="14cc9-459">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="14cc9-460">Ajout de `az deployment sub` et `az deployment operation sub` pour le déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="14cc9-460">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="14cc9-461">Il s’agit d’un doublon de `az deployment` et `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="14cc9-461">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="14cc9-462">Ajout de `az deployment mg` et `az deployment operation mg` pour le déploiement de modèle au niveau des groupes de gestion</span><span class="sxs-lookup"><span data-stu-id="14cc9-462">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="14cc9-463">Ajout de `az deployment tenant` et `az deployment operation tenant` pour le déploiement de modèle à l’étendue du locataire</span><span class="sxs-lookup"><span data-stu-id="14cc9-463">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="14cc9-464">az policy assignment create : ajout d’une description au paramètre `--location`</span><span class="sxs-lookup"><span data-stu-id="14cc9-464">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="14cc9-465">az group deployment create : ajout du paramètre `--aux-tenants` pour prendre en charge les locataires croisés</span><span class="sxs-lookup"><span data-stu-id="14cc9-465">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-466">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-466">CDN</span></span>

* <span data-ttu-id="14cc9-467">Ajouter de commandes WAF CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-467">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-468">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-468">Compute</span></span>

* <span data-ttu-id="14cc9-469">az sig image-version : ajout de --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="14cc9-469">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="14cc9-470">az ppg show: ajout de --colocation-status pour permettre l’extraction de l’état de colocalisation de toutes les ressources dans le groupe de placement de proximité</span><span class="sxs-lookup"><span data-stu-id="14cc9-470">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="14cc9-471">az vmss create/update : prise en charge des réparations automatiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-471">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="14cc9-472">[CHANGEMENT CASSANT] az image template : template a été renommé builder</span><span class="sxs-lookup"><span data-stu-id="14cc9-472">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="14cc9-473">az image builder create : ajout de --image-template</span><span class="sxs-lookup"><span data-stu-id="14cc9-473">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-474">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-474">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-475">Ajout d’applets de commande de déclencheur, de procédure stockée SQL et de fonctions définies par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-475">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="14cc9-476">az cosmosdb create : ajout de --key-uri pour prendre en charge l’ajout d’informations de chiffrement de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-476">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-477">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-477">KeyVault</span></span>

* <span data-ttu-id="14cc9-478">keyvault create : activation de la suppression réversible par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-478">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-479">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-479">Monitor</span></span>

* <span data-ttu-id="14cc9-480">az monitor metrics alert create : prise en charge de `~` dans `--condition`</span><span class="sxs-lookup"><span data-stu-id="14cc9-480">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-481">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-481">Network</span></span>

* <span data-ttu-id="14cc9-482">az network application-gateway rewrite-rule create : prise en charge de la configuration d’URL</span><span class="sxs-lookup"><span data-stu-id="14cc9-482">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="14cc9-483">az network dns zone import : --zone-name respectera la casse à l’avenir</span><span class="sxs-lookup"><span data-stu-id="14cc9-483">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="14cc9-484">az network private-endpoint/private-link-service : suppression de l’étiquette d’aperçu</span><span class="sxs-lookup"><span data-stu-id="14cc9-484">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="14cc9-485">az network bastion : prise en charge de bastion</span><span class="sxs-lookup"><span data-stu-id="14cc9-485">az network bastion: support bastion</span></span>
* <span data-ttu-id="14cc9-486">az network vnet list-available-ips : prise en charge de l’énumération des adresses IP disponibles sur un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-486">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="14cc9-487">az network watcher flow-log create/list/delete/update : ajout de nouvelles commandes pour gérer le journal de flux d’observateur et l’exposition de --location pour identifier explicitement l’observateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-487">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="14cc9-488">az network watcher flow-log configure : dépréciée</span><span class="sxs-lookup"><span data-stu-id="14cc9-488">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="14cc9-489">az network watcher flow-log show : prise en charge de --location et de --name pour obtenir un résultat au format ARM. L’ancienne sortie mise en forme est dépréciée</span><span class="sxs-lookup"><span data-stu-id="14cc9-489">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="14cc9-490">Policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-490">Policy</span></span>

* <span data-ttu-id="14cc9-491">az policy assignment create : correction du bogue qui générait automatiquement un nom d’attribution de stratégie dépassant la limite</span><span class="sxs-lookup"><span data-stu-id="14cc9-491">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-492">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-492">RBAC</span></span>

* <span data-ttu-id="14cc9-493">az ad group show : correction du bogue qui faisait que --group était traité comme un problème Regex</span><span class="sxs-lookup"><span data-stu-id="14cc9-493">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-494">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-494">RDBMS</span></span>

* <span data-ttu-id="14cc9-495">Passage du SDK azure-mgmt-rdbms à la version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-495">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="14cc9-496">az postgres private-endpoint-connection : gestion des connexions de point de terminaison privé postgres</span><span class="sxs-lookup"><span data-stu-id="14cc9-496">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="14cc9-497">az postgres private-link-resource : gestion des ressources de lien privé postgres</span><span class="sxs-lookup"><span data-stu-id="14cc9-497">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="14cc9-498">az mysql private-endpoint-connection : gestion des connexions de point de terminaison privé mysql</span><span class="sxs-lookup"><span data-stu-id="14cc9-498">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="14cc9-499">az mysql private-link-resource : gestion des ressources de lien privé mysql</span><span class="sxs-lookup"><span data-stu-id="14cc9-499">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="14cc9-500">az mariadb private-endpoint-connection : gestion des connexions de point de terminaison privé mariadb</span><span class="sxs-lookup"><span data-stu-id="14cc9-500">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="14cc9-501">az mariadb private-link-resource : gestion des ressources de lien privé mariadb</span><span class="sxs-lookup"><span data-stu-id="14cc9-501">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="14cc9-502">Mise à jour des tests de point de terminaison privé SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-502">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-503">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-503">SQL</span></span>

* <span data-ttu-id="14cc9-504">Sql midb ; ajout de list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="14cc9-504">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="14cc9-505">(sql server create :) Ajout de l’indicateur facultatif « Enable »/« Disable » d’accès au réseau public à sql server create</span><span class="sxs-lookup"><span data-stu-id="14cc9-505">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="14cc9-506">(sql server update :) modifications du client</span><span class="sxs-lookup"><span data-stu-id="14cc9-506">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="14cc9-507">Ajout de propriété minimal_tls_version pour MI et SQL DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-507">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-508">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-508">Storage</span></span>

* <span data-ttu-id="14cc9-509">az storage blob delete-batch : comportement incorrect de l’indicateur `--dryrun`</span><span class="sxs-lookup"><span data-stu-id="14cc9-509">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="14cc9-510">az storage account network-rule add (correctif de bogue) : l’opération d’ajout doit être idempotent</span><span class="sxs-lookup"><span data-stu-id="14cc9-510">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="14cc9-511">az storage account create/update : Ajout de la prise en charge des préférences de routage</span><span class="sxs-lookup"><span data-stu-id="14cc9-511">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="14cc9-512">Mise à niveau de la version azure-mgmt-storage vers 8.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-512">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="14cc9-513">az storage container immutability create : ajout du paramètre --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="14cc9-513">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="14cc9-514">az storage account private-link-resource list : ajout de la prise en charge de l’énumération des ressources de lien privé pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-514">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="14cc9-515">az storage account private-endpoint-connection approve/reject/show/delete : prise en charge de la gestion des connexions de point de terminaison privé</span><span class="sxs-lookup"><span data-stu-id="14cc9-515">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="14cc9-516">az storage account blob-service-properties update : ajout de --enable-restore-policy et --restore-days</span><span class="sxs-lookup"><span data-stu-id="14cc9-516">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="14cc9-517">az storage blob restore : ajout de la prise en charge de la restauration des plages d’objets blob</span><span class="sxs-lookup"><span data-stu-id="14cc9-517">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="14cc9-518">18 février 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-518">February 18, 2020</span></span>

<span data-ttu-id="14cc9-519">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-519">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-520">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-520">ACR</span></span>

* <span data-ttu-id="14cc9-521">Ajoute un nouvel argument `--expose-token` pour `az acr login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-521">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="14cc9-522">Corrige la sortie incorrecte de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="14cc9-522">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="14cc9-523">az acr login : lève une CLIError si des erreurs sont retournées par la commande docker</span><span class="sxs-lookup"><span data-stu-id="14cc9-523">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-524">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-524">ACS</span></span>

* <span data-ttu-id="14cc9-525">aks create/update : ajoute la validation `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="14cc9-525">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="14cc9-526">Aladdin</span><span class="sxs-lookup"><span data-stu-id="14cc9-526">Aladdin</span></span>

* <span data-ttu-id="14cc9-527">Analyse les exemples générés dans le _help.py des commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-527">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-528">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-528">AMS</span></span>

* <span data-ttu-id="14cc9-529">az ams est désormais en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="14cc9-529">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-530">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-530">AppConfig</span></span>

* <span data-ttu-id="14cc9-531">Modifie le message d’aide pour exclure les filtres de clé ou d’étiquette non pris en charge</span><span class="sxs-lookup"><span data-stu-id="14cc9-531">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="14cc9-532">Supprimer l’étiquette d’aperçu pour la plupart des commandes, à l’exception des indicateurs d’identité managée et de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="14cc9-532">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="14cc9-533">Ajoute une clé gérée par le client lors de la mise à jour des magasins</span><span class="sxs-lookup"><span data-stu-id="14cc9-533">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-534">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-534">AppService</span></span>

* <span data-ttu-id="14cc9-535">az webapp list-runtimes : correction du bogue concernant list-runtimes</span><span class="sxs-lookup"><span data-stu-id="14cc9-535">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="14cc9-536">Ajoute az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="14cc9-536">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="14cc9-537">Ajoute la prise en charge des applications de fonction v3 et du nœud 12</span><span class="sxs-lookup"><span data-stu-id="14cc9-537">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-538">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-538">ARM</span></span>

* <span data-ttu-id="14cc9-539">az policy assignment create : correction du message d’erreur lorsque le paramètre `--policy` n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="14cc9-539">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="14cc9-540">az group deployment create : correction de l’erreur « stat: path too long for Windows » (Chemin trop long pour Windows) lors de l’utilisation d’un fichier parameters.json volumineux</span><span class="sxs-lookup"><span data-stu-id="14cc9-540">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-541">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-541">Backup</span></span>

* <span data-ttu-id="14cc9-542">Correction du flux de récupération au niveau de l’élément dans OLR</span><span class="sxs-lookup"><span data-stu-id="14cc9-542">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="14cc9-543">Ajout de la prise en charge de la restauration sous forme de fichiers pour les bases de données SQL et SAP</span><span class="sxs-lookup"><span data-stu-id="14cc9-543">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-544">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-544">Compute</span></span>

* <span data-ttu-id="14cc9-545">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="14cc9-545">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="14cc9-546">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="14cc9-546">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="14cc9-547">az vm host : supprime l’étiquette d’aperçu pour `vm host` et `vm host group`</span><span class="sxs-lookup"><span data-stu-id="14cc9-547">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="14cc9-548">[CHANGEMENT CASSANT] Correctif n° 10728 : `az vm create` Création automatique d’un sous-réseau si un réseau virtuel est spécifié et s’il n’existe pas de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-548">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="14cc9-549">Amélioration de la robustesse de la liste d’images de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="14cc9-549">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="14cc9-550">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="14cc9-550">Eventhub</span></span>

* <span data-ttu-id="14cc9-551">Prise en charge d’Azure Stack pour le profil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-551">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-552">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-552">KeyVault</span></span>

* <span data-ttu-id="14cc9-553">az keyvault key create : ajouter une nouvelle valeur `import` pour le paramètre `--ops`</span><span class="sxs-lookup"><span data-stu-id="14cc9-553">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="14cc9-554">az keyvault key list-versions : prise en charge du paramètre `--id` pour la spécification des clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-554">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="14cc9-555">Prise en charge des connexions de points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="14cc9-555">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-556">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-556">Network</span></span>

* <span data-ttu-id="14cc9-557">Passage à azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-557">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="14cc9-558">az network private-link-service update/create: support --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="14cc9-558">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="14cc9-559">Ajout de la fonctionnalité Moniteur de connexion v2</span><span class="sxs-lookup"><span data-stu-id="14cc9-559">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-560">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-560">Packaging</span></span>

* <span data-ttu-id="14cc9-561">[CHANGEMENT CASSANT] Python 2.7 n’est plus pris en charge</span><span class="sxs-lookup"><span data-stu-id="14cc9-561">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-562">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-562">Profile</span></span>

* <span data-ttu-id="14cc9-563">Aperçu : Ajoutez les nouveaux attributs `homeTenantId` et `managedByTenants` aux comptes d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="14cc9-563">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="14cc9-564">Réexécutez `az login` pour que les modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="14cc9-564">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="14cc9-565">az login : affiche un avertissement lorsqu’un abonnement est listé par plusieurs locataires et s’affiche par défaut pour le premier.</span><span class="sxs-lookup"><span data-stu-id="14cc9-565">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="14cc9-566">Pour sélectionner un locataire lors de l’accès à cet abonnement, ajoutez `--tenant` dans `az login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-566">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-567">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-567">Role</span></span>

* <span data-ttu-id="14cc9-568">az role assignment create : correction de l’erreur lors de laquelle l’attribution d’un rôle à un principal de service par nom d’affichage générait une erreur HTTP 400</span><span class="sxs-lookup"><span data-stu-id="14cc9-568">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-569">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-569">SQL</span></span>

* <span data-ttu-id="14cc9-570">Mise à jour de l’applet de commande SQL Managed Instance `az sql mi update` avec deux nouveaux paramètres : tier et family</span><span class="sxs-lookup"><span data-stu-id="14cc9-570">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-571">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-571">Storage</span></span>

* <span data-ttu-id="14cc9-572">[CHANGEMENT CASSANT] `az storage account create` : Remplacement du type de compte de stockage par défaut par StorageV2</span><span class="sxs-lookup"><span data-stu-id="14cc9-572">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="14cc9-573">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-573">February 04, 2020</span></span>

<span data-ttu-id="14cc9-574">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="14cc9-574">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-575">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-575">ACS</span></span>

* <span data-ttu-id="14cc9-576">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="14cc9-576">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="14cc9-577">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-577">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-578">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-578">ACR</span></span>

* <span data-ttu-id="14cc9-579">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="14cc9-579">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="14cc9-580">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="14cc9-580">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="14cc9-581">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="14cc9-581">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-582">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-582">AKS</span></span>

* <span data-ttu-id="14cc9-583">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="14cc9-583">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-584">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-584">AppConfig</span></span>

* <span data-ttu-id="14cc9-585">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-585">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="14cc9-586">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-586">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="14cc9-587">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="14cc9-587">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="14cc9-588">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="14cc9-588">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="14cc9-589">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-589">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-590">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-590">AppService</span></span>

* <span data-ttu-id="14cc9-591">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-591">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="14cc9-592">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-592">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-593">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-593">ARM</span></span>

* <span data-ttu-id="14cc9-594">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-594">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="14cc9-595">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="14cc9-595">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="14cc9-596">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="14cc9-596">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="14cc9-597">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-597">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="14cc9-598">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-598">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="14cc9-599">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="14cc9-599">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="14cc9-600">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="14cc9-600">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-601">BotService</span><span class="sxs-lookup"><span data-stu-id="14cc9-601">BotService</span></span>

* <span data-ttu-id="14cc9-602">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="14cc9-602">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="14cc9-603">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="14cc9-603">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-604">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-604">CDN</span></span>

* <span data-ttu-id="14cc9-605">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="14cc9-605">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="14cc9-606">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="14cc9-606">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="14cc9-607">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="14cc9-607">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="14cc9-608">Deployment Manager</span><span class="sxs-lookup"><span data-stu-id="14cc9-608">Deployment Manager</span></span>

* <span data-ttu-id="14cc9-609">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="14cc9-609">Add list operation for all resources.</span></span>
* <span data-ttu-id="14cc9-610">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="14cc9-610">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="14cc9-611">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="14cc9-611">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-612">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-612">IoT</span></span>

* <span data-ttu-id="14cc9-613">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="14cc9-613">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="14cc9-614">IoT Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-614">IoT Central</span></span>

* <span data-ttu-id="14cc9-615">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="14cc9-615">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-616">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-616">Key Vault</span></span>

* <span data-ttu-id="14cc9-617">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="14cc9-617">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="14cc9-618">Divers</span><span class="sxs-lookup"><span data-stu-id="14cc9-618">Misc</span></span>

* <span data-ttu-id="14cc9-619">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="14cc9-619">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-620">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-620">Network</span></span>

* <span data-ttu-id="14cc9-621">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="14cc9-621">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="14cc9-622">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="14cc9-622">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="14cc9-623">Policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-623">Policy</span></span>

* <span data-ttu-id="14cc9-624">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="14cc9-624">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="14cc9-625">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="14cc9-625">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-626">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-626">Profile</span></span>

* <span data-ttu-id="14cc9-627">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-627">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-628">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-628">RBAC</span></span>

* <span data-ttu-id="14cc9-629">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-629">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="14cc9-630">Sécurité</span><span class="sxs-lookup"><span data-stu-id="14cc9-630">Security</span></span>

* <span data-ttu-id="14cc9-631">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="14cc9-631">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-632">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-632">SQL</span></span>

* <span data-ttu-id="14cc9-633">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-633">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="14cc9-634">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="14cc9-634">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="14cc9-635">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="14cc9-635">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="14cc9-636">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="14cc9-636">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="14cc9-637">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="14cc9-637">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="14cc9-638">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="14cc9-638">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-639">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-639">Storage</span></span>

* <span data-ttu-id="14cc9-640">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="14cc9-640">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="14cc9-641">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-641">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="14cc9-642">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="14cc9-642">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="14cc9-643">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="14cc9-643">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="14cc9-644">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="14cc9-644">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="14cc9-645">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="14cc9-645">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="14cc9-646">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-646">ServiceFabric</span></span>

* <span data-ttu-id="14cc9-647">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="14cc9-647">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="14cc9-648">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-648">January 13, 2020</span></span>

<span data-ttu-id="14cc9-649">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="14cc9-649">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-650">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-650">Compute</span></span>

* <span data-ttu-id="14cc9-651">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="14cc9-651">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="14cc9-652">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="14cc9-652">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-653">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-653">Storage</span></span>

* <span data-ttu-id="14cc9-654">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-654">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="14cc9-655">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="14cc9-655">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="14cc9-656">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="14cc9-656">January 07, 2020</span></span>

<span data-ttu-id="14cc9-657">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="14cc9-657">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-658">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-658">ACR</span></span>

* <span data-ttu-id="14cc9-659">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-659">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="14cc9-660">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="14cc9-660">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-661">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-661">AppConfig</span></span>

* <span data-ttu-id="14cc9-662">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="14cc9-662">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="14cc9-663">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-663">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="14cc9-664">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="14cc9-664">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-665">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-665">AppService</span></span>

* <span data-ttu-id="14cc9-666">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="14cc9-666">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="14cc9-667">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-667">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="14cc9-668">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="14cc9-668">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-669">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-669">ARM</span></span>

* <span data-ttu-id="14cc9-670">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-670">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-671">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-671">Backup</span></span>

* <span data-ttu-id="14cc9-672">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="14cc9-672">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="14cc9-673">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="14cc9-673">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="14cc9-674">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="14cc9-674">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-675">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-675">Compute</span></span>

* <span data-ttu-id="14cc9-676">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="14cc9-676">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="14cc9-677">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="14cc9-677">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="14cc9-678">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="14cc9-678">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-679">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-679">HDInsight</span></span>

* <span data-ttu-id="14cc9-680">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="14cc9-680">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="14cc9-681">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-681">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="14cc9-682">Divers</span><span class="sxs-lookup"><span data-stu-id="14cc9-682">Misc.</span></span>

* <span data-ttu-id="14cc9-683">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="14cc9-683">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="14cc9-684">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="14cc9-684">Event Hubs</span></span>

* <span data-ttu-id="14cc9-685">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-685">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="14cc9-686">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="14cc9-686">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="14cc9-687">Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-687">Service Bus</span></span>

* <span data-ttu-id="14cc9-688">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-688">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="14cc9-689">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="14cc9-689">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-690">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-690">RBAC</span></span>

* <span data-ttu-id="14cc9-691">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-691">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-692">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-692">Storage</span></span>

* <span data-ttu-id="14cc9-693">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="14cc9-693">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="14cc9-694">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-694">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="14cc9-695">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="14cc9-695">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="14cc9-696">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-696">December 17, 2019</span></span>

<span data-ttu-id="14cc9-697">2.0.78</span><span class="sxs-lookup"><span data-stu-id="14cc9-697">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-698">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-698">ACR</span></span>

* <span data-ttu-id="14cc9-699">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="14cc9-699">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-700">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-700">ACS</span></span>

* <span data-ttu-id="14cc9-701">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-701">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-702">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-702">AMS</span></span>

* <span data-ttu-id="14cc9-703">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="14cc9-703">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-704">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-704">AppConfig</span></span>

* <span data-ttu-id="14cc9-705">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="14cc9-705">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="14cc9-706">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="14cc9-706">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="14cc9-707">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="14cc9-707">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-708">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-708">AppService</span></span>

* <span data-ttu-id="14cc9-709">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="14cc9-709">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="14cc9-710">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="14cc9-710">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="14cc9-711">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="14cc9-711">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="14cc9-712">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-712">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-713">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-713">ARM</span></span>

* <span data-ttu-id="14cc9-714">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-714">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="14cc9-715">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="14cc9-715">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="14cc9-716">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="14cc9-716">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-717">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-717">Backup</span></span>

* <span data-ttu-id="14cc9-718">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="14cc9-718">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-719">BotService</span><span class="sxs-lookup"><span data-stu-id="14cc9-719">BotService</span></span>

* <span data-ttu-id="14cc9-720">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-720">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="14cc9-721">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="14cc9-721">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="14cc9-722">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-722">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="14cc9-723">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-723">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="14cc9-724">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-724">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="14cc9-725">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-725">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="14cc9-726">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-726">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="14cc9-727">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-727">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="14cc9-728">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="14cc9-728">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-729">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-729">Compute</span></span>

* <span data-ttu-id="14cc9-730">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="14cc9-730">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="14cc9-731">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="14cc9-731">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="14cc9-732">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="14cc9-732">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="14cc9-733">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="14cc9-733">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="14cc9-734">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="14cc9-734">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="14cc9-735">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="14cc9-735">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-736">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-736">Core</span></span>

* <span data-ttu-id="14cc9-737">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="14cc9-737">Removed support for Python 3.4</span></span>
* <span data-ttu-id="14cc9-738">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-738">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="14cc9-739">DLS</span><span class="sxs-lookup"><span data-stu-id="14cc9-739">DLS</span></span>

* <span data-ttu-id="14cc9-740">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="14cc9-740">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="14cc9-741">Installer</span><span class="sxs-lookup"><span data-stu-id="14cc9-741">Install</span></span>

* <span data-ttu-id="14cc9-742">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="14cc9-742">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-743">IOT</span><span class="sxs-lookup"><span data-stu-id="14cc9-743">IOT</span></span>

* <span data-ttu-id="14cc9-744">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="14cc9-744">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="14cc9-745">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-745">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-746">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-746">Key Vault</span></span>

* <span data-ttu-id="14cc9-747">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-747">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="14cc9-748">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="14cc9-748">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="14cc9-749">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="14cc9-749">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="14cc9-750">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="14cc9-750">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="14cc9-751">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="14cc9-751">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-752">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-752">Network</span></span>

* <span data-ttu-id="14cc9-753">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-753">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="14cc9-754">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-754">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="14cc9-755">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="14cc9-755">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="14cc9-756">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-756">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="14cc9-757">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="14cc9-757">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-758">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-758">Packaging</span></span>

* <span data-ttu-id="14cc9-759">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="14cc9-759">Added back edge builds for pip install</span></span>
* <span data-ttu-id="14cc9-760">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="14cc9-760">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="14cc9-761">Policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-761">Policy</span></span>

* <span data-ttu-id="14cc9-762">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="14cc9-762">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="14cc9-763">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="14cc9-763">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-764">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-764">Redis</span></span>

* <span data-ttu-id="14cc9-765">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-765">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="14cc9-766">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="14cc9-766">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="14cc9-767">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-767">ServiceFabric</span></span>

* <span data-ttu-id="14cc9-768">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="14cc9-768">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="14cc9-769">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="14cc9-769">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-770">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-770">SQL</span></span>

* <span data-ttu-id="14cc9-771">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="14cc9-771">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-772">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-772">Storage</span></span>

* <span data-ttu-id="14cc9-773">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="14cc9-773">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="14cc9-774">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="14cc9-774">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="14cc9-775">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="14cc9-775">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="14cc9-776">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-776">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="14cc9-777">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="14cc9-777">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="14cc9-778">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-778">November 26, 2019</span></span>

<span data-ttu-id="14cc9-779">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="14cc9-779">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-780">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-780">ACR</span></span>

* <span data-ttu-id="14cc9-781">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="14cc9-781">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="14cc9-782">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="14cc9-782">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="14cc9-783">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="14cc9-783">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="14cc9-784">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="14cc9-784">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-785">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-785">AKS</span></span>

* <span data-ttu-id="14cc9-786">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-786">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-787">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-787">AppConfig</span></span>

* <span data-ttu-id="14cc9-788">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-788">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="14cc9-789">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="14cc9-789">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="14cc9-790">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="14cc9-790">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="14cc9-791">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-791">AppService</span></span>

* <span data-ttu-id="14cc9-792">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-792">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="14cc9-793">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-793">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="14cc9-794">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="14cc9-794">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-795">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-795">Backup</span></span>

* <span data-ttu-id="14cc9-796">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="14cc9-796">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="14cc9-797">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="14cc9-797">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-798">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-798">Compute</span></span>

* <span data-ttu-id="14cc9-799">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-799">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="14cc9-800">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="14cc9-800">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="14cc9-801">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="14cc9-801">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="14cc9-802">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="14cc9-802">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="14cc9-803">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="14cc9-803">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="14cc9-804">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="14cc9-804">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="14cc9-805">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-805">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="14cc9-806">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="14cc9-806">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="14cc9-807">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="14cc9-807">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="14cc9-808">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="14cc9-808">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-809">IOT</span><span class="sxs-lookup"><span data-stu-id="14cc9-809">IOT</span></span>

* <span data-ttu-id="14cc9-810">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="14cc9-810">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="14cc9-811">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="14cc9-811">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="14cc9-812">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="14cc9-812">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-813">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-813">Key Vault</span></span>

* <span data-ttu-id="14cc9-814">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="14cc9-814">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="14cc9-815">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="14cc9-815">NetAppFiles</span></span>

* <span data-ttu-id="14cc9-816">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="14cc9-816">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-817">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-817">Network</span></span>

* <span data-ttu-id="14cc9-818">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="14cc9-818">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="14cc9-819">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="14cc9-819">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="14cc9-820">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="14cc9-820">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="14cc9-821">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="14cc9-821">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="14cc9-822">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="14cc9-822">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="14cc9-823">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="14cc9-823">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="14cc9-824">Packaging</span><span class="sxs-lookup"><span data-stu-id="14cc9-824">Packaging</span></span>

* <span data-ttu-id="14cc9-825">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="14cc9-825">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="14cc9-826">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="14cc9-826">Added support for Python 3.8</span></span>
* <span data-ttu-id="14cc9-827">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="14cc9-827">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-828">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-828">Profile</span></span>

* <span data-ttu-id="14cc9-829">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="14cc9-829">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="14cc9-830">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="14cc9-830">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="14cc9-831">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="14cc9-831">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="14cc9-832">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="14cc9-832">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="14cc9-833">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="14cc9-833">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-834">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-834">RBAC</span></span>

* <span data-ttu-id="14cc9-835">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="14cc9-835">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-836">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-836">Redis</span></span>

* <span data-ttu-id="14cc9-837">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="14cc9-837">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="14cc9-838">Réservations</span><span class="sxs-lookup"><span data-stu-id="14cc9-838">Reservations</span></span>

* <span data-ttu-id="14cc9-839">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-839">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="14cc9-840">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="14cc9-840">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="14cc9-841">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-841">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="14cc9-842">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-842">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="14cc9-843">Rest</span><span class="sxs-lookup"><span data-stu-id="14cc9-843">Rest</span></span>
* <span data-ttu-id="14cc9-844">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="14cc9-844">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-845">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-845">SQL</span></span>

* <span data-ttu-id="14cc9-846">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="14cc9-846">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-847">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-847">Storage</span></span>

* <span data-ttu-id="14cc9-848">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="14cc9-848">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="14cc9-849">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-849">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="14cc9-850">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="14cc9-850">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="14cc9-851">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="14cc9-851">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="14cc9-852">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-852">November 4, 2019</span></span>

<span data-ttu-id="14cc9-853">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="14cc9-853">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-854">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-854">ACR</span></span>

* <span data-ttu-id="14cc9-855">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-855">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="14cc9-856">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="14cc9-856">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="14cc9-857">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="14cc9-857">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-858">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-858">AKS</span></span>

* <span data-ttu-id="14cc9-859">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="14cc9-859">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="14cc9-860">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="14cc9-860">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="14cc9-861">AppConfig</span><span class="sxs-lookup"><span data-stu-id="14cc9-861">AppConfig</span></span>

* <span data-ttu-id="14cc9-862">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="14cc9-862">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="14cc9-863">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="14cc9-863">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="14cc9-864">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="14cc9-864">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-865">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-865">AppService</span></span>

* <span data-ttu-id="14cc9-866">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="14cc9-866">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="14cc9-867">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-867">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="14cc9-868">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="14cc9-868">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="14cc9-869">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-869">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="14cc9-870">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-870">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-871">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-871">ARM</span></span>

* <span data-ttu-id="14cc9-872">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="14cc9-872">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="14cc9-873">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-873">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-874">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-874">Backup</span></span>

* <span data-ttu-id="14cc9-875">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="14cc9-875">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-876">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-876">Compute</span></span>

* <span data-ttu-id="14cc9-877">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="14cc9-877">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="14cc9-878">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-878">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="14cc9-879">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="14cc9-879">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="14cc9-880">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="14cc9-880">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="14cc9-881">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="14cc9-881">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="14cc9-882">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-882">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="14cc9-883">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="14cc9-883">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="14cc9-884">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="14cc9-884">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-885">CosmosDB</span></span>

* <span data-ttu-id="14cc9-886">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-886">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="14cc9-887">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-887">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="14cc9-888">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-888">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="14cc9-889">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="14cc9-889">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="14cc9-890">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-890">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="14cc9-891">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="14cc9-891">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="14cc9-892">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-892">Fixed typo in help message</span></span>
* <span data-ttu-id="14cc9-893">base de données : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="14cc9-893">database: Added deprecation information</span></span>
* <span data-ttu-id="14cc9-894">collection : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="14cc9-894">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-895">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-895">IoT</span></span>

* <span data-ttu-id="14cc9-896">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="14cc9-896">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="14cc9-897">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-897">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-898">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-898">Key Vault</span></span>

* <span data-ttu-id="14cc9-899">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-899">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="14cc9-900">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-900">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="14cc9-901">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="14cc9-901">NetAppFiles</span></span>

* <span data-ttu-id="14cc9-902">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="14cc9-902">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="14cc9-903">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="14cc9-903">This new API version includes:</span></span>

    - <span data-ttu-id="14cc9-904">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="14cc9-904">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="14cc9-905">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="14cc9-905">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="14cc9-906">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="14cc9-906">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="14cc9-907">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="14cc9-907">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-908">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-908">Network</span></span>

* <span data-ttu-id="14cc9-909">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="14cc9-909">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="14cc9-910">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="14cc9-910">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="14cc9-911">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="14cc9-911">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="14cc9-912">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-912">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="14cc9-913">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-913">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="14cc9-914">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="14cc9-914">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-915">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-915">Profile</span></span>

* <span data-ttu-id="14cc9-916">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-916">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="14cc9-917">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-917">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-918">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-918">RBAC</span></span>

* <span data-ttu-id="14cc9-919">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-919">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="14cc9-920">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-920">ServiceFabric</span></span>

* <span data-ttu-id="14cc9-921">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="14cc9-921">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-922">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-922">SQL</span></span>

* <span data-ttu-id="14cc9-923">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="14cc9-923">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-924">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-924">Storage</span></span>

* <span data-ttu-id="14cc9-925">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="14cc9-925">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="14cc9-926">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="14cc9-926">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="14cc9-927">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-927">October 15, 2019</span></span>

<span data-ttu-id="14cc9-928">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="14cc9-928">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-929">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-929">AKS</span></span>

* <span data-ttu-id="14cc9-930">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-930">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="14cc9-931">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-931">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-932">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-932">AMS</span></span>

* <span data-ttu-id="14cc9-933">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-933">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="14cc9-934">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="14cc9-934">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-935">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-935">AppService</span></span>

* <span data-ttu-id="14cc9-936">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="14cc9-936">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="14cc9-937">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-937">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="14cc9-938">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-938">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-939">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-939">ARM</span></span>

* <span data-ttu-id="14cc9-940">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="14cc9-940">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-941">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-941">Compute</span></span>

* <span data-ttu-id="14cc9-942">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-942">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="14cc9-943">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="14cc9-943">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="14cc9-944">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-944">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="14cc9-945">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="14cc9-945">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="14cc9-946">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-946">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="14cc9-947">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-947">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-948">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-948">Core</span></span>

* <span data-ttu-id="14cc9-949">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="14cc9-949">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-950">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-950">IoT</span></span>

* <span data-ttu-id="14cc9-951">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="14cc9-951">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-952">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-952">Monitor</span></span>

* <span data-ttu-id="14cc9-953">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="14cc9-953">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-954">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-954">Network</span></span>

* <span data-ttu-id="14cc9-955">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-955">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="14cc9-956">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-956">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-957">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-957">SQL</span></span>

* <span data-ttu-id="14cc9-958">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="14cc9-958">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-959">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-959">Storage</span></span>

* <span data-ttu-id="14cc9-960">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="14cc9-960">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="14cc9-961">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-961">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="14cc9-962">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-962">September 24, 2019</span></span>

<span data-ttu-id="14cc9-963">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="14cc9-963">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-964">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-964">ACR</span></span>

* <span data-ttu-id="14cc9-965">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-965">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="14cc9-966">[CHANGEMENT CASSANT] Renommage du paramètre `--name -n` en `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-966">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-967">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-967">AKS</span></span>

* <span data-ttu-id="14cc9-968">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="14cc9-968">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="14cc9-969">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="14cc9-969">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="14cc9-970">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="14cc9-970">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-971">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-971">ARM</span></span>

* <span data-ttu-id="14cc9-972">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="14cc9-972">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-973">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-973">Compute</span></span>

* <span data-ttu-id="14cc9-974">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="14cc9-974">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="14cc9-975">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="14cc9-975">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="14cc9-976">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-976">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="14cc9-977">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="14cc9-977">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="14cc9-978">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-978">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-979">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-979">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-980">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="14cc9-980">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="14cc9-981">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="14cc9-981">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="14cc9-982">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="14cc9-982">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="14cc9-983">EventGrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-983">EventGrid</span></span>

* <span data-ttu-id="14cc9-984">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="14cc9-984">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-985">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-985">Key Vault</span></span>

* <span data-ttu-id="14cc9-986">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-986">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-987">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-987">Monitor</span></span>

* <span data-ttu-id="14cc9-988">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-988">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="14cc9-989">Policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-989">Policy</span></span>

* <span data-ttu-id="14cc9-990">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-990">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="14cc9-991">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-991">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-992">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-992">Storage</span></span>

* <span data-ttu-id="14cc9-993">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-993">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="14cc9-994">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-994">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-995">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-995">ACR</span></span>

* <span data-ttu-id="14cc9-996">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-996">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-997">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-997">AKS</span></span>

* <span data-ttu-id="14cc9-998">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-998">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="14cc9-999">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-999">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="14cc9-1000">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1000">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-1001">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-1001">ARM</span></span>

* <span data-ttu-id="14cc9-1002">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="14cc9-1002">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1003">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1003">Batch</span></span>

* <span data-ttu-id="14cc9-1004">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1004">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="14cc9-1005">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1005">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="14cc9-1006">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1006">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="14cc9-1007">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1007">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="14cc9-1008">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1008">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="14cc9-1009">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1009">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="14cc9-1010">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1010">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1011">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1011">HDInsight</span></span>

* <span data-ttu-id="14cc9-1012">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="14cc9-1012">GA release</span></span>
* <span data-ttu-id="14cc9-1013">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1013">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-1014">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-1014">Key Vault</span></span>

* <span data-ttu-id="14cc9-1015">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1015">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="14cc9-1016">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1016">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1017">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1017">Network</span></span>

* <span data-ttu-id="14cc9-1018">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="14cc9-1018">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="14cc9-1019">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1019">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="14cc9-1020">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1020">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="14cc9-1021">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1021">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="14cc9-1022">Policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-1022">Policy</span></span>

* <span data-ttu-id="14cc9-1023">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-1023">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="14cc9-1024">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1024">August 27, 2019</span></span>

<span data-ttu-id="14cc9-1025">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="14cc9-1025">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1026">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1026">ACR</span></span>

* <span data-ttu-id="14cc9-1027">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1027">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="14cc9-1028">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="14cc9-1028">API Management</span></span>

* <span data-ttu-id="14cc9-1029">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1029">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1030">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1030">AppService</span></span>

* <span data-ttu-id="14cc9-1031">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1031">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="14cc9-1032">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1032">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-1033">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-1033">Keyvault</span></span>

* <span data-ttu-id="14cc9-1034">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1034">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1035">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1035">Network</span></span>

* <span data-ttu-id="14cc9-1036">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1036">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="14cc9-1037">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="14cc9-1037">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="14cc9-1038">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1038">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="14cc9-1039">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1039">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-1040">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-1040">RBAC</span></span>

* <span data-ttu-id="14cc9-1041">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-1041">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="14cc9-1042">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-1042">ServiceFabric</span></span>

* <span data-ttu-id="14cc9-1043">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="14cc9-1043">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="14cc9-1044">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-1044">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="14cc9-1045">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="14cc9-1045">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="14cc9-1046">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="14cc9-1046">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="14cc9-1047">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1047">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="14cc9-1048">SignalR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1048">SignalR</span></span>

* <span data-ttu-id="14cc9-1049">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1049">Added new commands:</span></span>
  * <span data-ttu-id="14cc9-1050">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1050">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="14cc9-1051">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1051">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="14cc9-1052">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1052">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="14cc9-1053">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1053">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1054">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1054">Storage</span></span>

* <span data-ttu-id="14cc9-1055">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1055">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="14cc9-1056">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1056">August 13, 2019</span></span>

<span data-ttu-id="14cc9-1057">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="14cc9-1057">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1058">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1058">AppService</span></span>

* <span data-ttu-id="14cc9-1059">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="14cc9-1059">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1060">BotService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1060">BotService</span></span>

* <span data-ttu-id="14cc9-1061">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="14cc9-1061">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="14cc9-1062">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="14cc9-1062">CognitiveServices</span></span>

* <span data-ttu-id="14cc9-1063">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1063">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-1064">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1064">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-1065">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="14cc9-1065">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="14cc9-1066">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1066">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1067">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1067">HDInsight</span></span>

<span data-ttu-id="14cc9-1068">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1068">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="14cc9-1069">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1069">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="14cc9-1070">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1070">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="14cc9-1071">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1071">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="14cc9-1072">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="14cc9-1072">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="14cc9-1073">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1073">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="14cc9-1074">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1074">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="14cc9-1075">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1075">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="14cc9-1076">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1076">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="14cc9-1077">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1077">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="14cc9-1078">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1078">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="14cc9-1079">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1079">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="14cc9-1080">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1080">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="14cc9-1081">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1081">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="14cc9-1082">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1082">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="14cc9-1083">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1083">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="14cc9-1084">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1084">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="14cc9-1085">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="14cc9-1085">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="14cc9-1086">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1086">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="14cc9-1087">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="14cc9-1087">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="14cc9-1088">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1088">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="14cc9-1089">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-1089">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="14cc9-1090">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="14cc9-1090">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="14cc9-1091">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-1091">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-1092">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-1092">Interactive</span></span>

* <span data-ttu-id="14cc9-1093">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1093">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="14cc9-1094">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1094">Kubernetes</span></span>

* <span data-ttu-id="14cc9-1095">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1095">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1096">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1096">Network</span></span>

* <span data-ttu-id="14cc9-1097">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1097">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-1098">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-1098">Profile</span></span>

* <span data-ttu-id="14cc9-1099">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-1099">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="14cc9-1100">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-1100">ServiceFabric</span></span>

* <span data-ttu-id="14cc9-1101">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="14cc9-1101">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="14cc9-1102">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="14cc9-1102">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1103">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1103">Storage</span></span>

* <span data-ttu-id="14cc9-1104">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1104">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="14cc9-1105">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1105">July 30, 2019</span></span>

<span data-ttu-id="14cc9-1106">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="14cc9-1106">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1107">ACR</span></span>

* <span data-ttu-id="14cc9-1108">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1108">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="14cc9-1109">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1109">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1110">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1110">Appservice</span></span>

* <span data-ttu-id="14cc9-1111">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="14cc9-1111">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="14cc9-1112">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1112">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="14cc9-1113">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="14cc9-1113">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1114">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1114">Network</span></span>

* <span data-ttu-id="14cc9-1115">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1115">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="14cc9-1116">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1116">Fixes #9604.</span></span> <span data-ttu-id="14cc9-1117">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1117">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="14cc9-1118">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1118">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-1119">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-1119">RBAC</span></span>

* <span data-ttu-id="14cc9-1120">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1120">Added `user update` command</span></span>
* <span data-ttu-id="14cc9-1121">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1121">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="14cc9-1122">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1122">Use replacement argument `--id`</span></span>
* <span data-ttu-id="14cc9-1123">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1123">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1124">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1124">SQL</span></span>

* <span data-ttu-id="14cc9-1125">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="14cc9-1125">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1126">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1126">Storage</span></span>

* <span data-ttu-id="14cc9-1127">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1127">Added `storage remove` command</span></span>
* <span data-ttu-id="14cc9-1128">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1128">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1129">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1129">VM</span></span>

* <span data-ttu-id="14cc9-1130">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="14cc9-1130">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="14cc9-1131">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1131">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="14cc9-1132">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1132">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="14cc9-1133">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="14cc9-1133">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="14cc9-1134">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1134">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="14cc9-1135">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1135">July 16, 2019</span></span>

<span data-ttu-id="14cc9-1136">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="14cc9-1136">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1137">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1137">Appservice</span></span>

* <span data-ttu-id="14cc9-1138">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="14cc9-1138">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="14cc9-1139">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-1139">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="14cc9-1140">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1140">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1141">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1141">Core</span></span>

* <span data-ttu-id="14cc9-1142">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1142">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1143">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1143">Batch</span></span>

* <span data-ttu-id="14cc9-1144">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1144">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="14cc9-1145">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1145">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="14cc9-1146">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1146">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="14cc9-1147">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1147">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="14cc9-1148">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="14cc9-1148">Eventhubs</span></span>

* <span data-ttu-id="14cc9-1149">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1149">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1150">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1150">RDBMS</span></span>

* <span data-ttu-id="14cc9-1151">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="14cc9-1151">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="14cc9-1152">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1152">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="14cc9-1153">Relais</span><span class="sxs-lookup"><span data-stu-id="14cc9-1153">Relay</span></span>

* <span data-ttu-id="14cc9-1154">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1154">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="14cc9-1155">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1155">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="14cc9-1156">Servicebus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1156">Servicebus</span></span>

* <span data-ttu-id="14cc9-1157">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1157">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1158">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1158">Storage</span></span>

* <span data-ttu-id="14cc9-1159">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1159">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="14cc9-1160">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1160">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="14cc9-1161">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1161">July 2, 2019</span></span>

<span data-ttu-id="14cc9-1162">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="14cc9-1162">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1163">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1163">Core</span></span>

* <span data-ttu-id="14cc9-1164">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1164">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="14cc9-1165">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1165">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="14cc9-1166">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1166">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1167">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1167">ACR</span></span>

* <span data-ttu-id="14cc9-1168">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="14cc9-1168">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1169">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1169">Appservice</span></span>

* <span data-ttu-id="14cc9-1170">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1170">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="14cc9-1171">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1171">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="14cc9-1172">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="14cc9-1172">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="14cc9-1173">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1173">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-1174">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1174">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-1175">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1175">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="14cc9-1176">DLS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1176">DLS</span></span>

* <span data-ttu-id="14cc9-1177">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1177">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="14cc9-1178">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14cc9-1178">Feedback</span></span>

* <span data-ttu-id="14cc9-1179">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="14cc9-1179">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1180">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1180">HDInsight</span></span>

* <span data-ttu-id="14cc9-1181">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1181">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="14cc9-1182">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-1182">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="14cc9-1183">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1183">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="14cc9-1184">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="14cc9-1184">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="14cc9-1185">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="14cc9-1185">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="14cc9-1186">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1186">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="14cc9-1187">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1187">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="14cc9-1188">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1188">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="14cc9-1189">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1189">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="14cc9-1190">Services gérés</span><span class="sxs-lookup"><span data-stu-id="14cc9-1190">Managed Services</span></span>

* <span data-ttu-id="14cc9-1191">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-1191">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-1192">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-1192">Profile</span></span>
* <span data-ttu-id="14cc9-1193">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="14cc9-1193">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-1194">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-1194">RBAC</span></span>

* <span data-ttu-id="14cc9-1195">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1195">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="14cc9-1196">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="14cc9-1196">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="14cc9-1197">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1197">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="14cc9-1198">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1198">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1199">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1199">RDBMS</span></span>

* <span data-ttu-id="14cc9-1200">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1200">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1201">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1201">SQL</span></span>

* <span data-ttu-id="14cc9-1202">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1202">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1203">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1203">Storage</span></span>

* <span data-ttu-id="14cc9-1204">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1204">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="14cc9-1205">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1205">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="14cc9-1206">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1206">VM</span></span>

* <span data-ttu-id="14cc9-1207">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1207">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="14cc9-1208">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1208">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="14cc9-1209">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-1209">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="14cc9-1210">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1210">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="14cc9-1211">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1211">June 18, 2019</span></span>

<span data-ttu-id="14cc9-1212">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="14cc9-1212">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1213">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1213">Core</span></span>

<span data-ttu-id="14cc9-1214">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1214">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="14cc9-1215">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1215">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="14cc9-1216">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1216">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="14cc9-1217">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1217">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="14cc9-1218">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1218">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="14cc9-1219">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1219">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="14cc9-1220">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1220">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1221">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1221">ACR</span></span>
* <span data-ttu-id="14cc9-1222">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="14cc9-1222">Added 'acr check-health' command</span></span>
* <span data-ttu-id="14cc9-1223">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1223">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1224">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1224">ACS</span></span>
* <span data-ttu-id="14cc9-1225">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-1225">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1226">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1226">AMS</span></span>
* <span data-ttu-id="14cc9-1227">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="14cc9-1227">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1228">AppService</span></span>
* <span data-ttu-id="14cc9-1229">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1229">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="14cc9-1230">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-1230">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="14cc9-1231">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1231">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="14cc9-1232">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1232">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="14cc9-1233">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="14cc9-1233">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="14cc9-1234">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1234">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1235">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1235">Batch</span></span>
* <span data-ttu-id="14cc9-1236">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="14cc9-1236">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-1237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-1237">BatchAI</span></span>
* <span data-ttu-id="14cc9-1238">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1238">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1239">BotService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1239">BotService</span></span>
* <span data-ttu-id="14cc9-1240">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="14cc9-1240">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1241">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1241">CosmosDB</span></span>
* <span data-ttu-id="14cc9-1242">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1242">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="14cc9-1243">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1243">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="14cc9-1244">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-1244">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="14cc9-1245">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="14cc9-1245">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="14cc9-1246">EventGrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-1246">EventGrid</span></span>
* <span data-ttu-id="14cc9-1247">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="14cc9-1247">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="14cc9-1248">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="14cc9-1248">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="14cc9-1249">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="14cc9-1249">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="14cc9-1250">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1250">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="14cc9-1251">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1251">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1252">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1252">HDInsight</span></span>
* <span data-ttu-id="14cc9-1253">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1253">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-1254">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1254">IoT</span></span>
* <span data-ttu-id="14cc9-1255">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1255">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="14cc9-1256">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="14cc9-1256">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1257">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1257">Network</span></span>
* <span data-ttu-id="14cc9-1258">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="14cc9-1258">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="14cc9-1259">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1259">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="14cc9-1260">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="14cc9-1260">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="14cc9-1261">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="14cc9-1261">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1262">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1262">Resource</span></span>
* <span data-ttu-id="14cc9-1263">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="14cc9-1263">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="14cc9-1264">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1264">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="14cc9-1265">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1265">ServiceBus</span></span>
* <span data-ttu-id="14cc9-1266">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1266">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1267">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1267">SQL</span></span>
* <span data-ttu-id="14cc9-1268">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="14cc9-1268">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="14cc9-1269">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1269">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="14cc9-1270">SQLVm</span><span class="sxs-lookup"><span data-stu-id="14cc9-1270">SQLVm</span></span>
* <span data-ttu-id="14cc9-1271">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1271">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="14cc9-1272">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1272">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1273">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1273">Storage</span></span>
* <span data-ttu-id="14cc9-1274">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1274">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="14cc9-1275">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1275">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1276">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1276">VM</span></span>
* <span data-ttu-id="14cc9-1277">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1277">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="14cc9-1278">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1278">June 4, 2019</span></span>

<span data-ttu-id="14cc9-1279">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="14cc9-1279">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1280">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1280">Core</span></span>
* <span data-ttu-id="14cc9-1281">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1281">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1282">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1282">ACR</span></span>
* <span data-ttu-id="14cc9-1283">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1283">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1284">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1284">ACS</span></span>
* <span data-ttu-id="14cc9-1285">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1285">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="14cc9-1286">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="14cc9-1286">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1287">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1287">Batch</span></span>
* <span data-ttu-id="14cc9-1288">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="14cc9-1288">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-1289">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1289">IoT</span></span>
* <span data-ttu-id="14cc9-1290">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-1290">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1291">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1291">Network</span></span>
* <span data-ttu-id="14cc9-1292">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1292">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="14cc9-1293">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1293">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="14cc9-1294">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1294">Resource</span></span>
* <span data-ttu-id="14cc9-1295">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="14cc9-1295">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1296">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1296">Role</span></span>
* <span data-ttu-id="14cc9-1297">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-1297">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-1298">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-1298">Compute</span></span>
* <span data-ttu-id="14cc9-1299">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="14cc9-1299">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="14cc9-1300">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1300">May 21, 2019</span></span>

<span data-ttu-id="14cc9-1301">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="14cc9-1301">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1302">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1302">Core</span></span>
* <span data-ttu-id="14cc9-1303">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="14cc9-1303">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="14cc9-1304">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="14cc9-1304">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="14cc9-1305">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1305">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1306">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1306">ACR</span></span>
* <span data-ttu-id="14cc9-1307">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="14cc9-1307">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1308">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1308">ACS</span></span>
* <span data-ttu-id="14cc9-1309">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="14cc9-1309">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1310">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1310">AppService</span></span>
* <span data-ttu-id="14cc9-1311">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1311">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="14cc9-1312">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1312">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="14cc9-1313">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1313">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="14cc9-1314">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1314">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="14cc9-1315">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1315">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="14cc9-1316">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1316">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="14cc9-1317">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1317">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1318">BotService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1318">BotService</span></span>
* <span data-ttu-id="14cc9-1319">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1319">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="14cc9-1320">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-1320">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-1321">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1321">Consumption</span></span>
* <span data-ttu-id="14cc9-1322">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1322">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-1323">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1323">IoT</span></span>
* <span data-ttu-id="14cc9-1324">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-1324">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1325">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1325">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="14cc9-1327">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1327">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="14cc9-1328">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1328">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1329">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1329">RDBMS</span></span>
* <span data-ttu-id="14cc9-1330">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="14cc9-1330">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-1331">RBAC</span><span class="sxs-lookup"><span data-stu-id="14cc9-1331">RBAC</span></span>
* <span data-ttu-id="14cc9-1332">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1332">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1333">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1333">Storage</span></span>
* <span data-ttu-id="14cc9-1334">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1334">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="14cc9-1335">Calcul</span><span class="sxs-lookup"><span data-stu-id="14cc9-1335">Compute</span></span>
* <span data-ttu-id="14cc9-1336">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1336">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="14cc9-1337">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="14cc9-1337">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="14cc9-1338">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1338">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="14cc9-1339">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1339">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="14cc9-1340">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1340">May 6, 2019</span></span>

<span data-ttu-id="14cc9-1341">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="14cc9-1341">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1342">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1342">ACS</span></span>
* <span data-ttu-id="14cc9-1343">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1343">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="14cc9-1344">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="14cc9-1344">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="14cc9-1345">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1345">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="14cc9-1346">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1346">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1347">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1347">Appservice</span></span>
* <span data-ttu-id="14cc9-1348">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="14cc9-1348">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="14cc9-1349">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1349">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="14cc9-1350">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1350">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="14cc9-1351">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="14cc9-1351">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="14cc9-1352">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1352">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="14cc9-1353">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1353">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="14cc9-1354">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="14cc9-1354">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="14cc9-1355">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="14cc9-1355">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="14cc9-1356">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-1356">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="14cc9-1357">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1357">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1358">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1358">Batch</span></span>
* <span data-ttu-id="14cc9-1359">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1359">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1360">Botservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-1360">Botservice</span></span>
* <span data-ttu-id="14cc9-1361">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1361">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="14cc9-1362">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1362">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="14cc9-1363">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1363">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="14cc9-1364">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1364">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="14cc9-1365">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1365">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="14cc9-1366">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1366">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="14cc9-1367">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1367">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="14cc9-1368">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1368">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="14cc9-1369">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-1369">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="14cc9-1370">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="14cc9-1370">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="14cc9-1371">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="14cc9-1371">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="14cc9-1372">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1372">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="14cc9-1373">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="14cc9-1373">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="14cc9-1374">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1374">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="14cc9-1375">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1375">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="14cc9-1376">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="14cc9-1376">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="14cc9-1377">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1377">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="14cc9-1378">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1378">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="14cc9-1379">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="14cc9-1379">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="14cc9-1380">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1380">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="14cc9-1381">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1381">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="14cc9-1382">Configurer</span><span class="sxs-lookup"><span data-stu-id="14cc9-1382">Configure</span></span>
* <span data-ttu-id="14cc9-1383">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="14cc9-1383">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="14cc9-1384">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="14cc9-1384">Eventhubs</span></span>
* <span data-ttu-id="14cc9-1385">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1385">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="14cc9-1386">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1386">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1387">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1387">Network</span></span>
* <span data-ttu-id="14cc9-1388">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1388">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="14cc9-1389">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-1389">Policy Insights</span></span>
* <span data-ttu-id="14cc9-1390">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1390">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1391">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1391">Role</span></span>
* <span data-ttu-id="14cc9-1392">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1392">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="14cc9-1393">Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1393">Service Bus</span></span>
* <span data-ttu-id="14cc9-1394">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1394">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="14cc9-1395">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1395">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="14cc9-1396">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="14cc9-1396">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1397">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1397">SQL</span></span>
* <span data-ttu-id="14cc9-1398">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1398">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1399">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1399">VM</span></span>
* <span data-ttu-id="14cc9-1400">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1400">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="14cc9-1401">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1401">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="14cc9-1402">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1402">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="14cc9-1403">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="14cc9-1403">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="14cc9-1404">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="14cc9-1404">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="14cc9-1405">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1405">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="14cc9-1406">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1406">April 23, 2019</span></span>

<span data-ttu-id="14cc9-1407">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="14cc9-1407">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1408">ACS</span></span>
* <span data-ttu-id="14cc9-1409">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1409">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="14cc9-1410">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="14cc9-1410">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1411">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1411">AMS</span></span>
* <span data-ttu-id="14cc9-1412">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="14cc9-1412">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1413">AppService</span></span>
* <span data-ttu-id="14cc9-1414">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1414">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="14cc9-1415">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="14cc9-1415">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="14cc9-1416">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="14cc9-1416">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="14cc9-1417">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="14cc9-1417">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="14cc9-1418">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="14cc9-1418">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="14cc9-1419">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1419">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="14cc9-1420">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="14cc9-1420">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="14cc9-1421">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1421">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="14cc9-1422">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1422">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="14cc9-1423">Deployment Manager</span><span class="sxs-lookup"><span data-stu-id="14cc9-1423">Deployment Manager</span></span>
* <span data-ttu-id="14cc9-1424">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="14cc9-1424">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="14cc9-1425">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-1425">Lab</span></span>
* <span data-ttu-id="14cc9-1426">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="14cc9-1426">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1427">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1427">Network</span></span>
* <span data-ttu-id="14cc9-1428">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="14cc9-1428">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1429">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1429">Resource</span></span>
* <span data-ttu-id="14cc9-1430">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1430">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="14cc9-1431">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1431">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="14cc9-1432">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1432">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="14cc9-1433">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1433">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1434">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1434">SQL</span></span>
* <span data-ttu-id="14cc9-1435">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1435">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="14cc9-1436">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1436">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="14cc9-1437">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1437">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="14cc9-1438">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1438">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1439">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1439">Storage</span></span>
* <span data-ttu-id="14cc9-1440">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1440">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1441">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1441">VM</span></span>
* <span data-ttu-id="14cc9-1442">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="14cc9-1442">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="14cc9-1443">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="14cc9-1443">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="14cc9-1444">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="14cc9-1444">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="14cc9-1445">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1445">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1446">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1446">Core</span></span>
* <span data-ttu-id="14cc9-1447">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-1447">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1448">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1448">ACR</span></span>
* <span data-ttu-id="14cc9-1449">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="14cc9-1449">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1450">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1450">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="14cc9-1453">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1453">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="14cc9-1454">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1454">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1455">AppService</span></span>
* <span data-ttu-id="14cc9-1456">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1456">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="14cc9-1457">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1457">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="14cc9-1458">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1458">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="14cc9-1459">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="14cc9-1459">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="14cc9-1460">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1460">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="14cc9-1461">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1461">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="14cc9-1462">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="14cc9-1462">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-1463">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-1463">CDN</span></span>
* <span data-ttu-id="14cc9-1464">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1464">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="14cc9-1465">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14cc9-1465">Feedback</span></span>
* <span data-ttu-id="14cc9-1466">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="14cc9-1466">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="14cc9-1467">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="14cc9-1467">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="14cc9-1468">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="14cc9-1468">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1469">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1469">Monitor</span></span>
* <span data-ttu-id="14cc9-1470">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1470">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="14cc9-1471">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1471">Network</span></span>
* <span data-ttu-id="14cc9-1472">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1472">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="14cc9-1473">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1473">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="14cc9-1474">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1474">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="14cc9-1475">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1475">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="14cc9-1476">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1476">PrivateDNS</span></span>
* <span data-ttu-id="14cc9-1477">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1477">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1478">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1478">Resource</span></span>
* <span data-ttu-id="14cc9-1479">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1479">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1480">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1480">Role</span></span>
* <span data-ttu-id="14cc9-1481">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1481">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="14cc9-1482">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1482">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1483">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1483">SQL</span></span>
* <span data-ttu-id="14cc9-1484">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="14cc9-1484">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1485">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1485">Storage</span></span>
* <span data-ttu-id="14cc9-1486">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1486">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="14cc9-1487">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1487">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="14cc9-1488">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="14cc9-1488">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="14cc9-1489">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1489">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="14cc9-1490">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1490">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="14cc9-1491">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1491">Core</span></span>
* <span data-ttu-id="14cc9-1492">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1492">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="14cc9-1493">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1493">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="14cc9-1494">Cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-1494">Cloud</span></span>
* <span data-ttu-id="14cc9-1495">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1495">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1496">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1496">ACR</span></span>
* <span data-ttu-id="14cc9-1497">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="14cc9-1497">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="14cc9-1498">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1498">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="14cc9-1499">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="14cc9-1499">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="14cc9-1500">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1500">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1501">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1501">AppService</span></span>
* <span data-ttu-id="14cc9-1502">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="14cc9-1502">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="14cc9-1503">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1503">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="14cc9-1504">Service BOT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1504">BOT Service</span></span>
* <span data-ttu-id="14cc9-1505">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1505">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="14cc9-1506">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-1506">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="14cc9-1507">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="14cc9-1507">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="14cc9-1508">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="14cc9-1508">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-1509">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-1509">CDN</span></span>
* <span data-ttu-id="14cc9-1510">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1510">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="14cc9-1511">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1511">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="14cc9-1512">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-1512">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="14cc9-1513">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1513">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1514">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="14cc9-1514">Cosmosdb</span></span>
* <span data-ttu-id="14cc9-1515">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="14cc9-1515">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="14cc9-1516">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1516">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-1517">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-1517">Interactive</span></span>
* <span data-ttu-id="14cc9-1518">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="14cc9-1518">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1519">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1519">Monitor</span></span>
* <span data-ttu-id="14cc9-1520">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1520">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1521">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1521">Network</span></span>
* <span data-ttu-id="14cc9-1522">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1522">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-1523">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-1523">Profile</span></span>
* <span data-ttu-id="14cc9-1524">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1524">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="14cc9-1525">Postgres</span><span class="sxs-lookup"><span data-stu-id="14cc9-1525">Postgres</span></span> 
* <span data-ttu-id="14cc9-1526">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="14cc9-1526">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="14cc9-1527">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1527">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1528">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1528">Resource</span></span>
* <span data-ttu-id="14cc9-1529">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1529">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="14cc9-1530">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="14cc9-1530">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="14cc9-1531">Graph</span><span class="sxs-lookup"><span data-stu-id="14cc9-1531">Graph</span></span>
* <span data-ttu-id="14cc9-1532">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1532">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="14cc9-1533">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1533">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="14cc9-1534">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1534">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="14cc9-1535">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1535">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="14cc9-1536">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-1536">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1537">storage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1537">storage</span></span>
* <span data-ttu-id="14cc9-1538">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1538">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="14cc9-1539">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="14cc9-1539">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="14cc9-1540">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1540">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="14cc9-1541">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1541">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1542">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1542">VM</span></span>
* <span data-ttu-id="14cc9-1543">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1543">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="14cc9-1544">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1544">March 12, 2019</span></span>

<span data-ttu-id="14cc9-1545">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="14cc9-1545">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1546">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1546">Core</span></span>

* <span data-ttu-id="14cc9-1547">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="14cc9-1547">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1548">ACR</span></span>

* <span data-ttu-id="14cc9-1549">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="14cc9-1549">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1550">ACS</span></span>

* <span data-ttu-id="14cc9-1551">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="14cc9-1551">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="14cc9-1552">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1552">AppService</span></span>

* <span data-ttu-id="14cc9-1553">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="14cc9-1553">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="14cc9-1554">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1554">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="14cc9-1555">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1555">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="14cc9-1556">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-1556">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1557">Botservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-1557">Botservice</span></span>

* <span data-ttu-id="14cc9-1558">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="14cc9-1558">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="14cc9-1559">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="14cc9-1559">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="14cc9-1560">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1560">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="14cc9-1561">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="14cc9-1561">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-1562">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1562">Container</span></span>

* <span data-ttu-id="14cc9-1563">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1563">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="14cc9-1564">Event Hub</span><span class="sxs-lookup"><span data-stu-id="14cc9-1564">EventHub</span></span>

* <span data-ttu-id="14cc9-1565">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="14cc9-1565">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="14cc9-1566">Rechercher</span><span class="sxs-lookup"><span data-stu-id="14cc9-1566">Find</span></span>

* <span data-ttu-id="14cc9-1567">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="14cc9-1567">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1568">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1568">HDInsight</span></span>

* <span data-ttu-id="14cc9-1569">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="14cc9-1569">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1570">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1570">Network</span></span>

* <span data-ttu-id="14cc9-1571">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="14cc9-1571">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1572">Rdbms</span><span class="sxs-lookup"><span data-stu-id="14cc9-1572">Rdbms</span></span>

* <span data-ttu-id="14cc9-1573">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="14cc9-1573">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1574">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1574">Role</span></span>

* <span data-ttu-id="14cc9-1575">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="14cc9-1575">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="14cc9-1576">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="14cc9-1576">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14cc9-1577">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-1577">Service Fabric</span></span>

* <span data-ttu-id="14cc9-1578">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="14cc9-1578">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="14cc9-1579">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1579">February 26, 2019</span></span>

<span data-ttu-id="14cc9-1580">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="14cc9-1580">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1581">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1581">Core</span></span>

* <span data-ttu-id="14cc9-1582">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1582">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1583">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1583">ACR</span></span>

* <span data-ttu-id="14cc9-1584">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1584">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="14cc9-1585">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="14cc9-1585">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1586">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1586">ACS</span></span>

* <span data-ttu-id="14cc9-1587">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1587">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1588">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1588">AppService</span></span>

* <span data-ttu-id="14cc9-1589">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1589">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-1590">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-1590">Batch</span></span>
* <span data-ttu-id="14cc9-1591">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1591">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="14cc9-1592">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1592">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="14cc9-1593">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="14cc9-1593">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="14cc9-1594">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1594">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="14cc9-1595">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="14cc9-1595">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="14cc9-1596">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="14cc9-1596">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1597">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1597">CosmosDB</span></span>

* <span data-ttu-id="14cc9-1598">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1598">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="14cc9-1599">Kusto</span><span class="sxs-lookup"><span data-stu-id="14cc9-1599">Kusto</span></span>

* <span data-ttu-id="14cc9-1600">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="14cc9-1600">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1601">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1601">Network</span></span>

* <span data-ttu-id="14cc9-1602">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1602">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="14cc9-1603">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1603">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="14cc9-1604">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1604">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="14cc9-1605">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1605">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="14cc9-1606">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1606">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="14cc9-1607">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1607">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="14cc9-1608">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1608">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1609">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1609">Resource</span></span>

* <span data-ttu-id="14cc9-1610">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-1610">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="14cc9-1611">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1611">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="14cc9-1612">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1612">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="14cc9-1613">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1613">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="14cc9-1614">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1614">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1615">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1615">Role</span></span>

* <span data-ttu-id="14cc9-1616">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1616">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1617">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1617">VM</span></span>

* <span data-ttu-id="14cc9-1618">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-1618">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="14cc9-1619">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1619">February 12, 2019</span></span>

<span data-ttu-id="14cc9-1620">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="14cc9-1620">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1621">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1621">Core</span></span>

* <span data-ttu-id="14cc9-1622">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-1622">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="14cc9-1623">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="14cc9-1623">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1624">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1624">ACR</span></span>
* <span data-ttu-id="14cc9-1625">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1625">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="14cc9-1626">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1626">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1627">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1627">ACS</span></span>
* <span data-ttu-id="14cc9-1628">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1628">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="14cc9-1629">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1629">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="14cc9-1630">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1630">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1631">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1631">AMS</span></span>
* <span data-ttu-id="14cc9-1632">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1632">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="14cc9-1633">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1633">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1634">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1634">Appservice</span></span>
* <span data-ttu-id="14cc9-1635">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1635">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="14cc9-1636">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="14cc9-1636">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="14cc9-1637">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1637">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="14cc9-1638">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="14cc9-1638">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="14cc9-1639">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="14cc9-1639">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1640">Botservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-1640">Botservice</span></span>
* <span data-ttu-id="14cc9-1641">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1641">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="14cc9-1642">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1642">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="14cc9-1643">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1643">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="14cc9-1644">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-1644">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="14cc9-1645">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1645">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="14cc9-1646">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="14cc9-1646">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="14cc9-1647">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1647">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="14cc9-1648">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="14cc9-1648">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="14cc9-1649">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1649">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="14cc9-1650">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="14cc9-1650">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-1651">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-1651">Key Vault</span></span>
* <span data-ttu-id="14cc9-1652">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1652">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1653">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1653">Monitor</span></span>
* <span data-ttu-id="14cc9-1654">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1654">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1655">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1655">Network</span></span>
* <span data-ttu-id="14cc9-1656">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="14cc9-1656">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="14cc9-1657">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="14cc9-1657">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="14cc9-1658">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-1658">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="14cc9-1659">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1659">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="14cc9-1660">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-1660">Policy Insights</span></span>
* <span data-ttu-id="14cc9-1661">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-1661">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1662">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1662">RDBMS</span></span>
* <span data-ttu-id="14cc9-1663">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-1663">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-1664">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-1664">Redis</span></span>
* <span data-ttu-id="14cc9-1665">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1665">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="14cc9-1666">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1666">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="14cc9-1667">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1667">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="14cc9-1668">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="14cc9-1668">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="14cc9-1669">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1669">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="14cc9-1670">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="14cc9-1670">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="14cc9-1671">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1671">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1672">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1672">Role</span></span>
* <span data-ttu-id="14cc9-1673">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1673">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="14cc9-1674">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1674">SQL VM</span></span>
* <span data-ttu-id="14cc9-1675">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="14cc9-1675">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1676">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1676">VM</span></span>
* <span data-ttu-id="14cc9-1677">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1677">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="14cc9-1678">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1678">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="14cc9-1679">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="14cc9-1679">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="14cc9-1680">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1680">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="14cc9-1681">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1681">January 31, 2019</span></span>

<span data-ttu-id="14cc9-1682">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="14cc9-1682">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1683">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1683">Core</span></span>

* <span data-ttu-id="14cc9-1684">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="14cc9-1684">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="14cc9-1685">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1685">January 28, 2019</span></span>

<span data-ttu-id="14cc9-1686">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="14cc9-1686">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1687">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1687">ACR</span></span>
* <span data-ttu-id="14cc9-1688">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="14cc9-1688">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1689">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1689">ACS</span></span>
* <span data-ttu-id="14cc9-1690">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="14cc9-1690">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="14cc9-1691">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1691">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="14cc9-1692">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1692">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1693">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1693">AMS</span></span>
* <span data-ttu-id="14cc9-1694">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1694">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="14cc9-1695">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1695">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1696">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1696">Appservice</span></span>
* <span data-ttu-id="14cc9-1697">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1697">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="14cc9-1698">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="14cc9-1698">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="14cc9-1699">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="14cc9-1699">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-1700">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1700">Container</span></span>
* <span data-ttu-id="14cc9-1701">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1701">Added `container start` command</span></span>
* <span data-ttu-id="14cc9-1702">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1702">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="14cc9-1703">EventGrid</span><span class="sxs-lookup"><span data-stu-id="14cc9-1703">EventGrid</span></span>
* <span data-ttu-id="14cc9-1704">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1704">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="14cc9-1705">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="14cc9-1705">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="14cc9-1706">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="14cc9-1706">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="14cc9-1707">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1707">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="14cc9-1708">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="14cc9-1708">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1709">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1709">HDInsight</span></span>
* <span data-ttu-id="14cc9-1710">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1710">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="14cc9-1711">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="14cc9-1711">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="14cc9-1712">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1712">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="14cc9-1713">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1713">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="14cc9-1714">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1714">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="14cc9-1715">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1715">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-1716">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-1716">IoT</span></span>
* <span data-ttu-id="14cc9-1717">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="14cc9-1717">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="14cc9-1718">Kusto</span><span class="sxs-lookup"><span data-stu-id="14cc9-1718">Kusto</span></span>
* <span data-ttu-id="14cc9-1719">Préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-1719">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1720">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1720">Monitor</span></span>
* <span data-ttu-id="14cc9-1721">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-1721">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-1722">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-1722">Profile</span></span>
* <span data-ttu-id="14cc9-1723">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1723">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1724">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1724">Network</span></span>
* <span data-ttu-id="14cc9-1725">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="14cc9-1725">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="14cc9-1726">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="14cc9-1726">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1727">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1727">Resource</span></span>
* <span data-ttu-id="14cc9-1728">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1728">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="14cc9-1729">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1729">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="14cc9-1730">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1730">SQL Virtual Machine</span></span>
* <span data-ttu-id="14cc9-1731">Préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-1731">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1732">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1732">Storage</span></span>
* <span data-ttu-id="14cc9-1733">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="14cc9-1733">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="14cc9-1734">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1734">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1735">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1735">VM</span></span>
* <span data-ttu-id="14cc9-1736">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1736">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="14cc9-1737">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1737">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="14cc9-1738">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="14cc9-1738">January 15, 2019</span></span>

<span data-ttu-id="14cc9-1739">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="14cc9-1739">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1740">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1740">ACR</span></span>
* <span data-ttu-id="14cc9-1741">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1741">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="14cc9-1742">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-1742">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="14cc9-1743">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1743">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="14cc9-1744">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1744">ACS</span></span>
* <span data-ttu-id="14cc9-1745">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="14cc9-1745">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1746">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1746">Appservice</span></span>
* <span data-ttu-id="14cc9-1747">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="14cc9-1747">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="14cc9-1748">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1748">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="14cc9-1749">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1749">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="14cc9-1750">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1750">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1751">Botservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-1751">Botservice</span></span>
* <span data-ttu-id="14cc9-1752">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1752">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="14cc9-1753">Configurer</span><span class="sxs-lookup"><span data-stu-id="14cc9-1753">Configure</span></span>
* <span data-ttu-id="14cc9-1754">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="14cc9-1754">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1755">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1755">CosmosDB</span></span>
* <span data-ttu-id="14cc9-1756">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1756">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-1757">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-1757">HDInsight</span></span>
* <span data-ttu-id="14cc9-1758">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="14cc9-1758">Added commands for managing applications</span></span>
* <span data-ttu-id="14cc9-1759">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="14cc9-1759">Added commands for managing script actions</span></span>
* <span data-ttu-id="14cc9-1760">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1760">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="14cc9-1761">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1761">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="14cc9-1762">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1762">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1763">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1763">Network</span></span>
* <span data-ttu-id="14cc9-1764">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1764">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="14cc9-1765">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="14cc9-1765">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="14cc9-1766">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1766">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="14cc9-1767">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1767">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1768">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1768">Role</span></span>
* <span data-ttu-id="14cc9-1769">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1769">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="14cc9-1770">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="14cc9-1770">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="14cc9-1771">Sécurité</span><span class="sxs-lookup"><span data-stu-id="14cc9-1771">Security</span></span>
* <span data-ttu-id="14cc9-1772">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-1772">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1773">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1773">Storage</span></span>
* <span data-ttu-id="14cc9-1774">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1774">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="14cc9-1775">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="14cc9-1775">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="14cc9-1776">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1776">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="14cc9-1777">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1777">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="14cc9-1778">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-1778">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1779">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1779">VM</span></span>
* <span data-ttu-id="14cc9-1780">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="14cc9-1780">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="14cc9-1781">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1781">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="14cc9-1782">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1782">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="14cc9-1783">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-1783">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="14cc9-1784">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1784">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="14cc9-1785">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-1785">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="14cc9-1786">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1786">December 20, 2018</span></span>

<span data-ttu-id="14cc9-1787">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="14cc9-1787">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="14cc9-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1788">Appservice</span></span>
* <span data-ttu-id="14cc9-1789">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1789">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="14cc9-1790">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="14cc9-1790">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="14cc9-1791">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-1791">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="14cc9-1792">IotCentral</span><span class="sxs-lookup"><span data-stu-id="14cc9-1792">IoTCentral</span></span>
* <span data-ttu-id="14cc9-1793">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-1793">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1794">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1794">Role</span></span>
* <span data-ttu-id="14cc9-1795">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1795">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-1796">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1796">SQL</span></span>
* <span data-ttu-id="14cc9-1797">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1797">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1798">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1798">VM</span></span>
* <span data-ttu-id="14cc9-1799">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1799">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="14cc9-1800">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1800">December 18, 2018</span></span>

<span data-ttu-id="14cc9-1801">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="14cc9-1801">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="14cc9-1802">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1802">ACR</span></span>
* <span data-ttu-id="14cc9-1803">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1803">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="14cc9-1804">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="14cc9-1804">Condensed the table layout for task list</span></span>
* <span data-ttu-id="14cc9-1805">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="14cc9-1805">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1806">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1806">ACS</span></span>
* <span data-ttu-id="14cc9-1807">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="14cc9-1807">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="14cc9-1808">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1808">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="14cc9-1809">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1809">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="14cc9-1810">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1810">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="14cc9-1811">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1811">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="14cc9-1812">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="14cc9-1812">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1813">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1813">Appservice</span></span>
* <span data-ttu-id="14cc9-1814">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1814">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="14cc9-1815">Botservice</span><span class="sxs-lookup"><span data-stu-id="14cc9-1815">Botservice</span></span>
* <span data-ttu-id="14cc9-1816">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1816">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="14cc9-1817">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="14cc9-1817">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="14cc9-1818">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="14cc9-1818">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="14cc9-1819">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="14cc9-1819">Reduced Kudu network calls</span></span>
* <span data-ttu-id="14cc9-1820">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="14cc9-1820">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-1821">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-1821">Consumption</span></span>
* <span data-ttu-id="14cc9-1822">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="14cc9-1822">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1823">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1823">CosmosDB</span></span>
* <span data-ttu-id="14cc9-1824">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1824">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="14cc9-1825">Cartes</span><span class="sxs-lookup"><span data-stu-id="14cc9-1825">Maps</span></span>
* <span data-ttu-id="14cc9-1826">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1826">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1827">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1827">Network</span></span>
* <span data-ttu-id="14cc9-1828">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1828">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="14cc9-1829">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-1829">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1830">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1830">Resource</span></span>
* <span data-ttu-id="14cc9-1831">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1831">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="14cc9-1832">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1832">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1833">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1833">Storage</span></span>
*  <span data-ttu-id="14cc9-1834">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1834">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1835">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1835">VM</span></span>
* <span data-ttu-id="14cc9-1836">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="14cc9-1836">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="14cc9-1837">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1837">December 4, 2018</span></span>

<span data-ttu-id="14cc9-1838">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="14cc9-1838">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="14cc9-1839">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1839">Core</span></span>
* <span data-ttu-id="14cc9-1840">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1840">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="14cc9-1841">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1841">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1842">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1842">Appservice</span></span>
* <span data-ttu-id="14cc9-1843">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1843">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="14cc9-1844">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1844">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1845">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1845">Network</span></span>
* <span data-ttu-id="14cc9-1846">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="14cc9-1846">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1847">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1847">Role</span></span>
* <span data-ttu-id="14cc9-1848">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1848">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="14cc9-1849">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1849">VM</span></span>
* <span data-ttu-id="14cc9-1850">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1850">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="14cc9-1851">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1851">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="14cc9-1852">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1852">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="14cc9-1853">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1853">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="14cc9-1854">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1854">November 20, 2018</span></span>

<span data-ttu-id="14cc9-1855">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="14cc9-1855">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="14cc9-1856">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1856">Core</span></span>
* <span data-ttu-id="14cc9-1857">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="14cc9-1857">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1858">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1858">ACR</span></span>
* <span data-ttu-id="14cc9-1859">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="14cc9-1859">Added context token to task step</span></span>
* <span data-ttu-id="14cc9-1860">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="14cc9-1860">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="14cc9-1861">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1861">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1862">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1862">Appservice</span></span>
* <span data-ttu-id="14cc9-1863">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1863">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="14cc9-1864">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1864">Updated the default `node_version`.</span></span> <span data-ttu-id="14cc9-1865">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="14cc9-1865">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="14cc9-1866">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1866">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="14cc9-1867">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="14cc9-1867">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="14cc9-1868">IotCentral</span><span class="sxs-lookup"><span data-stu-id="14cc9-1868">IotCentral</span></span>
* <span data-ttu-id="14cc9-1869">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-1869">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-1870">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-1870">KeyVault</span></span>
* <span data-ttu-id="14cc9-1871">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="14cc9-1871">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1872">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1872">Network</span></span>
* <span data-ttu-id="14cc9-1873">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="14cc9-1873">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="14cc9-1874">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1874">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="14cc9-1875">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1875">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="14cc9-1876">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1876">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1877">Rdbms</span><span class="sxs-lookup"><span data-stu-id="14cc9-1877">Rdbms</span></span>
* <span data-ttu-id="14cc9-1878">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="14cc9-1878">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="14cc9-1879">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="14cc9-1879">Rbac</span></span>
* <span data-ttu-id="14cc9-1880">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1880">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="14cc9-1881">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1881">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="14cc9-1882">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1882">Storage</span></span>
* <span data-ttu-id="14cc9-1883">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1883">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="14cc9-1884">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-1884">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="14cc9-1885">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="14cc9-1885">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="14cc9-1886">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="14cc9-1886">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1887">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1887">VM</span></span>
* <span data-ttu-id="14cc9-1888">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="14cc9-1888">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="14cc9-1889">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1889">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="14cc9-1890">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1890">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="14cc9-1891">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1891">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="14cc9-1892">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1892">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="14cc9-1893">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1893">Added `snapshot wait` command</span></span>
* <span data-ttu-id="14cc9-1894">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1894">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="14cc9-1895">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1895">November 6, 2018</span></span>

<span data-ttu-id="14cc9-1896">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="14cc9-1896">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1897">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1897">Core</span></span>
* <span data-ttu-id="14cc9-1898">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="14cc9-1898">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1899">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1899">ACR</span></span>
* <span data-ttu-id="14cc9-1900">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="14cc9-1900">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="14cc9-1901">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="14cc9-1901">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-1902">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1902">ACS</span></span>
* <span data-ttu-id="14cc9-1903">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-1903">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="14cc9-1904">Advisor</span><span class="sxs-lookup"><span data-stu-id="14cc9-1904">Advisor</span></span>
* <span data-ttu-id="14cc9-1905">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="14cc9-1905">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-1906">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-1906">AMS</span></span>
* <span data-ttu-id="14cc9-1907">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1907">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="14cc9-1908">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1908">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="14cc9-1909">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1909">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="14cc9-1910">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="14cc9-1910">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="14cc9-1911">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1911">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="14cc9-1912">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1912">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="14cc9-1913">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1913">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="14cc9-1914">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1914">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="14cc9-1915">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1915">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="14cc9-1916">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1916">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="14cc9-1917">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1917">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="14cc9-1918">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1918">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="14cc9-1919">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="14cc9-1919">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="14cc9-1920">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="14cc9-1920">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="14cc9-1921">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1921">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="14cc9-1922">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="14cc9-1922">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="14cc9-1923">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="14cc9-1923">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-1924">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-1924">AppService</span></span>
* <span data-ttu-id="14cc9-1925">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="14cc9-1925">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="14cc9-1926">Configurer</span><span class="sxs-lookup"><span data-stu-id="14cc9-1926">Configure</span></span>
* <span data-ttu-id="14cc9-1927">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="14cc9-1927">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-1928">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1928">Container</span></span>
* <span data-ttu-id="14cc9-1929">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="14cc9-1929">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="14cc9-1930">Event Hub</span><span class="sxs-lookup"><span data-stu-id="14cc9-1930">EventHub</span></span>
* <span data-ttu-id="14cc9-1931">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1931">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-1932">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-1932">Interactive</span></span>
* <span data-ttu-id="14cc9-1933">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="14cc9-1933">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1934">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1934">Monitor</span></span>
* <span data-ttu-id="14cc9-1935">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1935">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1936">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1936">Network</span></span>
* <span data-ttu-id="14cc9-1937">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1937">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="14cc9-1938">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1938">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="14cc9-1939">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1939">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="14cc9-1940">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-1940">Profile</span></span>
* <span data-ttu-id="14cc9-1941">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="14cc9-1941">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-1942">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1942">RDBMS</span></span>
* <span data-ttu-id="14cc9-1943">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="14cc9-1943">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-1944">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-1944">Resource</span></span>
* <span data-ttu-id="14cc9-1945">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1945">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-1946">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-1946">Role</span></span>
* <span data-ttu-id="14cc9-1947">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="14cc9-1947">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="14cc9-1948">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1948">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="14cc9-1949">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="14cc9-1949">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-1950">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-1950">Storage</span></span>
* <span data-ttu-id="14cc9-1951">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1951">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-1952">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-1952">VM</span></span>
* <span data-ttu-id="14cc9-1953">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="14cc9-1953">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="14cc9-1954">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-1954">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="14cc9-1955">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="14cc9-1955">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="14cc9-1956">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="14cc9-1956">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="14cc9-1957">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="14cc9-1957">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="14cc9-1958">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1958">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="14cc9-1959">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-1959">October 23, 2018</span></span>

<span data-ttu-id="14cc9-1960">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="14cc9-1960">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-1961">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-1961">Core</span></span>
* <span data-ttu-id="14cc9-1962">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1962">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="14cc9-1963">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1963">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-1964">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-1964">ACR</span></span>
* <span data-ttu-id="14cc9-1965">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="14cc9-1965">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-1966">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-1966">CDN</span></span>
* <span data-ttu-id="14cc9-1967">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="14cc9-1967">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="14cc9-1968">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1968">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-1969">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-1969">Container</span></span>
* <span data-ttu-id="14cc9-1970">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="14cc9-1970">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="14cc9-1971">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-1971">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="14cc9-1972">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="14cc9-1972">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="14cc9-1973">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-1973">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="14cc9-1974">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="14cc9-1974">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="14cc9-1975">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="14cc9-1975">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="14cc9-1976">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1976">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-1977">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-1977">CosmosDB</span></span>
* <span data-ttu-id="14cc9-1978">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1978">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-1979">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-1979">Interactive</span></span>
* <span data-ttu-id="14cc9-1980">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="14cc9-1980">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="14cc9-1981">IoT Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-1981">IoT Central</span></span>
* <span data-ttu-id="14cc9-1982">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="14cc9-1982">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="14cc9-1983">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="14cc9-1983">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-1984">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-1984">Monitor</span></span>
* <span data-ttu-id="14cc9-1985">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1985">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="14cc9-1986">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-1986">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="14cc9-1987">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="14cc9-1987">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="14cc9-1988">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1988">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="14cc9-1989">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1989">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="14cc9-1990">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="14cc9-1990">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="14cc9-1991">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="14cc9-1991">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="14cc9-1992">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="14cc9-1992">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="14cc9-1993">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="14cc9-1993">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="14cc9-1994">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-1994">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-1995">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1995">Network</span></span>
* <span data-ttu-id="14cc9-1996">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1996">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="14cc9-1997">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-1997">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="14cc9-1998">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1998">ServiceBus</span></span>
* <span data-ttu-id="14cc9-1999">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-1999">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2000">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2000">SQL</span></span>
* <span data-ttu-id="14cc9-2001">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-2001">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2002">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2002">Storage</span></span>
* <span data-ttu-id="14cc9-2003">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="14cc9-2003">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="14cc9-2004">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2004">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2005">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2005">VM</span></span>
* <span data-ttu-id="14cc9-2006">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2006">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="14cc9-2007">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2007">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="14cc9-2008">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2008">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="14cc9-2009">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2009">October 16, 2018</span></span>

<span data-ttu-id="14cc9-2010">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="14cc9-2010">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2011">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2011">VM</span></span>
* <span data-ttu-id="14cc9-2012">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="14cc9-2012">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="14cc9-2013">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2013">October 9, 2018</span></span>

<span data-ttu-id="14cc9-2014">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="14cc9-2014">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2015">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2015">Core</span></span>
* <span data-ttu-id="14cc9-2016">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2016">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2017">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2017">ACR</span></span>
* <span data-ttu-id="14cc9-2018">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="14cc9-2018">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2019">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2019">ACS</span></span>
* <span data-ttu-id="14cc9-2020">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="14cc9-2020">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="14cc9-2021">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="14cc9-2021">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="14cc9-2022">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2022">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="14cc9-2023">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2023">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2024">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2024">Container</span></span>
* <span data-ttu-id="14cc9-2025">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2025">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="14cc9-2026">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-2026">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="14cc9-2027">Event Hub</span><span class="sxs-lookup"><span data-stu-id="14cc9-2027">Event Hub</span></span>
* <span data-ttu-id="14cc9-2028">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2028">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="14cc9-2029">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2029">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="14cc9-2030">Extensions</span><span class="sxs-lookup"><span data-stu-id="14cc9-2030">Extensions</span></span>
* <span data-ttu-id="14cc9-2031">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2031">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="14cc9-2032">HDInsight</span><span class="sxs-lookup"><span data-stu-id="14cc9-2032">HDInsight</span></span>
* <span data-ttu-id="14cc9-2033">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-2033">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2034">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2034">IoT</span></span>
* <span data-ttu-id="14cc9-2035">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="14cc9-2035">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-2036">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-2036">KeyVault</span></span>
* <span data-ttu-id="14cc9-2037">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="14cc9-2037">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2038">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2038">Network</span></span>
* <span data-ttu-id="14cc9-2039">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2039">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="14cc9-2040">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="14cc9-2040">See #6052</span></span>
* <span data-ttu-id="14cc9-2041">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2041">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="14cc9-2042">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="14cc9-2042">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="14cc9-2043">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2043">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="14cc9-2044">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2044">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="14cc9-2045">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2045">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="14cc9-2046">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2046">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2047">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2047">Role</span></span>
* <span data-ttu-id="14cc9-2048">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2048">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="14cc9-2049">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2049">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="14cc9-2050">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="14cc9-2050">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="14cc9-2051">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2051">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="14cc9-2052">Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-2052">Service Bus</span></span>
* <span data-ttu-id="14cc9-2053">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2053">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2054">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2054">VM</span></span>
* <span data-ttu-id="14cc9-2055">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2055">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="14cc9-2056">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2056">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="14cc9-2057">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2057">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="14cc9-2058">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2058">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="14cc9-2059">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2059">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="14cc9-2060">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="14cc9-2060">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="14cc9-2061">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2061">September 21, 2018</span></span>

<span data-ttu-id="14cc9-2062">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="14cc9-2062">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2063">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2063">ACR</span></span>
* <span data-ttu-id="14cc9-2064">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2064">Added ACR Task commands</span></span>
* <span data-ttu-id="14cc9-2065">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2065">Added quick run command</span></span>
* <span data-ttu-id="14cc9-2066">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2066">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="14cc9-2067">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2067">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="14cc9-2068">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2068">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="14cc9-2069">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="14cc9-2069">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2070">ACS</span></span>
* <span data-ttu-id="14cc9-2071">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2071">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="14cc9-2072">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="14cc9-2072">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2073">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2073">AppService</span></span>

* <span data-ttu-id="14cc9-2074">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2074">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="14cc9-2075">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="14cc9-2075">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="14cc9-2076">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="14cc9-2076">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="14cc9-2077">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2077">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2078">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2078">Batch</span></span>
* <span data-ttu-id="14cc9-2079">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="14cc9-2079">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="14cc9-2080">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2080">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="14cc9-2081">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2081">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="14cc9-2082">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2082">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="14cc9-2083">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2083">Batch AI</span></span> 
* <span data-ttu-id="14cc9-2084">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2084">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="14cc9-2085">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2085">Cognitive Services</span></span>
* <span data-ttu-id="14cc9-2086">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2086">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="14cc9-2087">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2087">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="14cc9-2088">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2088">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="14cc9-2089">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2089">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="14cc9-2090">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2090">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="14cc9-2091">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2091">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2092">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2092">Container</span></span>
* <span data-ttu-id="14cc9-2093">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="14cc9-2093">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="14cc9-2094">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2094">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="14cc9-2095">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-2095">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="14cc9-2096">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2096">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="14cc9-2097">DataLake</span><span class="sxs-lookup"><span data-stu-id="14cc9-2097">Datalake</span></span>
* <span data-ttu-id="14cc9-2098">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-2098">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="14cc9-2099">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="14cc9-2099">Interactive Shell</span></span>
* <span data-ttu-id="14cc9-2100">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2100">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="14cc9-2101">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2101">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2102">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2102">IoT</span></span>
* <span data-ttu-id="14cc9-2103">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2103">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-2104">Key Vault</span><span class="sxs-lookup"><span data-stu-id="14cc9-2104">Key Vault</span></span>
* <span data-ttu-id="14cc9-2105">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="14cc9-2105">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2106">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2106">Network</span></span>
* <span data-ttu-id="14cc9-2107">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2107">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="14cc9-2108">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-2108">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="14cc9-2109">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="14cc9-2109">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="14cc9-2110">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2110">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="14cc9-2111">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2111">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="14cc9-2112">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2112">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="14cc9-2113">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2113">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="14cc9-2114">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2114">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="14cc9-2115">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2115">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="14cc9-2116">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2116">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="14cc9-2117">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2117">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="14cc9-2118">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2118">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="14cc9-2119">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2119">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="14cc9-2120">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2120">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="14cc9-2121">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2121">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="14cc9-2122">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="14cc9-2122">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="14cc9-2123">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2123">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="14cc9-2124">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2124">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-2125">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2125">RDBMS</span></span>
* <span data-ttu-id="14cc9-2126">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-2126">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="14cc9-2127">Réservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2127">Reservation</span></span>
* <span data-ttu-id="14cc9-2128">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2128">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="14cc9-2129">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2129">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="14cc9-2130">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="14cc9-2130">Manage App</span></span>
* <span data-ttu-id="14cc9-2131">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2131">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="14cc9-2132">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="14cc9-2132">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2133">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2133">Role</span></span>
* <span data-ttu-id="14cc9-2134">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2134">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="14cc9-2135">SignalR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2135">SignalR</span></span>
* <span data-ttu-id="14cc9-2136">Première version</span><span class="sxs-lookup"><span data-stu-id="14cc9-2136">First release</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2137">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2137">Storage</span></span>
* <span data-ttu-id="14cc9-2138">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="14cc9-2138">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="14cc9-2139">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="14cc9-2139">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2140">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2140">VM</span></span>
* <span data-ttu-id="14cc9-2141">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2141">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="14cc9-2142">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2142">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="14cc9-2143">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2143">August 28, 2018</span></span>

<span data-ttu-id="14cc9-2144">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="14cc9-2144">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2145">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2145">Core</span></span>

* <span data-ttu-id="14cc9-2146">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2146">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="14cc9-2147">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14cc9-2147">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2148">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2148">ACR</span></span>

* <span data-ttu-id="14cc9-2149">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-2149">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="14cc9-2150">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2150">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2151">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2151">ACS</span></span>

* <span data-ttu-id="14cc9-2152">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2152">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="14cc9-2153">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="14cc9-2153">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2154">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2154">AppService</span></span>

* <span data-ttu-id="14cc9-2155">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="14cc9-2155">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="14cc9-2156">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="14cc9-2156">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="14cc9-2157">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2157">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-2158">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-2158">Backup</span></span>

* <span data-ttu-id="14cc9-2159">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2159">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="14cc9-2160">Service de robot</span><span class="sxs-lookup"><span data-stu-id="14cc9-2160">Bot Service</span></span>

* <span data-ttu-id="14cc9-2161">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="14cc9-2161">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="14cc9-2162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2162">Cognitive Services</span></span>

* <span data-ttu-id="14cc9-2163">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2163">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2164">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2164">IoT</span></span>

* <span data-ttu-id="14cc9-2165">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2165">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-2166">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2166">Monitor</span></span>

* <span data-ttu-id="14cc9-2167">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="14cc9-2167">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="14cc9-2168">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2168">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2169">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2169">Network</span></span>

* <span data-ttu-id="14cc9-2170">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2170">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2171">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2171">Resource</span></span>

* <span data-ttu-id="14cc9-2172">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2172">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2173">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2173">Storage</span></span>

* <span data-ttu-id="14cc9-2174">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2174">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2175">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2175">VM</span></span>

* <span data-ttu-id="14cc9-2176">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2176">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="14cc9-2177">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2177">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="14cc9-2178">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2178">Auguest 14, 2018</span></span>

<span data-ttu-id="14cc9-2179">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="14cc9-2179">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2180">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2180">Core</span></span>

* <span data-ttu-id="14cc9-2181">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2181">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="14cc9-2182">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="14cc9-2182">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="14cc9-2183">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2183">Telemetry</span></span>

* <span data-ttu-id="14cc9-2184">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2184">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2185">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2185">ACR</span></span>

* <span data-ttu-id="14cc9-2186">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2186">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="14cc9-2187">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2187">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2188">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2188">ACS</span></span>

* <span data-ttu-id="14cc9-2189">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-2189">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="14cc9-2190">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2190">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="14cc9-2191">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2191">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="14cc9-2192">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2192">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="14cc9-2193">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="14cc9-2193">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="14cc9-2194">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2194">AppService</span></span>

* <span data-ttu-id="14cc9-2195">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2195">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="14cc9-2196">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="14cc9-2196">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-2197">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2197">BatchAI</span></span>

* <span data-ttu-id="14cc9-2198">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="14cc9-2198">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="14cc9-2199">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2199">Container</span></span>

* <span data-ttu-id="14cc9-2200">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2200">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="14cc9-2201">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2201">IoT</span></span>

* <span data-ttu-id="14cc9-2202">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="14cc9-2202">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="14cc9-2203">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2203">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="14cc9-2204">Iot Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-2204">Iot Central</span></span>

* <span data-ttu-id="14cc9-2205">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="14cc9-2205">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-2206">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-2206">KeyVault</span></span>


* <span data-ttu-id="14cc9-2207">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2207">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="14cc9-2208">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2208">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="14cc9-2209">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="14cc9-2209">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="14cc9-2210">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2210">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="14cc9-2211">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2211">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="14cc9-2212">Relais</span><span class="sxs-lookup"><span data-stu-id="14cc9-2212">Relay</span></span>

* <span data-ttu-id="14cc9-2213">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-2213">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2214">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2214">Sql</span></span>

* <span data-ttu-id="14cc9-2215">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2215">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2216">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2216">Storage</span></span>

* <span data-ttu-id="14cc9-2217">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="14cc9-2217">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="14cc9-2218">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2218">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="14cc9-2219">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2219">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="14cc9-2220">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="14cc9-2220">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="14cc9-2221">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2221">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2222">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2222">VM</span></span>

* <span data-ttu-id="14cc9-2223">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2223">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="14cc9-2224">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2224">July 31, 2018</span></span>

<span data-ttu-id="14cc9-2225">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="14cc9-2225">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2226">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2226">ACR</span></span>

* <span data-ttu-id="14cc9-2227">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2227">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="14cc9-2228">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2228">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2229">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2229">ACS</span></span>

* <span data-ttu-id="14cc9-2230">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2230">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2231">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2231">Batch</span></span>

* <span data-ttu-id="14cc9-2232">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-2232">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2233">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2233">Container</span></span>

* <span data-ttu-id="14cc9-2234">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="14cc9-2234">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2235">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2235">Network</span></span>

* <span data-ttu-id="14cc9-2236">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14cc9-2236">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="14cc9-2237">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2237">Resource</span></span>

* <span data-ttu-id="14cc9-2238">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2238">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="14cc9-2239">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2239">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2240">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2240">Role</span></span>

* <span data-ttu-id="14cc9-2241">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-2241">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="14cc9-2242">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2242">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="14cc9-2243">Recherche</span><span class="sxs-lookup"><span data-stu-id="14cc9-2243">Search</span></span>

* <span data-ttu-id="14cc9-2244">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="14cc9-2244">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="14cc9-2245">Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-2245">Service Bus</span></span>

* <span data-ttu-id="14cc9-2246">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="14cc9-2246">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="14cc9-2247">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2247">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="14cc9-2248">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2248">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="14cc9-2249">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2249">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2250">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2250">Storage</span></span>

* <span data-ttu-id="14cc9-2251">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2251">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="14cc9-2252">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2252">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2253">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2253">VM</span></span>

* <span data-ttu-id="14cc9-2254">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2254">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="14cc9-2255">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2255">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="14cc9-2256">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="14cc9-2256">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="14cc9-2257">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="14cc9-2257">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="14cc9-2258">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2258">July 18, 2018</span></span>

<span data-ttu-id="14cc9-2259">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="14cc9-2259">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2260">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2260">Core</span></span>

* <span data-ttu-id="14cc9-2261">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-2261">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="14cc9-2262">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2262">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="14cc9-2263">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="14cc9-2263">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2264">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2264">ACR</span></span>

* <span data-ttu-id="14cc9-2265">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2265">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="14cc9-2266">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2266">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="14cc9-2267">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2267">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="14cc9-2268">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="14cc9-2268">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2269">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2269">ACS</span></span>

* <span data-ttu-id="14cc9-2270">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="14cc9-2270">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2271">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2271">AppService</span></span>

* <span data-ttu-id="14cc9-2272">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="14cc9-2272">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2273">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2273">Batch</span></span>

* <span data-ttu-id="14cc9-2274">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-2274">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="14cc9-2275">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-2275">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="14cc9-2276">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2276">Batch AI</span></span>

* <span data-ttu-id="14cc9-2277">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2277">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2278">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2278">Container</span></span>

* <span data-ttu-id="14cc9-2279">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="14cc9-2279">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="14cc9-2280">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="14cc9-2280">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2281">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2281">Network</span></span>

* <span data-ttu-id="14cc9-2282">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2282">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="14cc9-2283">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2283">Added `network nic wait`</span></span>
* <span data-ttu-id="14cc9-2284">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2284">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="14cc9-2285">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2285">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="14cc9-2286">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2286">Resource</span></span>

* <span data-ttu-id="14cc9-2287">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2287">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="14cc9-2288">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2288">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="14cc9-2289">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2289">Added `deployment wait` command</span></span>
* <span data-ttu-id="14cc9-2290">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="14cc9-2290">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2291">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2291">SQL</span></span>

* <span data-ttu-id="14cc9-2292">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2292">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="14cc9-2293">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2293">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="14cc9-2294">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2294">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2295">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2295">Storage</span></span>

* <span data-ttu-id="14cc9-2296">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="14cc9-2296">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2297">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2297">VM</span></span>

* <span data-ttu-id="14cc9-2298">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2298">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="14cc9-2299">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2299">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="14cc9-2300">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2300">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="14cc9-2301">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2301">July 3, 2018</span></span>

<span data-ttu-id="14cc9-2302">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="14cc9-2302">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-2303">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2303">AKS</span></span>

* <span data-ttu-id="14cc9-2304">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2304">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="14cc9-2305">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2305">July 3, 2018</span></span>

<span data-ttu-id="14cc9-2306">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="14cc9-2306">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2307">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2307">Core</span></span>

* <span data-ttu-id="14cc9-2308">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2308">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2309">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2309">ACR</span></span>

* <span data-ttu-id="14cc9-2310">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="14cc9-2310">Added polling build status</span></span>
* <span data-ttu-id="14cc9-2311">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-2311">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="14cc9-2312">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2312">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2313">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2313">ACS</span></span>

* <span data-ttu-id="14cc9-2314">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2314">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="14cc9-2315">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2315">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="14cc9-2316">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2316">Updated options for `aks browse` command.</span></span> <span data-ttu-id="14cc9-2317">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2317">Added `--listen-port` support</span></span>
* <span data-ttu-id="14cc9-2318">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2318">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="14cc9-2319">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="14cc9-2319">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="14cc9-2320">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="14cc9-2320">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2321">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2321">AppService</span></span>

* <span data-ttu-id="14cc9-2322">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2322">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="14cc9-2323">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="14cc9-2323">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-2324">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-2324">Backup</span></span>

* <span data-ttu-id="14cc9-2325">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="14cc9-2325">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-2326">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2326">BatchAI</span></span>

* <span data-ttu-id="14cc9-2327">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2327">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="14cc9-2328">Cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-2328">Cloud</span></span>

* <span data-ttu-id="14cc9-2329">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-2329">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2330">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2330">Container</span></span>

* <span data-ttu-id="14cc9-2331">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="14cc9-2331">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="14cc9-2332">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2332">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="14cc9-2333">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2333">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2334">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2334">Extension</span></span>

* <span data-ttu-id="14cc9-2335">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2335">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2336">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2336">Network</span></span>

* <span data-ttu-id="14cc9-2337">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="14cc9-2337">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-2338">Rdbms</span><span class="sxs-lookup"><span data-stu-id="14cc9-2338">Rdbms</span></span>

* <span data-ttu-id="14cc9-2339">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2339">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2340">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2340">Resource</span></span>

* <span data-ttu-id="14cc9-2341">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2341">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2342">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2342">VM</span></span>

* <span data-ttu-id="14cc9-2343">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="14cc9-2343">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="14cc9-2344">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2344">June 25, 2018</span></span>

<span data-ttu-id="14cc9-2345">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="14cc9-2345">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="14cc9-2346">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-2346">CLI</span></span>

* <span data-ttu-id="14cc9-2347">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2347">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="14cc9-2348">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2348">June 19, 2018</span></span>

<span data-ttu-id="14cc9-2349">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="14cc9-2349">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2350">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2350">Core</span></span>

* <span data-ttu-id="14cc9-2351">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2351">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2352">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2352">ACR</span></span>

* <span data-ttu-id="14cc9-2353">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="14cc9-2353">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="14cc9-2354">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2354">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2355">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2355">ACS</span></span>

* <span data-ttu-id="14cc9-2356">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2356">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="14cc9-2357">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2357">Added `--update` support</span></span>
* <span data-ttu-id="14cc9-2358">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2358">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="14cc9-2359">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2359">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="14cc9-2360">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2360">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="14cc9-2361">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2361">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="14cc9-2362">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2362">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="14cc9-2363">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2363">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2364">AppService</span></span>

* <span data-ttu-id="14cc9-2365">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2365">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="14cc9-2366">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2366">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2367">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2367">Batch</span></span>

* <span data-ttu-id="14cc9-2368">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2368">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="14cc9-2369">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2369">Batch AI</span></span>

* <span data-ttu-id="14cc9-2370">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2370">Added support for workspaces.</span></span> <span data-ttu-id="14cc9-2371">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2371">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="14cc9-2372">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2372">Added support for experiments.</span></span> <span data-ttu-id="14cc9-2373">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2373">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="14cc9-2374">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="14cc9-2374">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="14cc9-2375">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2375">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="14cc9-2376">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2376">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="14cc9-2377">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2377">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="14cc9-2378">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-2378">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="14cc9-2379">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="14cc9-2379">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="14cc9-2380">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2380">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="14cc9-2381">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2381">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="14cc9-2382">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2382">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="14cc9-2383">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2383">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="14cc9-2384">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2384">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="14cc9-2385">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2385">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="14cc9-2386">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2386">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="14cc9-2387">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2387">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="14cc9-2388">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2388">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="14cc9-2389">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2389">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="14cc9-2390">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2390">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="14cc9-2391">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2391">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="14cc9-2392">Cartes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2392">Maps</span></span>

* <span data-ttu-id="14cc9-2393">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2393">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2394">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2394">Network</span></span>

* <span data-ttu-id="14cc9-2395">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2395">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="14cc9-2396">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2396">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="14cc9-2397">#6502</span><span class="sxs-lookup"><span data-stu-id="14cc9-2397">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="14cc9-2398">Réservations</span><span class="sxs-lookup"><span data-stu-id="14cc9-2398">Reservations</span></span>

* <span data-ttu-id="14cc9-2399">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2399">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="14cc9-2400">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2400">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="14cc9-2401">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2401">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="14cc9-2402">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2402">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="14cc9-2403">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2403">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="14cc9-2404">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2404">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2405">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2405">Role</span></span>

* <span data-ttu-id="14cc9-2406">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2406">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2407">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2407">SQL</span></span>

* <span data-ttu-id="14cc9-2408">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2408">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2409">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2409">Storage</span></span>

* <span data-ttu-id="14cc9-2410">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="14cc9-2410">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2411">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2411">VM</span></span>

* <span data-ttu-id="14cc9-2412">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2412">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="14cc9-2413">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2413">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="14cc9-2414">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2414">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="14cc9-2415">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2415">June 13, 2018</span></span>

<span data-ttu-id="14cc9-2416">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="14cc9-2416">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2417">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2417">Core</span></span>

* <span data-ttu-id="14cc9-2418">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2418">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="14cc9-2419">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2419">June 13, 2018</span></span>

<span data-ttu-id="14cc9-2420">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="14cc9-2420">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-2421">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2421">AKS</span></span>

* <span data-ttu-id="14cc9-2422">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2422">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="14cc9-2423">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="14cc9-2423">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="14cc9-2424">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2424">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="14cc9-2425">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2425">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="14cc9-2426">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2426">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2427">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2427">AppService</span></span>

* <span data-ttu-id="14cc9-2428">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="14cc9-2428">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="14cc9-2429">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2429">June 5, 2018</span></span>

<span data-ttu-id="14cc9-2430">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="14cc9-2430">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2431">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2431">Interactive</span></span>

* <span data-ttu-id="14cc9-2432">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="14cc9-2432">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="14cc9-2433">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2433">June 5, 2018</span></span>

<span data-ttu-id="14cc9-2434">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="14cc9-2434">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2435">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2435">Core</span></span>

* <span data-ttu-id="14cc9-2436">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="14cc9-2436">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="14cc9-2437">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2437">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2438">ACR</span></span>

* <span data-ttu-id="14cc9-2439">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="14cc9-2439">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="14cc9-2440">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2440">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="14cc9-2441">AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2441">AKS</span></span>

* <span data-ttu-id="14cc9-2442">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2442">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2443">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2443">Batch</span></span>

* <span data-ttu-id="14cc9-2444">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="14cc9-2444">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2445">IOT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2445">IOT</span></span>

* <span data-ttu-id="14cc9-2446">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="14cc9-2446">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2447">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2447">Network</span></span>

* <span data-ttu-id="14cc9-2448">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="14cc9-2448">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="14cc9-2449">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="14cc9-2449">Policy Insights</span></span>

* <span data-ttu-id="14cc9-2450">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-2450">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="14cc9-2451">ARM</span><span class="sxs-lookup"><span data-stu-id="14cc9-2451">ARM</span></span>

* <span data-ttu-id="14cc9-2452">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2452">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2453">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2453">SQL</span></span>

* <span data-ttu-id="14cc9-2454">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2454">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="14cc9-2455">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2455">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="14cc9-2456">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2456">Storage</span></span>

* <span data-ttu-id="14cc9-2457">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="14cc9-2457">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2458">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2458">VM</span></span>

* <span data-ttu-id="14cc9-2459">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2459">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="14cc9-2460">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2460">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="14cc9-2461">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2461">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="14cc9-2462">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2462">May 22, 2018</span></span>

<span data-ttu-id="14cc9-2463">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="14cc9-2463">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2464">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2464">Core</span></span>

* <span data-ttu-id="14cc9-2465">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="14cc9-2465">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2466">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2466">ACS</span></span>

* <span data-ttu-id="14cc9-2467">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2467">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="14cc9-2468">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2468">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2469">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2469">AppService</span></span>

* <span data-ttu-id="14cc9-2470">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2470">Improved generic update commands</span></span>
* <span data-ttu-id="14cc9-2471">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2471">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2472">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2472">Container</span></span>

* <span data-ttu-id="14cc9-2473">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="14cc9-2473">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="14cc9-2474">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2474">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2475">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2475">Extension</span></span>

* <span data-ttu-id="14cc9-2476">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="14cc9-2476">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2477">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2477">Interactive</span></span>

* <span data-ttu-id="14cc9-2478">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2478">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="14cc9-2479">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="14cc9-2479">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-2480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-2480">KeyVault</span></span>

* <span data-ttu-id="14cc9-2481">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="14cc9-2481">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2482">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2482">Network</span></span>

* <span data-ttu-id="14cc9-2483">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2483">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="14cc9-2484">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2484">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2485">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2485">SQL</span></span>

* <span data-ttu-id="14cc9-2486">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2486">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="14cc9-2487">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2487">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="14cc9-2488">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2488">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="14cc9-2489">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="14cc9-2489">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="14cc9-2490">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2490">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="14cc9-2491">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2491">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="14cc9-2492">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2492">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="14cc9-2493">`edition`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2493">`edition`.</span></span> <span data-ttu-id="14cc9-2494">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2494">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="14cc9-2495">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2495">`elasticPoolName`.</span></span> <span data-ttu-id="14cc9-2496">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2496">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="14cc9-2497">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2497">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="14cc9-2498">`edition`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2498">`edition`.</span></span> <span data-ttu-id="14cc9-2499">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2499">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="14cc9-2500">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2500">`dtu`.</span></span> <span data-ttu-id="14cc9-2501">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2501">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="14cc9-2502">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2502">`databaseDtuMin`.</span></span> <span data-ttu-id="14cc9-2503">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2503">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="14cc9-2504">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2504">`databaseDtuMax`.</span></span> <span data-ttu-id="14cc9-2505">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2505">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="14cc9-2506">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2506">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="14cc9-2507">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2507">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2508">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2508">Storage</span></span>

* <span data-ttu-id="14cc9-2509">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2509">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="14cc9-2510">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2510">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2511">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2511">VM</span></span>

* <span data-ttu-id="14cc9-2512">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2512">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="14cc9-2513">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2513">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="14cc9-2514">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2514">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="14cc9-2515">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2515">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="14cc9-2516">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2516">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="14cc9-2517">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2517">May 7, 2018</span></span>

<span data-ttu-id="14cc9-2518">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="14cc9-2518">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2519">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2519">Core</span></span>

* <span data-ttu-id="14cc9-2520">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="14cc9-2520">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="14cc9-2521">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="14cc9-2521">Added limited support for positional arguments</span></span>
* <span data-ttu-id="14cc9-2522">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2522">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="14cc9-2523">#5591</span><span class="sxs-lookup"><span data-stu-id="14cc9-2523">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="14cc9-2524">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2524">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="14cc9-2525">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="14cc9-2525">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="14cc9-2526">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2526">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="14cc9-2527">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2527">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="14cc9-2528">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-2528">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2529">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2529">ACR</span></span>

* <span data-ttu-id="14cc9-2530">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2530">Added ACR Build commands</span></span>
* <span data-ttu-id="14cc9-2531">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="14cc9-2531">Improved resource not found error messages</span></span>
* <span data-ttu-id="14cc9-2532">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2532">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="14cc9-2533">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2533">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="14cc9-2534">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="14cc9-2534">Improved repository commands error messages</span></span>
* <span data-ttu-id="14cc9-2535">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2535">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2536">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2536">ACS</span></span>

* <span data-ttu-id="14cc9-2537">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-2537">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="14cc9-2538">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="14cc9-2538">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="14cc9-2539">AMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2539">AMS</span></span>

* <span data-ttu-id="14cc9-2540">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2540">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2541">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2541">Appservice</span></span>

* <span data-ttu-id="14cc9-2542">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="14cc9-2542">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="14cc9-2543">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2543">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="14cc9-2544">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-2544">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="14cc9-2545">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2545">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="14cc9-2546">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2546">Batch AI</span></span>

* <span data-ttu-id="14cc9-2547">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="14cc9-2547">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="14cc9-2548">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2548">Cognitive Services</span></span>

* <span data-ttu-id="14cc9-2549">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2549">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-2550">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2550">Consumption</span></span>

* <span data-ttu-id="14cc9-2551">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="14cc9-2551">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2552">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2552">Container</span></span>

* <span data-ttu-id="14cc9-2553">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="14cc9-2553">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="14cc9-2554">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-2554">Cosmos DB</span></span>

* <span data-ttu-id="14cc9-2555">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="14cc9-2555">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="14cc9-2556">DMS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2556">DMS</span></span>

* <span data-ttu-id="14cc9-2557">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="14cc9-2557">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2558">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2558">Extension</span></span>

* <span data-ttu-id="14cc9-2559">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2559">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2560">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2560">Interactive</span></span>

* <span data-ttu-id="14cc9-2561">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="14cc9-2561">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="14cc9-2562">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="14cc9-2562">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="14cc9-2563">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2563">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="14cc9-2564">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2564">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="14cc9-2565">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-2565">Lab</span></span>

* <span data-ttu-id="14cc9-2566">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="14cc9-2566">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2567">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2567">Network</span></span>

* <span data-ttu-id="14cc9-2568">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2568">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="14cc9-2569">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2569">Profile</span></span>

* <span data-ttu-id="14cc9-2570">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2570">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="14cc9-2571">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2571">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="14cc9-2572">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2572">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-2573">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-2573">Redis</span></span>

* <span data-ttu-id="14cc9-2574">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2574">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="14cc9-2575">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2575">Deprecated `redis list-all`.</span></span> <span data-ttu-id="14cc9-2576">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2576">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="14cc9-2577">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2577">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="14cc9-2578">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2578">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2579">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2579">Role</span></span>

* <span data-ttu-id="14cc9-2580">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2580">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2581">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2581">Storage</span></span>

* <span data-ttu-id="14cc9-2582">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2582">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="14cc9-2583">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="14cc9-2583">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="14cc9-2584">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2584">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="14cc9-2585">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2585">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="14cc9-2586">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2586">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2587">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2587">VM</span></span>

* <span data-ttu-id="14cc9-2588">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2588">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="14cc9-2589">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2589">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="14cc9-2590">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2590">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="14cc9-2591">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2591">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="14cc9-2592">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2592">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="14cc9-2593">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="14cc9-2593">Added write accelerator support</span></span>
* <span data-ttu-id="14cc9-2594">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2594">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="14cc9-2595">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2595">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="14cc9-2596">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="14cc9-2596">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="14cc9-2597">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2597">April 10, 2018</span></span>

<span data-ttu-id="14cc9-2598">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="14cc9-2598">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2599">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2599">ACR</span></span>

* <span data-ttu-id="14cc9-2600">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="14cc9-2600">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2601">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2601">ACS</span></span>

* <span data-ttu-id="14cc9-2602">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="14cc9-2602">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2603">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2603">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="14cc9-2605">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="14cc9-2605">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-2606">Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2606">BatchAI</span></span>

* <span data-ttu-id="14cc9-2607">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-2607">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="14cc9-2608">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-2608">Job level mounting</span></span>
  - <span data-ttu-id="14cc9-2609">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="14cc9-2609">Environment variables with secret values</span></span>
  - <span data-ttu-id="14cc9-2610">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="14cc9-2610">Performance counters settings</span></span>
  - <span data-ttu-id="14cc9-2611">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-2611">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="14cc9-2612">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="14cc9-2612">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="14cc9-2613">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="14cc9-2613">Usage and limits reporting</span></span>
  - <span data-ttu-id="14cc9-2614">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2614">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="14cc9-2615">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2615">Support for custom images</span></span>
  - <span data-ttu-id="14cc9-2616">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2616">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="14cc9-2617">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-2617">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="14cc9-2618">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="14cc9-2618">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="14cc9-2619">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="14cc9-2619">National clouds are supported</span></span>
* <span data-ttu-id="14cc9-2620">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="14cc9-2620">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="14cc9-2621">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2621">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="14cc9-2622">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2622">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="14cc9-2623">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2623">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="14cc9-2624">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2624">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="14cc9-2625">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2625">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="14cc9-2626">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2626">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="14cc9-2627">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2627">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="14cc9-2628">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="14cc9-2628">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="14cc9-2629">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2629">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="14cc9-2630">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-2630">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="14cc9-2631">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2631">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="14cc9-2632">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2632">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="14cc9-2633">Facturation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2633">Billing</span></span>

* <span data-ttu-id="14cc9-2634">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="14cc9-2634">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-2635">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2635">Consumption</span></span>

* <span data-ttu-id="14cc9-2636">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2636">Added `marketplace` commands</span></span>
* <span data-ttu-id="14cc9-2637">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2637">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="14cc9-2638">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2638">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="14cc9-2639">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2639">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="14cc9-2640">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2640">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="14cc9-2641">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2641">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2642">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2642">Container</span></span>

* <span data-ttu-id="14cc9-2643">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2643">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="14cc9-2644">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="14cc9-2644">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2645">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2645">Extension</span></span>

* <span data-ttu-id="14cc9-2646">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2646">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2647">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2647">Interactive</span></span>

* <span data-ttu-id="14cc9-2648">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="14cc9-2648">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="14cc9-2649">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-2649">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="14cc9-2650">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2650">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2651">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2651">Network</span></span>

* <span data-ttu-id="14cc9-2652">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="14cc9-2652">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="14cc9-2653">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2653">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="14cc9-2654">#4910</span><span class="sxs-lookup"><span data-stu-id="14cc9-2654">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="14cc9-2655">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2655">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="14cc9-2656">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2656">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="14cc9-2657">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2657">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="14cc9-2658">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2658">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="14cc9-2659">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2659">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-2660">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2660">Profile</span></span>

* <span data-ttu-id="14cc9-2661">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2661">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="14cc9-2662">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2662">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-2663">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2663">RDBMS</span></span>

* <span data-ttu-id="14cc9-2664">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2664">Added `georestore` command</span></span>
* <span data-ttu-id="14cc9-2665">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2665">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2666">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2666">Resource</span></span>

* <span data-ttu-id="14cc9-2667">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2667">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="14cc9-2668">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2668">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2669">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2669">SQL</span></span>

* <span data-ttu-id="14cc9-2670">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2670">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2671">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2671">Storage</span></span>

* <span data-ttu-id="14cc9-2672">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2672">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2673">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2673">VM</span></span>

* <span data-ttu-id="14cc9-2674">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2674">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="14cc9-2675">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2675">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="14cc9-2677">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2677">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="14cc9-2678">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2678">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="14cc9-2679">#5718</span><span class="sxs-lookup"><span data-stu-id="14cc9-2679">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="14cc9-2680">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="14cc9-2680">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="14cc9-2681">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2681">March 27, 2018</span></span>

<span data-ttu-id="14cc9-2682">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="14cc9-2682">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2683">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2683">Core</span></span>

* <span data-ttu-id="14cc9-2684">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2684">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2685">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2685">ACS</span></span>

* <span data-ttu-id="14cc9-2686">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-2686">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2687">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2687">Appservice</span></span>

* <span data-ttu-id="14cc9-2688">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2688">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="14cc9-2689">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2689">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-2690">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-2690">Backup</span></span>

* <span data-ttu-id="14cc9-2691">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2691">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="14cc9-2692">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2692">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="14cc9-2693">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2693">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="14cc9-2694">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2694">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2695">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2695">Container</span></span>

* <span data-ttu-id="14cc9-2696">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2696">Added `container exec` command.</span></span> <span data-ttu-id="14cc9-2697">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2697">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="14cc9-2698">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2698">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2699">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2699">Extension</span></span>

* <span data-ttu-id="14cc9-2700">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-2700">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="14cc9-2701">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2701">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="14cc9-2702">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2702">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2703">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2703">Interactive</span></span>

* <span data-ttu-id="14cc9-2704">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-2704">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="14cc9-2705">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2705">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="14cc9-2706">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="14cc9-2706">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="14cc9-2707">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="14cc9-2707">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="14cc9-2708">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-2708">Lab</span></span>

* <span data-ttu-id="14cc9-2709">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2709">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-2710">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2710">Monitor</span></span>

* <span data-ttu-id="14cc9-2711">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2711">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="14cc9-2712">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="14cc9-2712">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="14cc9-2713">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2713">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2714">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2714">Network</span></span>

* <span data-ttu-id="14cc9-2715">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2715">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-2716">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2716">Profile</span></span>

* <span data-ttu-id="14cc9-2717">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2717">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-2718">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2718">RDBMS</span></span>

* <span data-ttu-id="14cc9-2719">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-2719">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2720">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2720">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="14cc9-2722">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2722">Role</span></span>

* <span data-ttu-id="14cc9-2723">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2723">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="14cc9-2724">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="14cc9-2724">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="14cc9-2725">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2725">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="14cc9-2726">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2726">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="14cc9-2727">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2727">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2728">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2728">Storage</span></span>

* <span data-ttu-id="14cc9-2729">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="14cc9-2729">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="14cc9-2730">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="14cc9-2730">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2731">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2731">VM</span></span>

* <span data-ttu-id="14cc9-2732">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="14cc9-2732">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="14cc9-2733">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2733">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="14cc9-2734">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2734">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="14cc9-2735">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2735">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="14cc9-2736">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2736">March 13, 2018</span></span>

<span data-ttu-id="14cc9-2737">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="14cc9-2737">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2738">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2738">ACR</span></span>

* <span data-ttu-id="14cc9-2739">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2739">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="14cc9-2740">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2740">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="14cc9-2741">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="14cc9-2741">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2742">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2742">ACS</span></span>

* <span data-ttu-id="14cc9-2743">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="14cc9-2743">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="14cc9-2744">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="14cc9-2744">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="14cc9-2745">Advisor</span><span class="sxs-lookup"><span data-stu-id="14cc9-2745">Advisor</span></span>

* <span data-ttu-id="14cc9-2746">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2746">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="14cc9-2747">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2747">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="14cc9-2748">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2748">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="14cc9-2749">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2749">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="14cc9-2750">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2750">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2751">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2751">Appservice</span></span>

* <span data-ttu-id="14cc9-2752">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="14cc9-2752">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="14cc9-2753">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2753">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="14cc9-2754">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2754">Eventhubs</span></span>

* <span data-ttu-id="14cc9-2755">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-2755">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2756">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2756">Extension</span></span>

* <span data-ttu-id="14cc9-2757">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2757">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2758">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2758">Interactive</span></span>

* <span data-ttu-id="14cc9-2759">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="14cc9-2759">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="14cc9-2760">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="14cc9-2760">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="14cc9-2761">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="14cc9-2761">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="14cc9-2762">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="14cc9-2762">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-2763">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2763">Monitor</span></span>

* <span data-ttu-id="14cc9-2764">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2764">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="14cc9-2765">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2765">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="14cc9-2766">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2766">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="14cc9-2767">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2767">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2768">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2768">Network</span></span>

* <span data-ttu-id="14cc9-2769">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2769">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="14cc9-2770">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2770">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="14cc9-2771">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2771">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="14cc9-2772">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2772">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-2773">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2773">Profile</span></span>

* <span data-ttu-id="14cc9-2774">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2774">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="14cc9-2775">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2775">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-2776">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2776">RDBMS</span></span>

* <span data-ttu-id="14cc9-2777">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-2777">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="14cc9-2778">Service Bus</span><span class="sxs-lookup"><span data-stu-id="14cc9-2778">Service Bus</span></span>

* <span data-ttu-id="14cc9-2779">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-2779">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2780">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2780">Storage</span></span>

* <span data-ttu-id="14cc9-2781">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="14cc9-2781">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="14cc9-2782">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="14cc9-2782">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2783">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2783">VM</span></span>

* <span data-ttu-id="14cc9-2784">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="14cc9-2784">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="14cc9-2785">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2785">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="14cc9-2786">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2786">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="14cc9-2787">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="14cc9-2787">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="14cc9-2788">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2788">February 27, 2018</span></span>

<span data-ttu-id="14cc9-2789">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="14cc9-2789">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2790">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2790">Core</span></span>

* <span data-ttu-id="14cc9-2791">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="14cc9-2791">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="14cc9-2792">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="14cc9-2792">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="14cc9-2793">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2793">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2794">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2794">ACS</span></span>

* <span data-ttu-id="14cc9-2795">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2795">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="14cc9-2796">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2796">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="14cc9-2797">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2797">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="14cc9-2798">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2798">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2799">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2799">Appservice</span></span>

* <span data-ttu-id="14cc9-2800">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="14cc9-2800">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="14cc9-2801">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2801">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="14cc9-2802">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2802">Cognitive Services</span></span>

* <span data-ttu-id="14cc9-2803">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-2803">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-2804">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2804">Consumption</span></span>

* <span data-ttu-id="14cc9-2805">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="14cc9-2805">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="14cc9-2806">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2806">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2807">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2807">Container</span></span>

* <span data-ttu-id="14cc9-2808">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2808">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2809">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2809">Network</span></span>

* <span data-ttu-id="14cc9-2810">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2810">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2811">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2811">Resource</span></span>

* <span data-ttu-id="14cc9-2812">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="14cc9-2812">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2813">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2813">Role</span></span>

* <span data-ttu-id="14cc9-2814">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-2814">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2815">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2815">SQL</span></span>

* <span data-ttu-id="14cc9-2816">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="14cc9-2816">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2817">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2817">Storage</span></span>

* <span data-ttu-id="14cc9-2818">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2818">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2819">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2819">VM</span></span>

* <span data-ttu-id="14cc9-2820">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2820">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="14cc9-2821">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2821">February 13, 2018</span></span>

<span data-ttu-id="14cc9-2822">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="14cc9-2822">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2823">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2823">Core</span></span>

* <span data-ttu-id="14cc9-2824">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2824">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2825">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2825">ACS</span></span>

* <span data-ttu-id="14cc9-2826">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="14cc9-2826">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="14cc9-2827">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2827">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="14cc9-2828">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2828">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="14cc9-2829">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2829">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="14cc9-2830">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2830">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="14cc9-2831">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2831">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="14cc9-2832">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2832">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="14cc9-2833">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2833">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2834">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2834">Appservice</span></span>

* <span data-ttu-id="14cc9-2835">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="14cc9-2835">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="14cc9-2836">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2836">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-2837">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-2837">CDN</span></span>

* <span data-ttu-id="14cc9-2838">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2838">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2839">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2839">Container</span></span>

* <span data-ttu-id="14cc9-2840">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="14cc9-2840">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="14cc9-2841">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2841">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-2842">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-2842">CosmosDB</span></span>

* <span data-ttu-id="14cc9-2843">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="14cc9-2843">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-2844">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-2844">Extension</span></span>

* <span data-ttu-id="14cc9-2845">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2845">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="14cc9-2846">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2846">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="14cc9-2847">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14cc9-2847">Feedback</span></span>

* <span data-ttu-id="14cc9-2848">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="14cc9-2848">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2849">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2849">Interactive</span></span>

* <span data-ttu-id="14cc9-2850">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14cc9-2850">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="14cc9-2851">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="14cc9-2851">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2852">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2852">IoT</span></span>

* <span data-ttu-id="14cc9-2853">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="14cc9-2853">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="14cc9-2854">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="14cc9-2854">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="14cc9-2855">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2855">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="14cc9-2856">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="14cc9-2856">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-2857">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2857">Monitor</span></span>

* <span data-ttu-id="14cc9-2858">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2858">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2859">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2859">Network</span></span>

* <span data-ttu-id="14cc9-2860">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2860">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="14cc9-2861">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2861">Profile</span></span>

* <span data-ttu-id="14cc9-2862">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="14cc9-2862">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2863">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2863">Resource</span></span>

* <span data-ttu-id="14cc9-2864">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2864">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2865">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2865">Role</span></span>

* <span data-ttu-id="14cc9-2866">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2866">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-2867">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-2867">SQL</span></span>

* <span data-ttu-id="14cc9-2868">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2868">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="14cc9-2869">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2869">Added `sql db rename`</span></span>
* <span data-ttu-id="14cc9-2870">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="14cc9-2870">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2871">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2871">Storage</span></span>

* <span data-ttu-id="14cc9-2872">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="14cc9-2872">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2873">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2873">VM</span></span>

* <span data-ttu-id="14cc9-2874">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2874">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="14cc9-2875">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2875">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="14cc9-2876">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="14cc9-2876">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="14cc9-2877">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2877">January 31, 2018</span></span>

<span data-ttu-id="14cc9-2878">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="14cc9-2878">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-2879">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-2879">Core</span></span>

* <span data-ttu-id="14cc9-2880">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2880">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="14cc9-2881">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-2881">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="14cc9-2882">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2882">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="14cc9-2883">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="14cc9-2883">Use `--verbose` to see</span></span>
* <span data-ttu-id="14cc9-2884">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="14cc9-2884">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2885">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2885">ACS</span></span>

* <span data-ttu-id="14cc9-2886">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2886">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="14cc9-2887">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2887">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2888">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2888">Appservice</span></span>

* <span data-ttu-id="14cc9-2889">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="14cc9-2889">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="14cc9-2890">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="14cc9-2890">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-2891">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-2891">CDN</span></span>

* <span data-ttu-id="14cc9-2892">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2892">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-2893">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-2893">CosmosDB</span></span>

* <span data-ttu-id="14cc9-2894">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2894">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2895">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2895">Interactive</span></span>

* <span data-ttu-id="14cc9-2896">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="14cc9-2896">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2897">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2897">Network</span></span>

* <span data-ttu-id="14cc9-2898">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2898">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="14cc9-2899">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2899">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="14cc9-2900">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2900">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="14cc9-2901">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2901">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="14cc9-2902">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2902">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="14cc9-2903">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="14cc9-2903">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="14cc9-2904">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2904">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="14cc9-2905">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2905">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="14cc9-2906">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2906">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="14cc9-2907">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2907">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-2908">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2908">Profile</span></span>

* <span data-ttu-id="14cc9-2909">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="14cc9-2909">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-2910">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-2910">Resource</span></span>

* <span data-ttu-id="14cc9-2911">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="14cc9-2911">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2912">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2912">Storage</span></span>

* <span data-ttu-id="14cc9-2913">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="14cc9-2913">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="14cc9-2914">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="14cc9-2914">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="14cc9-2915">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2915">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="14cc9-2916">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2916">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="14cc9-2917">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="14cc9-2917">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2918">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2918">VM</span></span>

* <span data-ttu-id="14cc9-2919">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="14cc9-2919">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="14cc9-2920">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="14cc9-2920">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="14cc9-2921">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="14cc9-2921">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="14cc9-2922">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2922">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="14cc9-2923">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="14cc9-2923">January 17, 2018</span></span>

<span data-ttu-id="14cc9-2924">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="14cc9-2924">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-2925">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-2925">ACR</span></span>

* <span data-ttu-id="14cc9-2926">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-2926">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="14cc9-2927">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="14cc9-2927">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-2928">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2928">ACS</span></span>

* <span data-ttu-id="14cc9-2929">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2929">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="14cc9-2930">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="14cc9-2930">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-2931">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-2931">Appservice</span></span>

* <span data-ttu-id="14cc9-2932">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="14cc9-2932">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="14cc9-2933">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2933">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="14cc9-2934">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2934">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-2935">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-2935">Backup</span></span>

* <span data-ttu-id="14cc9-2936">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="14cc9-2936">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="14cc9-2937">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2937">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="14cc9-2938">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-2938">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="14cc9-2939">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="14cc9-2939">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="14cc9-2940">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-2940">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-2941">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-2941">Batch</span></span>

* <span data-ttu-id="14cc9-2942">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="14cc9-2942">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="14cc9-2943">Cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-2943">Cloud</span></span>

* <span data-ttu-id="14cc9-2944">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-2944">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-2945">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2945">Consumption</span></span>

* <span data-ttu-id="14cc9-2946">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2946">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="14cc9-2947">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14cc9-2947">Event Grid</span></span>

* <span data-ttu-id="14cc9-2948">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2948">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="14cc9-2949">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2949">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="14cc9-2950">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2950">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="14cc9-2951">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="14cc9-2951">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="14cc9-2952">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2952">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="14cc9-2953">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2953">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="14cc9-2954">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2954">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="14cc9-2955">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2955">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-2956">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-2956">Interactive</span></span>

* <span data-ttu-id="14cc9-2957">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="14cc9-2957">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="14cc9-2958">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2958">Fixed errors on startup</span></span>
* <span data-ttu-id="14cc9-2959">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="14cc9-2959">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-2960">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2960">IoT</span></span>

* <span data-ttu-id="14cc9-2961">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="14cc9-2961">Added support for device provisioning service</span></span>
* <span data-ttu-id="14cc9-2962">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2962">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="14cc9-2963">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-2963">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-2964">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-2964">Monitor</span></span>

* <span data-ttu-id="14cc9-2965">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="14cc9-2965">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="14cc9-2966">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2966">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="14cc9-2967">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="14cc9-2967">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2968">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2968">Network</span></span>

* <span data-ttu-id="14cc9-2969">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2969">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="14cc9-2970">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2970">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-2971">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-2971">Profile</span></span>

* <span data-ttu-id="14cc9-2972">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2972">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-2973">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-2973">Role</span></span>

* <span data-ttu-id="14cc9-2974">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="14cc9-2974">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14cc9-2975">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-2975">Service Fabric</span></span>

* <span data-ttu-id="14cc9-2976">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="14cc9-2976">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="14cc9-2977">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-2977">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2978">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2978">VM</span></span>

* <span data-ttu-id="14cc9-2979">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2979">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="14cc9-2980">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="14cc9-2980">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="14cc9-2981">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="14cc9-2981">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="14cc9-2982">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="14cc9-2982">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="14cc9-2983">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="14cc9-2983">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="14cc9-2984">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2984">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="14cc9-2985">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2985">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="14cc9-2986">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2986">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="14cc9-2987">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-2987">December 19, 2017</span></span>

<span data-ttu-id="14cc9-2988">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="14cc9-2988">Version 2.0.23</span></span>

* <span data-ttu-id="14cc9-2989">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-2989">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-2990">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2990">Container</span></span>

* <span data-ttu-id="14cc9-2991">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-2991">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-2992">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-2992">Network</span></span>

* <span data-ttu-id="14cc9-2993">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2993">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="14cc9-2994">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-2994">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-2995">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-2995">Storage</span></span>

* <span data-ttu-id="14cc9-2996">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="14cc9-2996">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-2997">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-2997">VM</span></span>

* <span data-ttu-id="14cc9-2998">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="14cc9-2998">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="14cc9-2999">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-2999">December 5, 2017</span></span>

<span data-ttu-id="14cc9-3000">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="14cc9-3000">Version 2.0.22</span></span>

* <span data-ttu-id="14cc9-3001">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3001">Removed `az component` commands.</span></span> <span data-ttu-id="14cc9-3002">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="14cc9-3002">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-3003">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3003">Core</span></span>
* <span data-ttu-id="14cc9-3004">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="14cc9-3004">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="14cc9-3005">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="14cc9-3005">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3006">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3006">ACS</span></span>

* <span data-ttu-id="14cc9-3007">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3007">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="14cc9-3008">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3008">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="14cc9-3009">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="14cc9-3009">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="14cc9-3010">Advisor</span><span class="sxs-lookup"><span data-stu-id="14cc9-3010">Advisor</span></span>

* <span data-ttu-id="14cc9-3011">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-3011">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3012">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3012">Appservice</span></span>

* <span data-ttu-id="14cc9-3013">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3013">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="14cc9-3014">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3014">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="14cc9-3015">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3015">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="14cc9-3016">Consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-3016">Consumption</span></span>

* <span data-ttu-id="14cc9-3017">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="14cc9-3017">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-3018">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3018">Container</span></span>

* <span data-ttu-id="14cc9-3019">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3019">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-3020">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-3020">Monitor</span></span>

* <span data-ttu-id="14cc9-3021">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="14cc9-3021">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3022">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3022">Resource</span></span>

* <span data-ttu-id="14cc9-3023">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3023">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-3024">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-3024">Role</span></span>

* <span data-ttu-id="14cc9-3025">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3025">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="14cc9-3026">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3026">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="14cc9-3027">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3027">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3028">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3028">SQL</span></span>

* <span data-ttu-id="14cc9-3029">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3029">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="14cc9-3030">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3030">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3031">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3031">VM</span></span>

* <span data-ttu-id="14cc9-3032">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3032">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="14cc9-3033">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3033">November 14, 2017</span></span>

<span data-ttu-id="14cc9-3034">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="14cc9-3034">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-3035">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-3035">ACR</span></span>

* <span data-ttu-id="14cc9-3036">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="14cc9-3036">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="14cc9-3037">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3037">ACS</span></span>

* <span data-ttu-id="14cc9-3038">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3038">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="14cc9-3039">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3039">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="14cc9-3040">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3040">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="14cc9-3041">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-3041">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="14cc9-3042">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14cc9-3042">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3043">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3043">Appservice</span></span>

* <span data-ttu-id="14cc9-3044">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="14cc9-3044">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="14cc9-3045">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3045">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="14cc9-3046">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3046">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="14cc9-3047">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3047">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="14cc9-3048">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="14cc9-3048">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="14cc9-3049">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3049">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-3050">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-3050">Batch</span></span>

* <span data-ttu-id="14cc9-3051">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3051">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-3052">Batchai</span><span class="sxs-lookup"><span data-stu-id="14cc9-3052">Batchai</span></span>

* <span data-ttu-id="14cc9-3053">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3053">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="14cc9-3054">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3054">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="14cc9-3055">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3055">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="14cc9-3056">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3056">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="14cc9-3057">Cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-3057">Cloud</span></span>

* <span data-ttu-id="14cc9-3058">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="14cc9-3058">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-3059">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3059">Container</span></span>

* <span data-ttu-id="14cc9-3060">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="14cc9-3060">Added support to open multiple ports</span></span>
* <span data-ttu-id="14cc9-3061">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14cc9-3061">Added container group restart policy</span></span>
* <span data-ttu-id="14cc9-3062">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="14cc9-3062">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="14cc9-3063">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="14cc9-3063">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14cc9-3064">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-3064">Data Lake Analytics</span></span>

* <span data-ttu-id="14cc9-3065">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="14cc9-3065">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14cc9-3066">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3066">Data Lake Store</span></span>

* <span data-ttu-id="14cc9-3067">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="14cc9-3067">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-3068">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-3068">Extension</span></span>

* <span data-ttu-id="14cc9-3069">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="14cc9-3069">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="14cc9-3070">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="14cc9-3070">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-3071">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-3071">IoT</span></span>

* <span data-ttu-id="14cc9-3072">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="14cc9-3072">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-3073">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-3073">Monitor</span></span>

* <span data-ttu-id="14cc9-3074">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3074">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3075">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3075">Network</span></span>

* <span data-ttu-id="14cc9-3076">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="14cc9-3076">Added support for CAA DNS records</span></span>
* <span data-ttu-id="14cc9-3077">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3077">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="14cc9-3078">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-3078">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="14cc9-3079">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3079">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="14cc9-3080">Réservations</span><span class="sxs-lookup"><span data-stu-id="14cc9-3080">Reservations</span></span>

* <span data-ttu-id="14cc9-3081">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-3081">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3082">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3082">Resource</span></span>

* <span data-ttu-id="14cc9-3083">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-3083">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3084">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3084">SQL</span></span>

* <span data-ttu-id="14cc9-3085">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3085">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3086">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3086">Storage</span></span>

* <span data-ttu-id="14cc9-3087">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3087">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="14cc9-3088">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="14cc9-3088">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="14cc9-3089">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3089">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="14cc9-3090">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3090">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="14cc9-3091">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3091">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="14cc9-3092">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3092">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="14cc9-3093">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3093">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3094">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3094">VM</span></span>

* <span data-ttu-id="14cc9-3095">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3095">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="14cc9-3096">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="14cc9-3096">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="14cc9-3097">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="14cc9-3097">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="14cc9-3098">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3098">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="14cc9-3099">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3099">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="14cc9-3100">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3100">October 24, 2017</span></span>

<span data-ttu-id="14cc9-3101">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="14cc9-3101">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-3102">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3102">Core</span></span>

* <span data-ttu-id="14cc9-3103">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3103">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-3104">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-3104">ACR</span></span>

* <span data-ttu-id="14cc9-3105">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3105">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="14cc9-3106">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="14cc9-3106">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="14cc9-3107">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="14cc9-3107">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3108">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3108">ACS</span></span>

* <span data-ttu-id="14cc9-3109">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3109">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="14cc9-3110">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3110">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3111">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3111">Appservice</span></span>

* <span data-ttu-id="14cc9-3112">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="14cc9-3112">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="14cc9-3113">Composant</span><span class="sxs-lookup"><span data-stu-id="14cc9-3113">Component</span></span>

* <span data-ttu-id="14cc9-3114">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="14cc9-3114">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-3115">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-3115">Monitor</span></span>

* <span data-ttu-id="14cc9-3116">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3116">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3117">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3117">Resource</span></span>

* <span data-ttu-id="14cc9-3118">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3118">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="14cc9-3119">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="14cc9-3119">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3120">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3120">VM</span></span>

* <span data-ttu-id="14cc9-3121">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3121">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="14cc9-3122">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3122">October 9, 2017</span></span>

<span data-ttu-id="14cc9-3123">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="14cc9-3123">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-3124">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3124">Core</span></span>

* <span data-ttu-id="14cc9-3125">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14cc9-3125">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3126">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3126">Appservice</span></span>

* <span data-ttu-id="14cc9-3127">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3127">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-3128">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-3128">Batch</span></span>

* <span data-ttu-id="14cc9-3129">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-3129">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="14cc9-3130">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="14cc9-3130">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="14cc9-3131">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-3131">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="14cc9-3132">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="14cc9-3132">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="14cc9-3133">Batchai</span><span class="sxs-lookup"><span data-stu-id="14cc9-3133">Batchai</span></span>

* <span data-ttu-id="14cc9-3134">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="14cc9-3134">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-3135">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-3135">Keyvault</span></span>

* <span data-ttu-id="14cc9-3136">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3136">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="14cc9-3137">(#4448)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3137">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="14cc9-3138">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3138">Network</span></span>

* <span data-ttu-id="14cc9-3139">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="14cc9-3139">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="14cc9-3140">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3140">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3141">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3141">Resource</span></span>

* <span data-ttu-id="14cc9-3142">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3142">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="14cc9-3143">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3143">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="14cc9-3144">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3144">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="14cc9-3145">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-3145">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3146">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3146">Sql</span></span>

* <span data-ttu-id="14cc9-3147">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="14cc9-3147">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="14cc9-3148">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="14cc9-3148">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="14cc9-3149">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="14cc9-3149">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3150">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3150">Storage</span></span>

* <span data-ttu-id="14cc9-3151">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="14cc9-3151">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3152">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3152">Vm</span></span>

* <span data-ttu-id="14cc9-3153">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3153">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="14cc9-3154">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3154">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="14cc9-3155">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3155">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="14cc9-3156">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3156">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="14cc9-3157">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3157">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="14cc9-3158">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3158">September 22, 2017</span></span>

<span data-ttu-id="14cc9-3159">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="14cc9-3159">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3160">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3160">Resource</span></span>

* <span data-ttu-id="14cc9-3161">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3161">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="14cc9-3162">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="14cc9-3162">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="14cc9-3163">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3163">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="14cc9-3164">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3164">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3165">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3165">Network</span></span>

* <span data-ttu-id="14cc9-3166">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3166">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="14cc9-3167">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3167">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="14cc9-3168">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3168">Added `asg` application security group commands</span></span>
* <span data-ttu-id="14cc9-3169">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3169">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="14cc9-3170">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3170">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="14cc9-3171">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3171">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="14cc9-3172">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3172">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3173">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3173">Storage</span></span>

* <span data-ttu-id="14cc9-3174">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3174">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="14cc9-3175">Événement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3175">Eventgrid</span></span>

* <span data-ttu-id="14cc9-3176">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="14cc9-3176">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3177">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3177">SQL</span></span>

* <span data-ttu-id="14cc9-3178">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3178">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="14cc9-3179">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3179">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="14cc9-3180">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3180">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-3181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-3181">Keyvault</span></span>

* <span data-ttu-id="14cc9-3182">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="14cc9-3182">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3183">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3183">VM</span></span>

* <span data-ttu-id="14cc9-3184">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3184">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="14cc9-3185">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="14cc9-3185">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="14cc9-3186">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3186">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="14cc9-3187">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3187">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="14cc9-3188">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3188">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="14cc9-3189">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3189">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3190">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3190">ACS</span></span>

* <span data-ttu-id="14cc9-3191">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-3191">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3192">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3192">Appservice</span></span>

* <span data-ttu-id="14cc9-3193">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3193">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="14cc9-3194">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14cc9-3194">Backup</span></span>

* <span data-ttu-id="14cc9-3195">Préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-3195">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="14cc9-3196">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3196">September 11, 2017</span></span>

<span data-ttu-id="14cc9-3197">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="14cc9-3197">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="14cc9-3198">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3198">Core</span></span>

* <span data-ttu-id="14cc9-3199">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="14cc9-3199">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="14cc9-3200">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="14cc9-3200">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3201">Acs</span><span class="sxs-lookup"><span data-stu-id="14cc9-3201">Acs</span></span>

* <span data-ttu-id="14cc9-3202">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3202">Added `acs list-locations` command</span></span>
* <span data-ttu-id="14cc9-3203">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="14cc9-3203">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3204">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3204">Appservice</span></span>

* <span data-ttu-id="14cc9-3205">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="14cc9-3205">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-3206">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-3206">CDN</span></span>

* <span data-ttu-id="14cc9-3207">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3207">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="14cc9-3208">Extension</span><span class="sxs-lookup"><span data-stu-id="14cc9-3208">Extension</span></span>

* <span data-ttu-id="14cc9-3209">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-3209">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-3210">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-3210">Keyvault</span></span>

* <span data-ttu-id="14cc9-3211">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3211">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3212">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3212">Network</span></span>

* <span data-ttu-id="14cc9-3213">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3213">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="14cc9-3214">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3214">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="14cc9-3215">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3215">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="14cc9-3216">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3216">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="14cc9-3217">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3217">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3218">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3218">Resource</span></span>

* <span data-ttu-id="14cc9-3219">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3219">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="14cc9-3220">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3220">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="14cc9-3221">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="14cc9-3221">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="14cc9-3222">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="14cc9-3222">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3223">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3223">SQL</span></span>

* <span data-ttu-id="14cc9-3224">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3224">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3225">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3225">VM</span></span>

* <span data-ttu-id="14cc9-3226">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="14cc9-3226">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="14cc9-3227">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="14cc9-3227">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="14cc9-3228">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3228">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="14cc9-3229">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="14cc9-3229">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="14cc9-3230">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="14cc9-3230">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="14cc9-3231">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3231">August 31, 2017</span></span>

<span data-ttu-id="14cc9-3232">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="14cc9-3232">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-3233">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-3233">Keyvault</span></span>

* <span data-ttu-id="14cc9-3234">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3234">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="14cc9-3235">Sf</span><span class="sxs-lookup"><span data-stu-id="14cc9-3235">Sf</span></span>

* <span data-ttu-id="14cc9-3236">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3236">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3237">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3237">Storage</span></span>

* <span data-ttu-id="14cc9-3238">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="14cc9-3238">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="14cc9-3239">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3239">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="14cc9-3240">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3240">August 28, 2017</span></span>

<span data-ttu-id="14cc9-3241">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="14cc9-3241">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="14cc9-3242">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-3242">CLI</span></span>

* <span data-ttu-id="14cc9-3243">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3243">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3244">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3244">ACS</span></span>

* <span data-ttu-id="14cc9-3245">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="14cc9-3245">Corrected preview regions</span></span>
* <span data-ttu-id="14cc9-3246">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3246">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="14cc9-3247">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3247">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3248">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3248">Appservice</span></span>

* <span data-ttu-id="14cc9-3249">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3249">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="14cc9-3250">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3250">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="14cc9-3251">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3251">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="14cc9-3252">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3252">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="14cc9-3253">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3253">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-3254">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-3254">IoT</span></span>

* <span data-ttu-id="14cc9-3255">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3255">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3256">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3256">Network</span></span>

* <span data-ttu-id="14cc9-3257">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3257">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="14cc9-3258">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3258">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="14cc9-3259">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3259">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="14cc9-3260">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3260">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="14cc9-3261">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3261">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-3262">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-3262">Profile</span></span>

* <span data-ttu-id="14cc9-3263">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3263">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14cc9-3264">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-3264">Service Fabric</span></span>

* <span data-ttu-id="14cc9-3265">Préversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-3265">Preview release</span></span>
* <span data-ttu-id="14cc9-3266">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-3266">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="14cc9-3267">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="14cc9-3267">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="14cc9-3268">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3268">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3269">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3269">Storage</span></span>

* <span data-ttu-id="14cc9-3270">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="14cc9-3270">Enabled setting blob tier</span></span>
* <span data-ttu-id="14cc9-3271">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="14cc9-3271">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="14cc9-3272">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3272">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="14cc9-3273">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="14cc9-3273">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="14cc9-3274">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3274">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="14cc9-3275">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3275">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3276">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3276">VM</span></span>

* <span data-ttu-id="14cc9-3277">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3277">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="14cc9-3278">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="14cc9-3278">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="14cc9-3279">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3279">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="14cc9-3280">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="14cc9-3280">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="14cc9-3281">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="14cc9-3281">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="14cc9-3282">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3282">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="14cc9-3283">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3283">August 15, 2017</span></span>

<span data-ttu-id="14cc9-3284">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="14cc9-3284">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3285">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3285">ACS</span></span>

* <span data-ttu-id="14cc9-3286">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3286">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3287">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3287">Appservice</span></span>

* <span data-ttu-id="14cc9-3288">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="14cc9-3288">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="14cc9-3289">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14cc9-3289">Event Grid</span></span>

* <span data-ttu-id="14cc9-3290">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3290">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="14cc9-3291">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3291">August 11, 2017</span></span>

<span data-ttu-id="14cc9-3292">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="14cc9-3292">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3293">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3293">ACS</span></span>

* <span data-ttu-id="14cc9-3294">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="14cc9-3294">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-3295">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-3295">Batch</span></span>

* <span data-ttu-id="14cc9-3296">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-3296">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="14cc9-3297">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-3297">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="14cc9-3298">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="14cc9-3298">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="14cc9-3299">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="14cc9-3299">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="14cc9-3300">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-3300">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="14cc9-3301">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="14cc9-3301">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="14cc9-3302">Composant</span><span class="sxs-lookup"><span data-stu-id="14cc9-3302">Component</span></span>

* <span data-ttu-id="14cc9-3303">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="14cc9-3303">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="14cc9-3304">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3304">Container</span></span>

* <span data-ttu-id="14cc9-3305">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3305">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="14cc9-3306">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3306">Data Lake Store</span></span>

* <span data-ttu-id="14cc9-3307">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="14cc9-3307">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="14cc9-3308">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14cc9-3308">Event Grid</span></span>

* <span data-ttu-id="14cc9-3309">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14cc9-3309">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3310">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3310">Network</span></span>

* <span data-ttu-id="14cc9-3311">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="14cc9-3311">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="14cc9-3312">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3312">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="14cc9-3313">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3313">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="14cc9-3314">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3314">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-3315">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-3315">Profile</span></span>

* <span data-ttu-id="14cc9-3316">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3316">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3317">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3317">Storage</span></span>

* <span data-ttu-id="14cc9-3318">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="14cc9-3318">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3319">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3319">VM</span></span>

* <span data-ttu-id="14cc9-3320">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="14cc9-3320">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="14cc9-3321">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3321">Exposed `list-skus` command</span></span>
* <span data-ttu-id="14cc9-3322">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3322">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="14cc9-3323">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="14cc9-3323">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="14cc9-3324">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3324">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="14cc9-3325">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3325">July 28, 2017</span></span>

<span data-ttu-id="14cc9-3326">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="14cc9-3326">Version 2.0.12</span></span>

* <span data-ttu-id="14cc9-3327">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3327">Added container commands</span></span>
* <span data-ttu-id="14cc9-3328">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="14cc9-3328">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="14cc9-3329">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3329">Core</span></span>

* <span data-ttu-id="14cc9-3330">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="14cc9-3330">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="14cc9-3331">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3331">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="14cc9-3332">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3332">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="14cc9-3333">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3333">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="14cc9-3334">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="14cc9-3334">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="14cc9-3335">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3335">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="14cc9-3336">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3336">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="14cc9-3337">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3337">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="14cc9-3338">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3338">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="14cc9-3339">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3339">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="14cc9-3340">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="14cc9-3340">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="14cc9-3341">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3341">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="14cc9-3342">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-3342">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="14cc9-3343">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="14cc9-3343">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="14cc9-3344">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14cc9-3344">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="14cc9-3345">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3345">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="14cc9-3346">ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-3346">ACR</span></span>

* <span data-ttu-id="14cc9-3347">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3347">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="14cc9-3348">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3348">Support SKU update for managed registries</span></span>
* <span data-ttu-id="14cc9-3349">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3349">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="14cc9-3350">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="14cc9-3350">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="14cc9-3351">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="14cc9-3351">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="14cc9-3352">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="14cc9-3352">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3353">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3353">ACS</span></span>

* <span data-ttu-id="14cc9-3354">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="14cc9-3354">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3355">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3355">Appservice</span></span>

* <span data-ttu-id="14cc9-3356">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="14cc9-3356">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="14cc9-3357">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="14cc9-3357">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="14cc9-3358">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3358">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="14cc9-3359">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3359">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="14cc9-3360">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3360">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="14cc9-3361">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3361">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="14cc9-3362">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3362">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="14cc9-3363">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3363">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="14cc9-3364">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3364">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="14cc9-3365">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3365">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="14cc9-3366">Batch</span><span class="sxs-lookup"><span data-stu-id="14cc9-3366">Batch</span></span>

* <span data-ttu-id="14cc9-3367">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="14cc9-3367">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="14cc9-3368">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3368">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="14cc9-3369">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3369">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="14cc9-3370">CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-3370">CDN</span></span>

* <span data-ttu-id="14cc9-3371">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-3371">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="14cc9-3372">Cloud</span><span class="sxs-lookup"><span data-stu-id="14cc9-3372">Cloud</span></span>

* <span data-ttu-id="14cc9-3373">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="14cc9-3373">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="14cc9-3374">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3374">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="14cc9-3375">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="14cc9-3375">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="14cc9-3376">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="14cc9-3376">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="14cc9-3377">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3377">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-3378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-3378">CosmosDB</span></span>

* <span data-ttu-id="14cc9-3379">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3379">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="14cc9-3380">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="14cc9-3380">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14cc9-3381">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-3381">Data Lake Analytics</span></span>

* <span data-ttu-id="14cc9-3382">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3382">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="14cc9-3383">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3383">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="14cc9-3384">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3384">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14cc9-3385">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3385">Data Lake Store</span></span>

* <span data-ttu-id="14cc9-3386">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3386">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="14cc9-3387">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="14cc9-3387">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="14cc9-3388">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3388">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="14cc9-3389">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3389">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="14cc9-3390">Interactive</span><span class="sxs-lookup"><span data-stu-id="14cc9-3390">Interactive</span></span>

* <span data-ttu-id="14cc9-3391">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="14cc9-3391">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="14cc9-3392">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="14cc9-3392">Increased test coverage</span></span>
* <span data-ttu-id="14cc9-3393">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="14cc9-3393">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="14cc9-3394">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3394">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="14cc9-3395">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3395">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="14cc9-3396">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3396">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="14cc9-3397">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3397">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="14cc9-3398">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3398">Added `--progress` flag</span></span>
* <span data-ttu-id="14cc9-3399">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="14cc9-3399">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="14cc9-3400">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3400">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="14cc9-3401">IoT</span><span class="sxs-lookup"><span data-stu-id="14cc9-3401">IoT</span></span>

* <span data-ttu-id="14cc9-3402">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3402">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="14cc9-3403">(#3934)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3403">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="14cc9-3404">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3404">Key vault</span></span>

* <span data-ttu-id="14cc9-3405">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="14cc9-3405">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="14cc9-3406">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3406">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="14cc9-3407">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3407">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="14cc9-3408">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3408">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="14cc9-3409">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3409">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="14cc9-3410">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3410">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="14cc9-3411">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3411">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="14cc9-3412">(#3307)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3412">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="14cc9-3413">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3413">Lab</span></span>

* <span data-ttu-id="14cc9-3414">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3414">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="14cc9-3415">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3415">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-3416">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-3416">Monitor</span></span>

* <span data-ttu-id="14cc9-3417">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3417">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="14cc9-3418">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3418">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="14cc9-3419">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3419">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="14cc9-3420">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3420">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="14cc9-3421">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3421">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="14cc9-3422">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="14cc9-3422">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="14cc9-3423">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="14cc9-3423">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="14cc9-3424">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3424">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="14cc9-3425">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3425">`location` no longer required</span></span>
  * <span data-ttu-id="14cc9-3426">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="14cc9-3426">Add name and ID support for target</span></span>
  * <span data-ttu-id="14cc9-3427">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3427">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="14cc9-3428">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3428">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="14cc9-3429">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="14cc9-3429">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="14cc9-3430">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="14cc9-3430">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="14cc9-3431">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3431">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="14cc9-3432">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3432">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3433">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3433">Network</span></span>

* <span data-ttu-id="14cc9-3434">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3434">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="14cc9-3435">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3435">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="14cc9-3436">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="14cc9-3436">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="14cc9-3437">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="14cc9-3437">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="14cc9-3438">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3438">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="14cc9-3439">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3439">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="14cc9-3440">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3440">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="14cc9-3441">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3441">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="14cc9-3442">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3442">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="14cc9-3443">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3443">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="14cc9-3444">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3444">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="14cc9-3445">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3445">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="14cc9-3446">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3446">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="14cc9-3447">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3447">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="14cc9-3448">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3448">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="14cc9-3449">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3449">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="14cc9-3450">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="14cc9-3450">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="14cc9-3451">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3451">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="14cc9-3452">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3452">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="14cc9-3453">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3453">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="14cc9-3454">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3454">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="14cc9-3455">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3455">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="14cc9-3456">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3456">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="14cc9-3457">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14cc9-3457">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="14cc9-3458">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14cc9-3458">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="14cc9-3459">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14cc9-3459">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="14cc9-3460">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14cc9-3460">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-3461">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-3461">Profile</span></span>

* <span data-ttu-id="14cc9-3462">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3462">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="14cc9-3463">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3463">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="14cc9-3464">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="14cc9-3464">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="14cc9-3465">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3465">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="14cc9-3466">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="14cc9-3466">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="14cc9-3467">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14cc9-3467">RDBMS</span></span>

* <span data-ttu-id="14cc9-3468">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3468">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="14cc9-3469">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3469">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="14cc9-3470">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3470">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="14cc9-3471">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3471">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3472">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3472">Resource</span></span>

* <span data-ttu-id="14cc9-3473">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3473">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="14cc9-3474">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3474">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="14cc9-3475">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3475">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="14cc9-3476">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="14cc9-3476">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="14cc9-3477">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3477">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="14cc9-3478">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3478">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="14cc9-3479">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3479">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="14cc9-3480">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14cc9-3480">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-3481">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-3481">Role</span></span>

* <span data-ttu-id="14cc9-3482">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3482">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="14cc9-3483">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3483">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="14cc9-3484">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="14cc9-3484">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="14cc9-3485">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3485">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="14cc9-3486">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3486">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14cc9-3487">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-3487">Service Fabric</span></span>
* <span data-ttu-id="14cc9-3488">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3488">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="14cc9-3489">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3489">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="14cc9-3490">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3490">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3491">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3491">SQL</span></span>

* <span data-ttu-id="14cc9-3492">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="14cc9-3492">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="14cc9-3493">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3493">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="14cc9-3494">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3494">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3495">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3495">Storage</span></span>

* <span data-ttu-id="14cc9-3496">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3496">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="14cc9-3497">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="14cc9-3497">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="14cc9-3498">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3498">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="14cc9-3499">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3499">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="14cc9-3500">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3500">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="14cc9-3501">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3501">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3502">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3502">VM</span></span>

* <span data-ttu-id="14cc9-3503">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3503">Support configuring nsg</span></span>
* <span data-ttu-id="14cc9-3504">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3504">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="14cc9-3505">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="14cc9-3505">Support managed service identities</span></span>
* <span data-ttu-id="14cc9-3506">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3506">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="14cc9-3507">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="14cc9-3507">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="14cc9-3508">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3508">May 10, 2017</span></span>

<span data-ttu-id="14cc9-3509">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="14cc9-3509">Version 2.0.6</span></span>

* <span data-ttu-id="14cc9-3510">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="14cc9-3510">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="14cc9-3511">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3511">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="14cc9-3512">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3512">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="14cc9-3513">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14cc9-3513">Include Cognitive Services module</span></span>
* <span data-ttu-id="14cc9-3514">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14cc9-3514">Include Service Fabric module</span></span>
* <span data-ttu-id="14cc9-3515">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3515">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="14cc9-3516">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="14cc9-3516">Add support for CDN commands</span></span>
* <span data-ttu-id="14cc9-3517">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="14cc9-3517">Remove Container module</span></span>
* <span data-ttu-id="14cc9-3518">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3518">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="14cc9-3519">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3519">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="14cc9-3520">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3520">Core</span></span>

* <span data-ttu-id="14cc9-3521">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3521">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="14cc9-3522">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3522">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="14cc9-3523">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3523">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="14cc9-3524">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3524">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="14cc9-3525">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3525">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="14cc9-3526">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3526">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="14cc9-3527">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3527">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="14cc9-3528">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3528">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="14cc9-3529">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3529">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="14cc9-3530">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="14cc9-3530">core: Improved performance</span></span>
* <span data-ttu-id="14cc9-3531">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="14cc9-3531">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="14cc9-3532">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="14cc9-3532">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3533">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3533">ACS</span></span>

* <span data-ttu-id="14cc9-3534">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="14cc9-3534">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="14cc9-3535">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="14cc9-3535">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="14cc9-3536">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="14cc9-3536">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="14cc9-3537">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3537">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3538">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3538">AppService</span></span>

* <span data-ttu-id="14cc9-3539">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3539">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="14cc9-3540">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="14cc9-3540">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="14cc9-3541">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3541">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="14cc9-3542">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="14cc9-3542">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="14cc9-3543">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="14cc9-3543">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="14cc9-3544">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3544">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="14cc9-3545">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="14cc9-3545">support slot swap with preview</span></span>
* <span data-ttu-id="14cc9-3546">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3546">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="14cc9-3547">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3547">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14cc9-3548">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-3548">CosmosDB</span></span>

* <span data-ttu-id="14cc9-3549">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="14cc9-3549">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="14cc9-3550">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="14cc9-3550">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="14cc9-3551">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="14cc9-3551">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="14cc9-3552">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="14cc9-3552">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14cc9-3553">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-3553">Data Lake Analytics</span></span>

* <span data-ttu-id="14cc9-3554">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3554">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="14cc9-3555">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3555">Add support for new catalog item type: package.</span></span> <span data-ttu-id="14cc9-3556">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3556">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="14cc9-3557">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="14cc9-3557">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="14cc9-3558">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="14cc9-3558">Table</span></span>
  * <span data-ttu-id="14cc9-3559">Fonction table</span><span class="sxs-lookup"><span data-stu-id="14cc9-3559">Table valued function</span></span>
  * <span data-ttu-id="14cc9-3560">Affichage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3560">View</span></span>
  * <span data-ttu-id="14cc9-3561">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3561">Table Statistics.</span></span> <span data-ttu-id="14cc9-3562">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="14cc9-3562">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14cc9-3563">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3563">Data Lake Store</span></span>

* <span data-ttu-id="14cc9-3564">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="14cc9-3564">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="14cc9-3565">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3565">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="14cc9-3566">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3566">missed help for access show.</span></span> <span data-ttu-id="14cc9-3567">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3567">adding it.</span></span> <span data-ttu-id="14cc9-3568">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3568">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="14cc9-3569">Rechercher</span><span class="sxs-lookup"><span data-stu-id="14cc9-3569">Find</span></span>

* <span data-ttu-id="14cc9-3570">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="14cc9-3570">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="14cc9-3571">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14cc9-3571">KeyVault</span></span>

* <span data-ttu-id="14cc9-3572">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="14cc9-3572">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="14cc9-3573">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="14cc9-3573">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="14cc9-3574">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="14cc9-3574">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="14cc9-3575">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-3575">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="14cc9-3576">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3576">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="14cc9-3577">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3577">Lab</span></span>

* <span data-ttu-id="14cc9-3578">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3578">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="14cc9-3579">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3579">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="14cc9-3580">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3580">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="14cc9-3581">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3581">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="14cc9-3582">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="14cc9-3582">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="14cc9-3583">Superviser</span><span class="sxs-lookup"><span data-stu-id="14cc9-3583">Monitor</span></span>

* <span data-ttu-id="14cc9-3584">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3584">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="14cc9-3585">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3585">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="14cc9-3586">Réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3586">Network</span></span>

* <span data-ttu-id="14cc9-3587">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3587">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="14cc9-3588">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3588">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="14cc9-3589">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="14cc9-3589">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="14cc9-3590">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="14cc9-3590">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="14cc9-3591">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="14cc9-3591">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="14cc9-3592">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="14cc9-3592">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="14cc9-3593">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="14cc9-3593">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="14cc9-3594">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="14cc9-3594">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="14cc9-3595">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3595">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="14cc9-3596">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="14cc9-3596">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="14cc9-3597">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3597">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="14cc9-3598">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3598">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="14cc9-3599">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3599">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="14cc9-3600">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="14cc9-3600">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="14cc9-3601">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="14cc9-3601">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="14cc9-3602">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="14cc9-3602">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="14cc9-3603">Profil</span><span class="sxs-lookup"><span data-stu-id="14cc9-3603">Profile</span></span>

* <span data-ttu-id="14cc9-3604">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3604">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="14cc9-3605">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3605">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="14cc9-3606">Redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-3606">Redis</span></span>

* <span data-ttu-id="14cc9-3607">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="14cc9-3607">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="14cc9-3608">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="14cc9-3608">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="14cc9-3609">Ressource</span><span class="sxs-lookup"><span data-stu-id="14cc9-3609">Resource</span></span>

* <span data-ttu-id="14cc9-3610">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3610">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="14cc9-3611">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3611">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="14cc9-3612">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3612">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="14cc9-3613">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3613">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="14cc9-3614">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3614">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="14cc9-3615">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3615">Add docs for az lock update.</span></span> <span data-ttu-id="14cc9-3616">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3616">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="14cc9-3617">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3617">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="14cc9-3618">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3618">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="14cc9-3619">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3619">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="14cc9-3620">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3620">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="14cc9-3621">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3621">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="14cc9-3622">Role</span><span class="sxs-lookup"><span data-stu-id="14cc9-3622">Role</span></span>

* <span data-ttu-id="14cc9-3623">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3623">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="14cc9-3624">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3624">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="14cc9-3625">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3625">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="14cc9-3626">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="14cc9-3626">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="14cc9-3627">SQL</span><span class="sxs-lookup"><span data-stu-id="14cc9-3627">SQL</span></span>

* <span data-ttu-id="14cc9-3628">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="14cc9-3628">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="14cc9-3629">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3629">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="14cc9-3630">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3630">Storage</span></span>

* <span data-ttu-id="14cc9-3631">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="14cc9-3631">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="14cc9-3632">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="14cc9-3632">Add support for incremental blob copy</span></span>
* <span data-ttu-id="14cc9-3633">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="14cc9-3633">Add support for large block blob upload</span></span>
* <span data-ttu-id="14cc9-3634">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="14cc9-3634">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3635">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3635">VM</span></span>

* <span data-ttu-id="14cc9-3636">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="14cc9-3636">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="14cc9-3637">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="14cc9-3637">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="14cc9-3638">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="14cc9-3638">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="14cc9-3639">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="14cc9-3639">az vm/vmss disk</span></span>
  3. <span data-ttu-id="14cc9-3640">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="14cc9-3640">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="14cc9-3641">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="14cc9-3641">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="14cc9-3642">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3642">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="14cc9-3643">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3643">April 3, 2017</span></span>

<span data-ttu-id="14cc9-3644">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="14cc9-3644">Version 2.0.2</span></span>

<span data-ttu-id="14cc9-3645">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="14cc9-3645">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="14cc9-3646">Core</span><span class="sxs-lookup"><span data-stu-id="14cc9-3646">Core</span></span>

* <span data-ttu-id="14cc9-3647">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3647">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="14cc9-3648">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3648">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="14cc9-3649">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3649">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="14cc9-3650">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3650">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="14cc9-3651">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3651">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="14cc9-3652">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3652">Add prompting for missing template parameters.</span></span> <span data-ttu-id="14cc9-3653">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3653">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="14cc9-3654">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="14cc9-3654">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="14cc9-3655">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="14cc9-3655">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="14cc9-3656">ACS</span><span class="sxs-lookup"><span data-stu-id="14cc9-3656">ACS</span></span>

* <span data-ttu-id="14cc9-3657">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3657">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="14cc9-3658">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3658">Add support for ssh key password prompting.</span></span> <span data-ttu-id="14cc9-3659">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3659">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="14cc9-3660">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3660">Add support for windows clusters.</span></span> <span data-ttu-id="14cc9-3661">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3661">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="14cc9-3662">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3662">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="14cc9-3663">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3663">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="14cc9-3664">AppService</span><span class="sxs-lookup"><span data-stu-id="14cc9-3664">AppService</span></span>

* <span data-ttu-id="14cc9-3665">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3665">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="14cc9-3666">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3666">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="14cc9-3667">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3667">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="14cc9-3668">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3668">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="14cc9-3669">DataLake</span><span class="sxs-lookup"><span data-stu-id="14cc9-3669">DataLake</span></span>

* <span data-ttu-id="14cc9-3670">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14cc9-3670">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="14cc9-3671">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14cc9-3671">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="14cc9-3672">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="14cc9-3672">DocuemntDB</span></span>

* <span data-ttu-id="14cc9-3673">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3673">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="14cc9-3674">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14cc9-3674">VM</span></span>

* <span data-ttu-id="14cc9-3675">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3675">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="14cc9-3676">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3676">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="14cc9-3677">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3677">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="14cc9-3678">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3678">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="14cc9-3679">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3679">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="14cc9-3680">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3680">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="14cc9-3681">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="14cc9-3681">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="14cc9-3682">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="14cc9-3682">February 27, 2017</span></span>

<span data-ttu-id="14cc9-3683">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="14cc9-3683">Version 2.0.0</span></span>

<span data-ttu-id="14cc9-3684">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="14cc9-3684">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="14cc9-3685">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3685">Container Service (acs)</span></span>
- <span data-ttu-id="14cc9-3686">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3686">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="14cc9-3687">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="14cc9-3687">Networking</span></span>
- <span data-ttu-id="14cc9-3688">Stockage</span><span class="sxs-lookup"><span data-stu-id="14cc9-3688">Storage</span></span>

<span data-ttu-id="14cc9-3689">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3689">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="14cc9-3690">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3690">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="14cc9-3691">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3691">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="14cc9-3692">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3692">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="14cc9-3693">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="14cc9-3693">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="14cc9-3694">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="14cc9-3694">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="14cc9-3695">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="14cc9-3695">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="14cc9-3696">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="14cc9-3696">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="14cc9-3697">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="14cc9-3697">Provide feedback from the command line with the `az feedback` command</span></span>
