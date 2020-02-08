---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/04/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: eafd18344ac4c1c0124ff53864a45510070b6fe7
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013282"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="1f138-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1f138-103">Azure CLI release notes</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="1f138-104">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="1f138-104">February 04, 2020</span></span>

<span data-ttu-id="1f138-105">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="1f138-105">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-106">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-106">ACS</span></span>

* <span data-ttu-id="1f138-107">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="1f138-107">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="1f138-108">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="1f138-108">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-109">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-109">ACR</span></span>

* <span data-ttu-id="1f138-110">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="1f138-110">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="1f138-111">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="1f138-111">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="1f138-112">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="1f138-112">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-113">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-113">AKS</span></span>

* <span data-ttu-id="1f138-114">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="1f138-114">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="1f138-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1f138-115">AppConfig</span></span>

* <span data-ttu-id="1f138-116">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="1f138-116">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="1f138-117">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="1f138-117">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="1f138-118">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="1f138-118">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="1f138-119">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="1f138-119">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="1f138-120">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="1f138-120">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-121">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-121">AppService</span></span>

* <span data-ttu-id="1f138-122">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="1f138-122">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="1f138-123">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-123">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-124">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-124">ARM</span></span>

* <span data-ttu-id="1f138-125">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-125">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="1f138-126">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="1f138-126">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="1f138-127">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="1f138-127">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="1f138-128">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="1f138-128">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="1f138-129">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="1f138-129">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="1f138-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="1f138-130">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="1f138-131">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="1f138-131">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-132">BotService</span><span class="sxs-lookup"><span data-stu-id="1f138-132">BotService</span></span>

* <span data-ttu-id="1f138-133">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="1f138-133">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="1f138-134">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="1f138-134">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-135">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-135">CDN</span></span>

* <span data-ttu-id="1f138-136">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="1f138-136">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="1f138-137">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="1f138-137">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="1f138-138">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="1f138-138">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="1f138-139">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="1f138-139">Deployment Manager</span></span>

* <span data-ttu-id="1f138-140">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="1f138-140">Add list operation for all resources.</span></span>
* <span data-ttu-id="1f138-141">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="1f138-141">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="1f138-142">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="1f138-142">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-143">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-143">IoT</span></span>

* <span data-ttu-id="1f138-144">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="1f138-144">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="1f138-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="1f138-145">IoT Central</span></span>

* <span data-ttu-id="1f138-146">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="1f138-146">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-147">Key Vault</span></span>

* <span data-ttu-id="1f138-148">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="1f138-148">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="1f138-149">Divers</span><span class="sxs-lookup"><span data-stu-id="1f138-149">Misc</span></span>

* <span data-ttu-id="1f138-150">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="1f138-150">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="1f138-151">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-151">Network</span></span>

* <span data-ttu-id="1f138-152">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="1f138-152">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="1f138-153">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="1f138-153">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="1f138-154">Stratégie</span><span class="sxs-lookup"><span data-stu-id="1f138-154">Policy</span></span>

* <span data-ttu-id="1f138-155">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="1f138-155">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="1f138-156">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="1f138-156">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-157">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-157">Profile</span></span>

* <span data-ttu-id="1f138-158">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-158">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-159">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-159">RBAC</span></span>

* <span data-ttu-id="1f138-160">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-160">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="1f138-161">Sécurité</span><span class="sxs-lookup"><span data-stu-id="1f138-161">Security</span></span>

* <span data-ttu-id="1f138-162">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="1f138-162">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-163">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-163">SQL</span></span>

* <span data-ttu-id="1f138-164">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="1f138-164">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="1f138-165">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="1f138-165">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="1f138-166">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="1f138-166">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="1f138-167">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="1f138-167">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="1f138-168">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="1f138-168">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="1f138-169">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="1f138-169">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-170">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-170">Storage</span></span>

* <span data-ttu-id="1f138-171">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="1f138-171">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="1f138-172">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="1f138-172">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="1f138-173">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="1f138-173">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="1f138-174">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1f138-174">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="1f138-175">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1f138-175">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="1f138-176">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1f138-176">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1f138-177">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f138-177">ServiceFabric</span></span>

* <span data-ttu-id="1f138-178">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="1f138-178">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="1f138-179">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="1f138-179">January 13, 2020</span></span>

<span data-ttu-id="1f138-180">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="1f138-180">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-181">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-181">Compute</span></span>

* <span data-ttu-id="1f138-182">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="1f138-182">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="1f138-183">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="1f138-183">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-184">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-184">Storage</span></span>

* <span data-ttu-id="1f138-185">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="1f138-185">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="1f138-186">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="1f138-186">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="1f138-187">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="1f138-187">January 07, 2020</span></span>

<span data-ttu-id="1f138-188">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="1f138-188">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-189">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-189">ACR</span></span>

* <span data-ttu-id="1f138-190">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="1f138-190">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="1f138-191">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="1f138-191">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="1f138-192">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1f138-192">AppConfig</span></span>

* <span data-ttu-id="1f138-193">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="1f138-193">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="1f138-194">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-194">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="1f138-195">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="1f138-195">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-196">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-196">AppService</span></span>

* <span data-ttu-id="1f138-197">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="1f138-197">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="1f138-198">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-198">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="1f138-199">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="1f138-199">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-200">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-200">ARM</span></span>

* <span data-ttu-id="1f138-201">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="1f138-201">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-202">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-202">Backup</span></span>

* <span data-ttu-id="1f138-203">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="1f138-203">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="1f138-204">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="1f138-204">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="1f138-205">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="1f138-205">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-206">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-206">Compute</span></span>

* <span data-ttu-id="1f138-207">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1f138-207">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="1f138-208">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="1f138-208">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="1f138-209">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="1f138-209">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-210">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-210">HDInsight</span></span>

* <span data-ttu-id="1f138-211">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="1f138-211">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="1f138-212">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="1f138-212">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="1f138-213">Divers</span><span class="sxs-lookup"><span data-stu-id="1f138-213">Misc.</span></span>

* <span data-ttu-id="1f138-214">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="1f138-214">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="1f138-215">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="1f138-215">Event Hubs</span></span>

* <span data-ttu-id="1f138-216">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="1f138-216">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="1f138-217">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="1f138-217">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="1f138-218">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-218">Service Bus</span></span>

* <span data-ttu-id="1f138-219">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="1f138-219">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="1f138-220">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="1f138-220">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-221">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-221">RBAC</span></span>

* <span data-ttu-id="1f138-222">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="1f138-222">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-223">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-223">Storage</span></span>

* <span data-ttu-id="1f138-224">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="1f138-224">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="1f138-225">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="1f138-225">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="1f138-226">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="1f138-226">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="1f138-227">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-227">December 17, 2019</span></span>

<span data-ttu-id="1f138-228">2.0.78</span><span class="sxs-lookup"><span data-stu-id="1f138-228">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-229">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-229">ACR</span></span>

* <span data-ttu-id="1f138-230">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="1f138-230">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-231">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-231">ACS</span></span>

* <span data-ttu-id="1f138-232">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="1f138-232">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-233">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-233">AMS</span></span>

* <span data-ttu-id="1f138-234">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="1f138-234">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="1f138-235">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1f138-235">AppConfig</span></span>

* <span data-ttu-id="1f138-236">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="1f138-236">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="1f138-237">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="1f138-237">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="1f138-238">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="1f138-238">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-239">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-239">AppService</span></span>

* <span data-ttu-id="1f138-240">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="1f138-240">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="1f138-241">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="1f138-241">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="1f138-242">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="1f138-242">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="1f138-243">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="1f138-243">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-244">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-244">ARM</span></span>

* <span data-ttu-id="1f138-245">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="1f138-245">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="1f138-246">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="1f138-246">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="1f138-247">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="1f138-247">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-248">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-248">Backup</span></span>

* <span data-ttu-id="1f138-249">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="1f138-249">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-250">BotService</span><span class="sxs-lookup"><span data-stu-id="1f138-250">BotService</span></span>

* <span data-ttu-id="1f138-251">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="1f138-251">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="1f138-252">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="1f138-252">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="1f138-253">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="1f138-253">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="1f138-254">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="1f138-254">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="1f138-255">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="1f138-255">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="1f138-256">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="1f138-256">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="1f138-257">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="1f138-257">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="1f138-258">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="1f138-258">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="1f138-259">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="1f138-259">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-260">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-260">Compute</span></span>

* <span data-ttu-id="1f138-261">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="1f138-261">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="1f138-262">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="1f138-262">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="1f138-263">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="1f138-263">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="1f138-264">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="1f138-264">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="1f138-265">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="1f138-265">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="1f138-266">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="1f138-266">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="1f138-267">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-267">Core</span></span>

* <span data-ttu-id="1f138-268">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="1f138-268">Removed support for Python 3.4</span></span>
* <span data-ttu-id="1f138-269">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-269">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="1f138-270">DLS</span><span class="sxs-lookup"><span data-stu-id="1f138-270">DLS</span></span>

* <span data-ttu-id="1f138-271">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="1f138-271">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="1f138-272">Installer</span><span class="sxs-lookup"><span data-stu-id="1f138-272">Install</span></span>

* <span data-ttu-id="1f138-273">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="1f138-273">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-274">IOT</span><span class="sxs-lookup"><span data-stu-id="1f138-274">IOT</span></span>

* <span data-ttu-id="1f138-275">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="1f138-275">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="1f138-276">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="1f138-276">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-277">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-277">Key Vault</span></span>

* <span data-ttu-id="1f138-278">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-278">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="1f138-279">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="1f138-279">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="1f138-280">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="1f138-280">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="1f138-281">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="1f138-281">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="1f138-282">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="1f138-282">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-283">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-283">Network</span></span>

* <span data-ttu-id="1f138-284">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-284">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="1f138-285">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-285">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="1f138-286">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="1f138-286">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="1f138-287">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="1f138-287">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="1f138-288">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="1f138-288">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="1f138-289">Packaging</span><span class="sxs-lookup"><span data-stu-id="1f138-289">Packaging</span></span>

* <span data-ttu-id="1f138-290">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="1f138-290">Added back edge builds for pip install</span></span>
* <span data-ttu-id="1f138-291">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="1f138-291">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="1f138-292">Stratégie</span><span class="sxs-lookup"><span data-stu-id="1f138-292">Policy</span></span>

* <span data-ttu-id="1f138-293">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="1f138-293">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="1f138-294">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="1f138-294">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="1f138-295">Redis</span><span class="sxs-lookup"><span data-stu-id="1f138-295">Redis</span></span>

* <span data-ttu-id="1f138-296">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="1f138-296">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="1f138-297">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="1f138-297">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1f138-298">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f138-298">ServiceFabric</span></span>

* <span data-ttu-id="1f138-299">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="1f138-299">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="1f138-300">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="1f138-300">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-301">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-301">SQL</span></span>

* <span data-ttu-id="1f138-302">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="1f138-302">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-303">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-303">Storage</span></span>

* <span data-ttu-id="1f138-304">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="1f138-304">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="1f138-305">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="1f138-305">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="1f138-306">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="1f138-306">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="1f138-307">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="1f138-307">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="1f138-308">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="1f138-308">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="1f138-309">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-309">November 26, 2019</span></span>

<span data-ttu-id="1f138-310">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="1f138-310">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-311">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-311">ACR</span></span>

* <span data-ttu-id="1f138-312">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="1f138-312">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="1f138-313">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="1f138-313">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="1f138-314">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="1f138-314">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="1f138-315">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="1f138-315">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-316">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-316">AKS</span></span>

* <span data-ttu-id="1f138-317">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="1f138-317">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="1f138-318">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1f138-318">AppConfig</span></span>

* <span data-ttu-id="1f138-319">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="1f138-319">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="1f138-320">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="1f138-320">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="1f138-321">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="1f138-321">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="1f138-322">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-322">AppService</span></span>

* <span data-ttu-id="1f138-323">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="1f138-323">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="1f138-324">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="1f138-324">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="1f138-325">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="1f138-325">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-326">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-326">Backup</span></span>

* <span data-ttu-id="1f138-327">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="1f138-327">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="1f138-328">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="1f138-328">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-329">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-329">Compute</span></span>

* <span data-ttu-id="1f138-330">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1f138-330">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="1f138-331">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="1f138-331">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="1f138-332">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="1f138-332">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="1f138-333">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="1f138-333">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="1f138-334">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="1f138-334">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="1f138-335">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="1f138-335">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="1f138-336">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="1f138-336">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="1f138-337">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="1f138-337">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="1f138-338">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="1f138-338">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="1f138-339">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="1f138-339">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-340">IOT</span><span class="sxs-lookup"><span data-stu-id="1f138-340">IOT</span></span>

* <span data-ttu-id="1f138-341">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="1f138-341">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="1f138-342">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="1f138-342">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="1f138-343">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="1f138-343">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-344">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-344">Key Vault</span></span>

* <span data-ttu-id="1f138-345">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="1f138-345">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="1f138-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="1f138-346">NetAppFiles</span></span>

* <span data-ttu-id="1f138-347">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="1f138-347">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="1f138-348">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-348">Network</span></span>

* <span data-ttu-id="1f138-349">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="1f138-349">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="1f138-350">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="1f138-350">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="1f138-351">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="1f138-351">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="1f138-352">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="1f138-352">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="1f138-353">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="1f138-353">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="1f138-354">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="1f138-354">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="1f138-355">Packaging</span><span class="sxs-lookup"><span data-stu-id="1f138-355">Packaging</span></span>

* <span data-ttu-id="1f138-356">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="1f138-356">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="1f138-357">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="1f138-357">Added support for Python 3.8</span></span>
* <span data-ttu-id="1f138-358">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="1f138-358">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-359">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-359">Profile</span></span>

* <span data-ttu-id="1f138-360">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="1f138-360">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="1f138-361">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="1f138-361">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="1f138-362">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="1f138-362">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="1f138-363">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="1f138-363">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="1f138-364">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="1f138-364">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-365">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-365">RBAC</span></span>

* <span data-ttu-id="1f138-366">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="1f138-366">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="1f138-367">Redis</span><span class="sxs-lookup"><span data-stu-id="1f138-367">Redis</span></span>

* <span data-ttu-id="1f138-368">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="1f138-368">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="1f138-369">Réservations</span><span class="sxs-lookup"><span data-stu-id="1f138-369">Reservations</span></span>

* <span data-ttu-id="1f138-370">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="1f138-370">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="1f138-371">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="1f138-371">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="1f138-372">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="1f138-372">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="1f138-373">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="1f138-373">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="1f138-374">Rest</span><span class="sxs-lookup"><span data-stu-id="1f138-374">Rest</span></span>
* <span data-ttu-id="1f138-375">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="1f138-375">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-376">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-376">SQL</span></span>

* <span data-ttu-id="1f138-377">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="1f138-377">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-378">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-378">Storage</span></span>

* <span data-ttu-id="1f138-379">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="1f138-379">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="1f138-380">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-380">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="1f138-381">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="1f138-381">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="1f138-382">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="1f138-382">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="1f138-383">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-383">November 4, 2019</span></span>

<span data-ttu-id="1f138-384">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="1f138-384">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-385">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-385">ACR</span></span>

* <span data-ttu-id="1f138-386">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="1f138-386">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="1f138-387">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="1f138-387">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="1f138-388">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="1f138-388">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-389">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-389">AKS</span></span>

* <span data-ttu-id="1f138-390">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="1f138-390">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="1f138-391">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="1f138-391">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="1f138-392">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1f138-392">AppConfig</span></span>

* <span data-ttu-id="1f138-393">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="1f138-393">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="1f138-394">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="1f138-394">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="1f138-395">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="1f138-395">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-396">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-396">AppService</span></span>

* <span data-ttu-id="1f138-397">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="1f138-397">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="1f138-398">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-398">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="1f138-399">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="1f138-399">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="1f138-400">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-400">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="1f138-401">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="1f138-401">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-402">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-402">ARM</span></span>

* <span data-ttu-id="1f138-403">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="1f138-403">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="1f138-404">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1f138-404">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-405">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-405">Backup</span></span>

* <span data-ttu-id="1f138-406">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="1f138-406">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-407">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-407">Compute</span></span>

* <span data-ttu-id="1f138-408">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="1f138-408">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="1f138-409">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="1f138-409">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="1f138-410">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="1f138-410">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="1f138-411">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="1f138-411">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="1f138-412">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="1f138-412">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="1f138-413">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1f138-413">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="1f138-414">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="1f138-414">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="1f138-415">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="1f138-415">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-416">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-416">CosmosDB</span></span>

* <span data-ttu-id="1f138-417">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="1f138-417">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="1f138-418">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="1f138-418">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="1f138-419">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-419">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="1f138-420">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="1f138-420">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="1f138-421">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-421">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="1f138-422">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="1f138-422">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="1f138-423">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-423">Fixed typo in help message</span></span>
* <span data-ttu-id="1f138-424">base de données : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="1f138-424">database: Added deprecation infomation</span></span>
* <span data-ttu-id="1f138-425">collection : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="1f138-425">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-426">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-426">IoT</span></span>

* <span data-ttu-id="1f138-427">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="1f138-427">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="1f138-428">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="1f138-428">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-429">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-429">Key Vault</span></span>

* <span data-ttu-id="1f138-430">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="1f138-430">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="1f138-431">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-431">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="1f138-432">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="1f138-432">NetAppFiles</span></span>

* <span data-ttu-id="1f138-433">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="1f138-433">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="1f138-434">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1f138-434">This new API version includes:</span></span>

    - <span data-ttu-id="1f138-435">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="1f138-435">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="1f138-436">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="1f138-436">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="1f138-437">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="1f138-437">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="1f138-438">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="1f138-438">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="1f138-439">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-439">Network</span></span>

* <span data-ttu-id="1f138-440">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="1f138-440">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="1f138-441">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="1f138-441">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="1f138-442">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="1f138-442">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="1f138-443">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="1f138-443">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="1f138-444">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="1f138-444">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="1f138-445">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="1f138-445">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-446">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-446">Profile</span></span>

* <span data-ttu-id="1f138-447">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-447">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="1f138-448">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="1f138-448">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-449">RBAC</span></span>

* <span data-ttu-id="1f138-450">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-450">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1f138-451">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f138-451">ServiceFabric</span></span>

* <span data-ttu-id="1f138-452">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="1f138-452">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-453">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-453">SQL</span></span>

* <span data-ttu-id="1f138-454">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="1f138-454">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-455">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-455">Storage</span></span>

* <span data-ttu-id="1f138-456">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f138-456">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="1f138-457">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="1f138-457">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="1f138-458">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-458">October 15, 2019</span></span>

<span data-ttu-id="1f138-459">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="1f138-459">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-460">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-460">AKS</span></span>

* <span data-ttu-id="1f138-461">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-461">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="1f138-462">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-462">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-463">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-463">AMS</span></span>

* <span data-ttu-id="1f138-464">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="1f138-464">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="1f138-465">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="1f138-465">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-466">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-466">AppService</span></span>

* <span data-ttu-id="1f138-467">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="1f138-467">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="1f138-468">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-468">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="1f138-469">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="1f138-469">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-470">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-470">ARM</span></span>

* <span data-ttu-id="1f138-471">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="1f138-471">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-472">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-472">Compute</span></span>

* <span data-ttu-id="1f138-473">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-473">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="1f138-474">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="1f138-474">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="1f138-475">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-475">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="1f138-476">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="1f138-476">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="1f138-477">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-477">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="1f138-478">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1f138-478">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="1f138-479">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-479">Core</span></span>

* <span data-ttu-id="1f138-480">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="1f138-480">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-481">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-481">IoT</span></span>

* <span data-ttu-id="1f138-482">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="1f138-482">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-483">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-483">Monitor</span></span>

* <span data-ttu-id="1f138-484">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="1f138-484">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-485">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-485">Network</span></span>

* <span data-ttu-id="1f138-486">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-486">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="1f138-487">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-487">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-488">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-488">SQL</span></span>

* <span data-ttu-id="1f138-489">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="1f138-489">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-490">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-490">Storage</span></span>

* <span data-ttu-id="1f138-491">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="1f138-491">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="1f138-492">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-492">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="1f138-493">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-493">September 24, 2019</span></span>

<span data-ttu-id="1f138-494">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="1f138-494">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-495">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-495">ACR</span></span>

* <span data-ttu-id="1f138-496">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="1f138-496">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="1f138-497">[CHANGEMENT CASSANT] Remplacement du paramètre `--name -n` par `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="1f138-497">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-498">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-498">AKS</span></span>

* <span data-ttu-id="1f138-499">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="1f138-499">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="1f138-500">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="1f138-500">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="1f138-501">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="1f138-501">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-502">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-502">ARM</span></span>

* <span data-ttu-id="1f138-503">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="1f138-503">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-504">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-504">Compute</span></span>

* <span data-ttu-id="1f138-505">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="1f138-505">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="1f138-506">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="1f138-506">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="1f138-507">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-507">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="1f138-508">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="1f138-508">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="1f138-509">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="1f138-509">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1f138-510">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-510">Cosmos DB</span></span>

* <span data-ttu-id="1f138-511">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="1f138-511">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="1f138-512">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="1f138-512">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="1f138-513">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="1f138-513">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1f138-514">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1f138-514">EventGrid</span></span>

* <span data-ttu-id="1f138-515">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="1f138-515">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-516">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-516">Key Vault</span></span>

* <span data-ttu-id="1f138-517">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="1f138-517">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-518">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-518">Monitor</span></span>

* <span data-ttu-id="1f138-519">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="1f138-519">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="1f138-520">Stratégie</span><span class="sxs-lookup"><span data-stu-id="1f138-520">Policy</span></span>

* <span data-ttu-id="1f138-521">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="1f138-521">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="1f138-522">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1f138-522">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-523">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-523">Storage</span></span>

* <span data-ttu-id="1f138-524">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="1f138-524">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="1f138-525">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-525">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-526">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-526">ACR</span></span>

* <span data-ttu-id="1f138-527">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="1f138-527">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-528">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-528">AKS</span></span>

* <span data-ttu-id="1f138-529">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="1f138-529">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="1f138-530">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-530">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="1f138-531">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-531">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-532">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-532">ARM</span></span>

* <span data-ttu-id="1f138-533">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="1f138-533">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-534">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-534">Batch</span></span>

* <span data-ttu-id="1f138-535">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="1f138-535">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="1f138-536">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="1f138-536">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="1f138-537">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="1f138-537">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="1f138-538">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="1f138-538">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="1f138-539">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="1f138-539">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="1f138-540">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="1f138-540">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="1f138-541">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="1f138-541">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-542">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-542">HDInsight</span></span>

* <span data-ttu-id="1f138-543">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="1f138-543">GA release</span></span>
* <span data-ttu-id="1f138-544">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="1f138-544">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-545">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-545">Key Vault</span></span>

* <span data-ttu-id="1f138-546">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-546">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="1f138-547">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-547">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="1f138-548">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-548">Network</span></span>

* <span data-ttu-id="1f138-549">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="1f138-549">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="1f138-550">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="1f138-550">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="1f138-551">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="1f138-551">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="1f138-552">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="1f138-552">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="1f138-553">Stratégie</span><span class="sxs-lookup"><span data-stu-id="1f138-553">Policy</span></span>

* <span data-ttu-id="1f138-554">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1f138-554">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="1f138-555">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-555">August 27, 2019</span></span>

<span data-ttu-id="1f138-556">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="1f138-556">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-557">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-557">ACR</span></span>

* <span data-ttu-id="1f138-558">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="1f138-558">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="1f138-559">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="1f138-559">API Management</span></span>

* <span data-ttu-id="1f138-560">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="1f138-560">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-561">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-561">AppService</span></span>

* <span data-ttu-id="1f138-562">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="1f138-562">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="1f138-563">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="1f138-563">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-564">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-564">Keyvault</span></span>

* <span data-ttu-id="1f138-565">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="1f138-565">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="1f138-566">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-566">Network</span></span>

* <span data-ttu-id="1f138-567">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="1f138-567">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="1f138-568">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="1f138-568">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="1f138-569">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="1f138-569">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="1f138-570">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1f138-570">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-571">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-571">RBAC</span></span>

* <span data-ttu-id="1f138-572">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-572">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1f138-573">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f138-573">ServiceFabric</span></span>

* <span data-ttu-id="1f138-574">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="1f138-574">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="1f138-575">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-575">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="1f138-576">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="1f138-576">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="1f138-577">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="1f138-577">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="1f138-578">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-578">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="1f138-579">SignalR</span><span class="sxs-lookup"><span data-stu-id="1f138-579">SignalR</span></span>

* <span data-ttu-id="1f138-580">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="1f138-580">Added new commands:</span></span>
  * <span data-ttu-id="1f138-581">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="1f138-581">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="1f138-582">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="1f138-582">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="1f138-583">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="1f138-583">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="1f138-584">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="1f138-584">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-585">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-585">Storage</span></span>

* <span data-ttu-id="1f138-586">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="1f138-586">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="1f138-587">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-587">August 13, 2019</span></span>

<span data-ttu-id="1f138-588">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="1f138-588">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-589">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-589">AppService</span></span>

* <span data-ttu-id="1f138-590">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="1f138-590">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-591">BotService</span><span class="sxs-lookup"><span data-stu-id="1f138-591">BotService</span></span>

* <span data-ttu-id="1f138-592">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="1f138-592">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="1f138-593">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1f138-593">CognitiveServices</span></span>

* <span data-ttu-id="1f138-594">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-594">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1f138-595">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-595">Cosmos DB</span></span>

* <span data-ttu-id="1f138-596">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="1f138-596">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="1f138-597">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-597">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-598">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-598">HDInsight</span></span>

<span data-ttu-id="1f138-599">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="1f138-599">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="1f138-600">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="1f138-600">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="1f138-601">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="1f138-601">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="1f138-602">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="1f138-602">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="1f138-603">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="1f138-603">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="1f138-604">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="1f138-604">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="1f138-605">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="1f138-605">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="1f138-606">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="1f138-606">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="1f138-607">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="1f138-607">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="1f138-608">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="1f138-608">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="1f138-609">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="1f138-609">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="1f138-610">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="1f138-610">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="1f138-611">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="1f138-611">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="1f138-612">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="1f138-612">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="1f138-613">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="1f138-613">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="1f138-614">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="1f138-614">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="1f138-615">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="1f138-615">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="1f138-616">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="1f138-616">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="1f138-617">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="1f138-617">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="1f138-618">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="1f138-618">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="1f138-619">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="1f138-619">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="1f138-620">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-620">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="1f138-621">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="1f138-621">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="1f138-622">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-622">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-623">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-623">Interactive</span></span>

* <span data-ttu-id="1f138-624">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="1f138-624">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="1f138-625">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-625">Kubernetes</span></span>

* <span data-ttu-id="1f138-626">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="1f138-626">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-627">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-627">Network</span></span>

* <span data-ttu-id="1f138-628">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-628">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-629">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-629">Profile</span></span>

* <span data-ttu-id="1f138-630">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-630">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1f138-631">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f138-631">ServiceFabric</span></span>

* <span data-ttu-id="1f138-632">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="1f138-632">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="1f138-633">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="1f138-633">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-634">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-634">Storage</span></span>

* <span data-ttu-id="1f138-635">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="1f138-635">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="1f138-636">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-636">July 30, 2019</span></span>

<span data-ttu-id="1f138-637">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="1f138-637">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-638">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-638">ACR</span></span>

* <span data-ttu-id="1f138-639">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="1f138-639">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="1f138-640">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="1f138-640">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-641">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-641">Appservice</span></span>

* <span data-ttu-id="1f138-642">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="1f138-642">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="1f138-643">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="1f138-643">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="1f138-644">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="1f138-644">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="1f138-645">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-645">Network</span></span>

* <span data-ttu-id="1f138-646">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="1f138-646">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="1f138-647">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="1f138-647">Fixes #9604.</span></span> <span data-ttu-id="1f138-648">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1f138-648">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="1f138-649">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="1f138-649">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-650">RBAC</span></span>

* <span data-ttu-id="1f138-651">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="1f138-651">Added `user update` command</span></span>
* <span data-ttu-id="1f138-652">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1f138-652">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="1f138-653">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="1f138-653">Use replacement argument `--id`</span></span>
* <span data-ttu-id="1f138-654">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1f138-654">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-655">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-655">SQL</span></span>

* <span data-ttu-id="1f138-656">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="1f138-656">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-657">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-657">Storage</span></span>

* <span data-ttu-id="1f138-658">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="1f138-658">Added `storage remove` command</span></span>
* <span data-ttu-id="1f138-659">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="1f138-659">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-660">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-660">VM</span></span>

* <span data-ttu-id="1f138-661">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="1f138-661">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="1f138-662">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1f138-662">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="1f138-663">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-663">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="1f138-664">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="1f138-664">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="1f138-665">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-665">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="1f138-666">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-666">July 16, 2019</span></span>

<span data-ttu-id="1f138-667">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="1f138-667">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-668">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-668">Appservice</span></span>

* <span data-ttu-id="1f138-669">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="1f138-669">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="1f138-670">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-670">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="1f138-671">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="1f138-671">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="1f138-672">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-672">Core</span></span>

* <span data-ttu-id="1f138-673">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-673">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-674">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-674">Batch</span></span>

* <span data-ttu-id="1f138-675">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="1f138-675">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="1f138-676">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="1f138-676">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="1f138-677">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="1f138-677">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="1f138-678">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-678">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1f138-679">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="1f138-679">Eventhubs</span></span>

* <span data-ttu-id="1f138-680">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="1f138-680">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-681">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-681">RDBMS</span></span>

* <span data-ttu-id="1f138-682">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="1f138-682">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="1f138-683">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="1f138-683">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="1f138-684">Relais</span><span class="sxs-lookup"><span data-stu-id="1f138-684">Relay</span></span>

* <span data-ttu-id="1f138-685">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="1f138-685">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="1f138-686">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="1f138-686">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="1f138-687">Servicebus</span><span class="sxs-lookup"><span data-stu-id="1f138-687">Servicebus</span></span>

* <span data-ttu-id="1f138-688">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="1f138-688">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-689">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-689">Storage</span></span>

* <span data-ttu-id="1f138-690">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-690">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="1f138-691">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="1f138-691">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="1f138-692">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-692">July 2, 2019</span></span>

<span data-ttu-id="1f138-693">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="1f138-693">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="1f138-694">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-694">Core</span></span>

* <span data-ttu-id="1f138-695">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="1f138-695">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="1f138-696">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="1f138-696">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="1f138-697">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="1f138-697">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-698">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-698">ACR</span></span>

* <span data-ttu-id="1f138-699">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="1f138-699">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-700">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-700">Appservice</span></span>

* <span data-ttu-id="1f138-701">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-701">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="1f138-702">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="1f138-702">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="1f138-703">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="1f138-703">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="1f138-704">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="1f138-704">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1f138-705">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-705">Cosmos DB</span></span>

* <span data-ttu-id="1f138-706">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="1f138-706">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="1f138-707">DLS</span><span class="sxs-lookup"><span data-stu-id="1f138-707">DLS</span></span>

* <span data-ttu-id="1f138-708">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="1f138-708">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="1f138-709">Commentaires</span><span class="sxs-lookup"><span data-stu-id="1f138-709">Feedback</span></span>

* <span data-ttu-id="1f138-710">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="1f138-710">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-711">HDInsight</span></span>

* <span data-ttu-id="1f138-712">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="1f138-712">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="1f138-713">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="1f138-713">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="1f138-714">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="1f138-714">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="1f138-715">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="1f138-715">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="1f138-716">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="1f138-716">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="1f138-717">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-717">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="1f138-718">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="1f138-718">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="1f138-719">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="1f138-719">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="1f138-720">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="1f138-720">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="1f138-721">Services gérés</span><span class="sxs-lookup"><span data-stu-id="1f138-721">Managed Services</span></span>

* <span data-ttu-id="1f138-722">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-722">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-723">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-723">Profile</span></span>
* <span data-ttu-id="1f138-724">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="1f138-724">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-725">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-725">RBAC</span></span>

* <span data-ttu-id="1f138-726">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1f138-726">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="1f138-727">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="1f138-727">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="1f138-728">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="1f138-728">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="1f138-729">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="1f138-729">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-730">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-730">RDBMS</span></span>

* <span data-ttu-id="1f138-731">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="1f138-731">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-732">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-732">SQL</span></span>

* <span data-ttu-id="1f138-733">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-733">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-734">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-734">Storage</span></span>

* <span data-ttu-id="1f138-735">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1f138-735">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="1f138-736">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1f138-736">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="1f138-737">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-737">VM</span></span>

* <span data-ttu-id="1f138-738">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-738">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="1f138-739">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="1f138-739">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="1f138-740">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-740">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="1f138-741">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="1f138-741">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="1f138-742">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-742">June 18, 2019</span></span>

<span data-ttu-id="1f138-743">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="1f138-743">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="1f138-744">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-744">Core</span></span>

<span data-ttu-id="1f138-745">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="1f138-745">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="1f138-746">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="1f138-746">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="1f138-747">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="1f138-747">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="1f138-748">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="1f138-748">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="1f138-749">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="1f138-749">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="1f138-750">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="1f138-750">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="1f138-751">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="1f138-751">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-752">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-752">ACR</span></span>
* <span data-ttu-id="1f138-753">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="1f138-753">Added 'acr check-health' command</span></span>
* <span data-ttu-id="1f138-754">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="1f138-754">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-755">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-755">ACS</span></span>
* <span data-ttu-id="1f138-756">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-756">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-757">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-757">AMS</span></span>
* <span data-ttu-id="1f138-758">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="1f138-758">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-759">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-759">AppService</span></span>
* <span data-ttu-id="1f138-760">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="1f138-760">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="1f138-761">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1f138-761">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="1f138-762">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="1f138-762">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="1f138-763">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-763">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="1f138-764">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="1f138-764">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="1f138-765">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="1f138-765">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-766">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-766">Batch</span></span>
* <span data-ttu-id="1f138-767">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="1f138-767">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-768">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-768">BatchAI</span></span>
* <span data-ttu-id="1f138-769">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="1f138-769">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-770">BotService</span><span class="sxs-lookup"><span data-stu-id="1f138-770">BotService</span></span>
* <span data-ttu-id="1f138-771">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="1f138-771">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-772">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-772">CosmosDB</span></span>
* <span data-ttu-id="1f138-773">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="1f138-773">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="1f138-774">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="1f138-774">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="1f138-775">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="1f138-775">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="1f138-776">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="1f138-776">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1f138-777">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1f138-777">EventGrid</span></span>
* <span data-ttu-id="1f138-778">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="1f138-778">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="1f138-779">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="1f138-779">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="1f138-780">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="1f138-780">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="1f138-781">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="1f138-781">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="1f138-782">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-782">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-783">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-783">HDInsight</span></span>
* <span data-ttu-id="1f138-784">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1f138-784">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-785">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-785">IoT</span></span>
* <span data-ttu-id="1f138-786">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="1f138-786">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="1f138-787">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="1f138-787">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="1f138-788">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-788">Network</span></span>
* <span data-ttu-id="1f138-789">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="1f138-789">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="1f138-790">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="1f138-790">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="1f138-791">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="1f138-791">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="1f138-792">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="1f138-792">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-793">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-793">Resource</span></span>
* <span data-ttu-id="1f138-794">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="1f138-794">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="1f138-795">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="1f138-795">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="1f138-796">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1f138-796">ServiceBus</span></span>
* <span data-ttu-id="1f138-797">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="1f138-797">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-798">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-798">SQL</span></span>
* <span data-ttu-id="1f138-799">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="1f138-799">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="1f138-800">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="1f138-800">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="1f138-801">SQLVm</span><span class="sxs-lookup"><span data-stu-id="1f138-801">SQLVm</span></span>
* <span data-ttu-id="1f138-802">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="1f138-802">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="1f138-803">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-803">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-804">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-804">Storage</span></span>
* <span data-ttu-id="1f138-805">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1f138-805">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="1f138-806">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-806">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-807">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-807">VM</span></span>
* <span data-ttu-id="1f138-808">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-808">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="1f138-809">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-809">June 4, 2019</span></span>

<span data-ttu-id="1f138-810">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="1f138-810">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="1f138-811">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-811">Core</span></span>
* <span data-ttu-id="1f138-812">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="1f138-812">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-813">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-813">ACR</span></span>
* <span data-ttu-id="1f138-814">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="1f138-814">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-815">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-815">ACS</span></span>
* <span data-ttu-id="1f138-816">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-816">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="1f138-817">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="1f138-817">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-818">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-818">Batch</span></span>
* <span data-ttu-id="1f138-819">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="1f138-819">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-820">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-820">IoT</span></span>
* <span data-ttu-id="1f138-821">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="1f138-821">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="1f138-822">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-822">Network</span></span>
* <span data-ttu-id="1f138-823">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="1f138-823">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="1f138-824">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-824">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="1f138-825">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-825">Resource</span></span>
* <span data-ttu-id="1f138-826">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="1f138-826">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="1f138-827">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-827">Role</span></span>
* <span data-ttu-id="1f138-828">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-828">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-829">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-829">Compute</span></span>
* <span data-ttu-id="1f138-830">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="1f138-830">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="1f138-831">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-831">May 21, 2019</span></span>

<span data-ttu-id="1f138-832">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="1f138-832">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="1f138-833">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-833">Core</span></span>
* <span data-ttu-id="1f138-834">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="1f138-834">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="1f138-835">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="1f138-835">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="1f138-836">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="1f138-836">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-837">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-837">ACR</span></span>
* <span data-ttu-id="1f138-838">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="1f138-838">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-839">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-839">ACS</span></span>
* <span data-ttu-id="1f138-840">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="1f138-840">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-841">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-841">AppService</span></span>
* <span data-ttu-id="1f138-842">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="1f138-842">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="1f138-843">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="1f138-843">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="1f138-844">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="1f138-844">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="1f138-845">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="1f138-845">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="1f138-846">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-846">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="1f138-847">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="1f138-847">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="1f138-848">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-848">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-849">BotService</span><span class="sxs-lookup"><span data-stu-id="1f138-849">BotService</span></span>
* <span data-ttu-id="1f138-850">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-850">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="1f138-851">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-851">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-852">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-852">Consumption</span></span>
* <span data-ttu-id="1f138-853">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-853">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-854">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-854">IoT</span></span>
* <span data-ttu-id="1f138-855">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="1f138-855">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="1f138-856">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-856">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="1f138-858">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="1f138-858">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="1f138-859">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="1f138-859">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-860">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-860">RDBMS</span></span>
* <span data-ttu-id="1f138-861">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="1f138-861">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-862">RBAC</span><span class="sxs-lookup"><span data-stu-id="1f138-862">RBAC</span></span>
* <span data-ttu-id="1f138-863">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="1f138-863">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-864">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-864">Storage</span></span>
* <span data-ttu-id="1f138-865">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-865">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="1f138-866">Calcul</span><span class="sxs-lookup"><span data-stu-id="1f138-866">Compute</span></span>
* <span data-ttu-id="1f138-867">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-867">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="1f138-868">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="1f138-868">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="1f138-869">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="1f138-869">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="1f138-870">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="1f138-870">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="1f138-871">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-871">May 6, 2019</span></span>

<span data-ttu-id="1f138-872">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="1f138-872">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-873">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-873">ACS</span></span>
* <span data-ttu-id="1f138-874">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="1f138-874">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="1f138-875">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="1f138-875">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="1f138-876">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="1f138-876">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="1f138-877">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-877">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-878">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-878">Appservice</span></span>
* <span data-ttu-id="1f138-879">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="1f138-879">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="1f138-880">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="1f138-880">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="1f138-881">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-881">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="1f138-882">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="1f138-882">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="1f138-883">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-883">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="1f138-884">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="1f138-884">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="1f138-885">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="1f138-885">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="1f138-886">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="1f138-886">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="1f138-887">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-887">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="1f138-888">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="1f138-888">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-889">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-889">Batch</span></span>
* <span data-ttu-id="1f138-890">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="1f138-890">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-891">Botservice</span><span class="sxs-lookup"><span data-stu-id="1f138-891">Botservice</span></span>
* <span data-ttu-id="1f138-892">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="1f138-892">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="1f138-893">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="1f138-893">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="1f138-894">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="1f138-894">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="1f138-895">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-895">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="1f138-896">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="1f138-896">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="1f138-897">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-897">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="1f138-898">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="1f138-898">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="1f138-899">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="1f138-899">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="1f138-900">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="1f138-900">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="1f138-901">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="1f138-901">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="1f138-902">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="1f138-902">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="1f138-903">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="1f138-903">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="1f138-904">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="1f138-904">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="1f138-905">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="1f138-905">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="1f138-906">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-906">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="1f138-907">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="1f138-907">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="1f138-908">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="1f138-908">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="1f138-909">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="1f138-909">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="1f138-910">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="1f138-910">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="1f138-911">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="1f138-911">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="1f138-912">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="1f138-912">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="1f138-913">Configurer</span><span class="sxs-lookup"><span data-stu-id="1f138-913">Configure</span></span>
* <span data-ttu-id="1f138-914">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="1f138-914">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1f138-915">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="1f138-915">Eventhubs</span></span>
* <span data-ttu-id="1f138-916">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-916">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="1f138-917">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-917">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-918">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-918">Network</span></span>
* <span data-ttu-id="1f138-919">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-919">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="1f138-920">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1f138-920">Policy Insights</span></span>
* <span data-ttu-id="1f138-921">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-921">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="1f138-922">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-922">Role</span></span>
* <span data-ttu-id="1f138-923">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-923">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="1f138-924">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-924">Service Bus</span></span>
* <span data-ttu-id="1f138-925">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-925">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="1f138-926">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-926">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="1f138-927">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="1f138-927">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-928">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-928">SQL</span></span>
* <span data-ttu-id="1f138-929">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="1f138-929">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-930">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-930">VM</span></span>
* <span data-ttu-id="1f138-931">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="1f138-931">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="1f138-932">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="1f138-932">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="1f138-933">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-933">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="1f138-934">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="1f138-934">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="1f138-935">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="1f138-935">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="1f138-936">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="1f138-936">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="1f138-937">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-937">April 23, 2019</span></span>

<span data-ttu-id="1f138-938">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="1f138-938">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-939">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-939">ACS</span></span>
* <span data-ttu-id="1f138-940">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="1f138-940">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="1f138-941">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="1f138-941">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-942">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-942">AMS</span></span>
* <span data-ttu-id="1f138-943">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="1f138-943">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-944">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-944">AppService</span></span>
* <span data-ttu-id="1f138-945">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="1f138-945">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="1f138-946">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="1f138-946">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="1f138-947">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="1f138-947">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="1f138-948">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="1f138-948">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="1f138-949">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="1f138-949">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="1f138-950">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-950">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="1f138-951">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="1f138-951">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="1f138-952">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="1f138-952">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="1f138-953">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="1f138-953">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="1f138-954">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="1f138-954">Deployment Manager</span></span>
* <span data-ttu-id="1f138-955">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="1f138-955">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="1f138-956">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-956">Lab</span></span>
* <span data-ttu-id="1f138-957">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="1f138-957">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="1f138-958">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-958">Network</span></span>
* <span data-ttu-id="1f138-959">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="1f138-959">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-960">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-960">Resource</span></span>
* <span data-ttu-id="1f138-961">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="1f138-961">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="1f138-962">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="1f138-962">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="1f138-963">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-963">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="1f138-964">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-964">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-965">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-965">SQL</span></span>
* <span data-ttu-id="1f138-966">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="1f138-966">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="1f138-967">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="1f138-967">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="1f138-968">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-968">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="1f138-969">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-969">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-970">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-970">Storage</span></span>
* <span data-ttu-id="1f138-971">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1f138-971">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-972">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-972">VM</span></span>
* <span data-ttu-id="1f138-973">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="1f138-973">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="1f138-974">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="1f138-974">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="1f138-975">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="1f138-975">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="1f138-976">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-976">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="1f138-977">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-977">Core</span></span>
* <span data-ttu-id="1f138-978">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-978">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-979">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-979">ACR</span></span>
* <span data-ttu-id="1f138-980">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="1f138-980">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-981">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-981">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="1f138-984">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="1f138-984">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="1f138-985">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="1f138-985">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-986">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-986">AppService</span></span>
* <span data-ttu-id="1f138-987">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-987">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="1f138-988">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="1f138-988">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="1f138-989">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="1f138-989">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="1f138-990">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="1f138-990">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="1f138-991">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-991">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="1f138-992">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="1f138-992">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="1f138-993">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="1f138-993">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-994">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-994">CDN</span></span>
* <span data-ttu-id="1f138-995">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="1f138-995">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="1f138-996">Commentaires</span><span class="sxs-lookup"><span data-stu-id="1f138-996">Feedback</span></span>
* <span data-ttu-id="1f138-997">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="1f138-997">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="1f138-998">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="1f138-998">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="1f138-999">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="1f138-999">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1000">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1000">Monitor</span></span>
* <span data-ttu-id="1f138-1001">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1001">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="1f138-1002">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1002">Network</span></span>
* <span data-ttu-id="1f138-1003">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="1f138-1003">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="1f138-1004">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-1004">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="1f138-1005">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="1f138-1005">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="1f138-1006">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1006">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="1f138-1007">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="1f138-1007">PrivateDNS</span></span>
* <span data-ttu-id="1f138-1008">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="1f138-1008">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1009">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1009">Resource</span></span>
* <span data-ttu-id="1f138-1010">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-1010">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1011">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1011">Role</span></span>
* <span data-ttu-id="1f138-1012">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-1012">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="1f138-1013">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1013">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1014">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1014">SQL</span></span>
* <span data-ttu-id="1f138-1015">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="1f138-1015">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1016">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1016">Storage</span></span>
* <span data-ttu-id="1f138-1017">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-1017">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="1f138-1018">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="1f138-1018">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="1f138-1019">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="1f138-1019">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="1f138-1020">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="1f138-1020">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="1f138-1021">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1021">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="1f138-1022">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1022">Core</span></span>
* <span data-ttu-id="1f138-1023">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="1f138-1023">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="1f138-1024">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="1f138-1024">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="1f138-1025">Cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-1025">Cloud</span></span>
* <span data-ttu-id="1f138-1026">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="1f138-1026">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1027">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1027">ACR</span></span>
* <span data-ttu-id="1f138-1028">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="1f138-1028">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="1f138-1029">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1029">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="1f138-1030">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="1f138-1030">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="1f138-1031">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="1f138-1031">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1032">AppService</span></span>
* <span data-ttu-id="1f138-1033">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="1f138-1033">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="1f138-1034">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="1f138-1034">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="1f138-1035">Service BOT</span><span class="sxs-lookup"><span data-stu-id="1f138-1035">BOT Service</span></span>
* <span data-ttu-id="1f138-1036">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="1f138-1036">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="1f138-1037">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-1037">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="1f138-1038">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="1f138-1038">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="1f138-1039">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="1f138-1039">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-1040">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-1040">CDN</span></span>
* <span data-ttu-id="1f138-1041">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1041">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="1f138-1042">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1042">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="1f138-1043">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="1f138-1043">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1f138-1044">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="1f138-1044">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-1045">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1f138-1045">Cosmosdb</span></span>
* <span data-ttu-id="1f138-1046">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="1f138-1046">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="1f138-1047">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-1047">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-1048">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1048">Interactive</span></span>
* <span data-ttu-id="1f138-1049">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="1f138-1049">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1050">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1050">Monitor</span></span>
* <span data-ttu-id="1f138-1051">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1051">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1052">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1052">Network</span></span>
* <span data-ttu-id="1f138-1053">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="1f138-1053">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-1054">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-1054">Profile</span></span>
* <span data-ttu-id="1f138-1055">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="1f138-1055">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="1f138-1056">Postgres</span><span class="sxs-lookup"><span data-stu-id="1f138-1056">Postgres</span></span> 
* <span data-ttu-id="1f138-1057">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="1f138-1057">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="1f138-1058">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="1f138-1058">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1059">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1059">Resource</span></span>
* <span data-ttu-id="1f138-1060">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1060">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="1f138-1061">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="1f138-1061">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="1f138-1062">Graph</span><span class="sxs-lookup"><span data-stu-id="1f138-1062">Graph</span></span>
* <span data-ttu-id="1f138-1063">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="1f138-1063">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="1f138-1064">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="1f138-1064">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="1f138-1065">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="1f138-1065">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="1f138-1066">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1066">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="1f138-1067">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-1067">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1068">storage</span><span class="sxs-lookup"><span data-stu-id="1f138-1068">storage</span></span>
* <span data-ttu-id="1f138-1069">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="1f138-1069">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="1f138-1070">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="1f138-1070">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="1f138-1071">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="1f138-1071">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="1f138-1072">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="1f138-1072">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1073">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1073">VM</span></span>
* <span data-ttu-id="1f138-1074">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1074">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="1f138-1075">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1075">March 12, 2019</span></span>

<span data-ttu-id="1f138-1076">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="1f138-1076">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1077">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1077">Core</span></span>

* <span data-ttu-id="1f138-1078">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="1f138-1078">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1079">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1079">ACR</span></span>

* <span data-ttu-id="1f138-1080">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="1f138-1080">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1081">ACS</span></span>

* <span data-ttu-id="1f138-1082">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="1f138-1082">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="1f138-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1083">AppService</span></span>

* <span data-ttu-id="1f138-1084">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="1f138-1084">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="1f138-1085">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1085">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="1f138-1086">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-1086">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="1f138-1087">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="1f138-1087">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-1088">Botservice</span><span class="sxs-lookup"><span data-stu-id="1f138-1088">Botservice</span></span>

* <span data-ttu-id="1f138-1089">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="1f138-1089">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1f138-1090">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="1f138-1090">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1f138-1091">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1091">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="1f138-1092">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="1f138-1092">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1093">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1093">Container</span></span>

* <span data-ttu-id="1f138-1094">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1094">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="1f138-1095">Event Hub</span><span class="sxs-lookup"><span data-stu-id="1f138-1095">EventHub</span></span>

* <span data-ttu-id="1f138-1096">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="1f138-1096">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="1f138-1097">Rechercher</span><span class="sxs-lookup"><span data-stu-id="1f138-1097">Find</span></span>

* <span data-ttu-id="1f138-1098">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="1f138-1098">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-1099">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-1099">HDInsight</span></span>

* <span data-ttu-id="1f138-1100">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="1f138-1100">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1101">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1101">Network</span></span>

* <span data-ttu-id="1f138-1102">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="1f138-1102">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1f138-1103">Rdbms</span></span>

* <span data-ttu-id="1f138-1104">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="1f138-1104">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1105">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1105">Role</span></span>

* <span data-ttu-id="1f138-1106">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="1f138-1106">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="1f138-1107">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="1f138-1107">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1f138-1108">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1f138-1108">Service Fabric</span></span>

* <span data-ttu-id="1f138-1109">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="1f138-1109">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="1f138-1110">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1110">February 26, 2019</span></span>

<span data-ttu-id="1f138-1111">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="1f138-1111">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1112">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1112">Core</span></span>

* <span data-ttu-id="1f138-1113">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="1f138-1113">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1114">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1114">ACR</span></span>

* <span data-ttu-id="1f138-1115">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1115">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="1f138-1116">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="1f138-1116">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1117">ACS</span></span>

* <span data-ttu-id="1f138-1118">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="1f138-1118">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1119">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1119">AppService</span></span>

* <span data-ttu-id="1f138-1120">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="1f138-1120">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1121">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1121">Batch</span></span>
* <span data-ttu-id="1f138-1122">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="1f138-1122">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="1f138-1123">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="1f138-1123">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="1f138-1124">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="1f138-1124">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="1f138-1125">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="1f138-1125">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="1f138-1126">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="1f138-1126">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="1f138-1127">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="1f138-1127">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-1128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-1128">CosmosDB</span></span>

* <span data-ttu-id="1f138-1129">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-1129">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="1f138-1130">Kusto</span><span class="sxs-lookup"><span data-stu-id="1f138-1130">Kusto</span></span>

* <span data-ttu-id="1f138-1131">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="1f138-1131">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1132">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1132">Network</span></span>

* <span data-ttu-id="1f138-1133">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1133">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="1f138-1134">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="1f138-1134">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="1f138-1135">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="1f138-1135">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="1f138-1136">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1136">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="1f138-1137">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1137">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="1f138-1138">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1138">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="1f138-1139">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="1f138-1139">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1140">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1140">Resource</span></span>

* <span data-ttu-id="1f138-1141">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-1141">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="1f138-1142">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1142">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="1f138-1143">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1143">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="1f138-1144">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1144">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="1f138-1145">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1145">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1146">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1146">Role</span></span>

* <span data-ttu-id="1f138-1147">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1147">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1148">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1148">VM</span></span>

* <span data-ttu-id="1f138-1149">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="1f138-1149">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="1f138-1150">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1150">February 12, 2019</span></span>

<span data-ttu-id="1f138-1151">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="1f138-1151">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1152">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1152">Core</span></span>

* <span data-ttu-id="1f138-1153">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-1153">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="1f138-1154">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="1f138-1154">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1155">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1155">ACR</span></span>
* <span data-ttu-id="1f138-1156">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="1f138-1156">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="1f138-1157">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-1157">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1158">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1158">ACS</span></span>
* <span data-ttu-id="1f138-1159">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1159">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="1f138-1160">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="1f138-1160">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="1f138-1161">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1f138-1161">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-1162">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-1162">AMS</span></span>
* <span data-ttu-id="1f138-1163">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1163">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="1f138-1164">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1164">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1165">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1165">Appservice</span></span>
* <span data-ttu-id="1f138-1166">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1166">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="1f138-1167">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="1f138-1167">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="1f138-1168">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1168">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="1f138-1169">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="1f138-1169">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="1f138-1170">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="1f138-1170">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-1171">Botservice</span><span class="sxs-lookup"><span data-stu-id="1f138-1171">Botservice</span></span>
* <span data-ttu-id="1f138-1172">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="1f138-1172">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="1f138-1173">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="1f138-1173">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="1f138-1174">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1174">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="1f138-1175">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="1f138-1175">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="1f138-1176">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="1f138-1176">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="1f138-1177">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="1f138-1177">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="1f138-1178">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="1f138-1178">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="1f138-1179">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="1f138-1179">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="1f138-1180">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="1f138-1180">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="1f138-1181">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="1f138-1181">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-1182">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-1182">Key Vault</span></span>
* <span data-ttu-id="1f138-1183">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="1f138-1183">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1184">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1184">Monitor</span></span>
* <span data-ttu-id="1f138-1185">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="1f138-1185">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1186">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1186">Network</span></span>
* <span data-ttu-id="1f138-1187">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="1f138-1187">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="1f138-1188">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="1f138-1188">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="1f138-1189">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-1189">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="1f138-1190">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1190">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="1f138-1191">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1f138-1191">Policy Insights</span></span>
* <span data-ttu-id="1f138-1192">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-1192">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1193">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-1193">RDBMS</span></span>
* <span data-ttu-id="1f138-1194">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-1194">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="1f138-1195">Redis</span><span class="sxs-lookup"><span data-stu-id="1f138-1195">Redis</span></span>
* <span data-ttu-id="1f138-1196">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="1f138-1196">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="1f138-1197">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="1f138-1197">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="1f138-1198">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="1f138-1198">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="1f138-1199">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="1f138-1199">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="1f138-1200">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="1f138-1200">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="1f138-1201">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="1f138-1201">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="1f138-1202">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="1f138-1202">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1203">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1203">Role</span></span>
* <span data-ttu-id="1f138-1204">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="1f138-1204">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="1f138-1205">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1205">SQL VM</span></span>
* <span data-ttu-id="1f138-1206">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="1f138-1206">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1207">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1207">VM</span></span>
* <span data-ttu-id="1f138-1208">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="1f138-1208">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="1f138-1209">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1209">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="1f138-1210">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="1f138-1210">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="1f138-1211">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="1f138-1211">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="1f138-1212">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1212">January 31, 2019</span></span>

<span data-ttu-id="1f138-1213">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="1f138-1213">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1214">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1214">Core</span></span>

* <span data-ttu-id="1f138-1215">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="1f138-1215">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="1f138-1216">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1216">January 28, 2019</span></span>

<span data-ttu-id="1f138-1217">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="1f138-1217">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1218">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1218">ACR</span></span>
* <span data-ttu-id="1f138-1219">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="1f138-1219">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1220">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1220">ACS</span></span>
* <span data-ttu-id="1f138-1221">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="1f138-1221">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1f138-1222">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="1f138-1222">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="1f138-1223">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="1f138-1223">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-1224">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-1224">AMS</span></span>
* <span data-ttu-id="1f138-1225">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="1f138-1225">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="1f138-1226">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="1f138-1226">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1227">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1227">Appservice</span></span>
* <span data-ttu-id="1f138-1228">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1228">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="1f138-1229">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="1f138-1229">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="1f138-1230">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="1f138-1230">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1231">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1231">Container</span></span>
* <span data-ttu-id="1f138-1232">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="1f138-1232">Added `container start` command</span></span>
* <span data-ttu-id="1f138-1233">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1233">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1f138-1234">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1f138-1234">EventGrid</span></span>
* <span data-ttu-id="1f138-1235">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1235">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="1f138-1236">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="1f138-1236">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="1f138-1237">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="1f138-1237">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="1f138-1238">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="1f138-1238">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="1f138-1239">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="1f138-1239">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-1240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-1240">HDInsight</span></span>
* <span data-ttu-id="1f138-1241">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1241">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="1f138-1242">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="1f138-1242">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="1f138-1243">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1243">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="1f138-1244">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1244">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="1f138-1245">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="1f138-1245">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="1f138-1246">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1246">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1247">IoT</span></span>
* <span data-ttu-id="1f138-1248">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="1f138-1248">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="1f138-1249">Kusto</span><span class="sxs-lookup"><span data-stu-id="1f138-1249">Kusto</span></span>
* <span data-ttu-id="1f138-1250">Préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-1250">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1251">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1251">Monitor</span></span>
* <span data-ttu-id="1f138-1252">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-1252">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-1253">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-1253">Profile</span></span>
* <span data-ttu-id="1f138-1254">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="1f138-1254">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1255">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1255">Network</span></span>
* <span data-ttu-id="1f138-1256">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="1f138-1256">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="1f138-1257">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="1f138-1257">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1258">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1258">Resource</span></span>
* <span data-ttu-id="1f138-1259">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1259">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="1f138-1260">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1260">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="1f138-1261">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1261">SQL Virtual Machine</span></span>
* <span data-ttu-id="1f138-1262">Préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-1262">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1263">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1263">Storage</span></span>
* <span data-ttu-id="1f138-1264">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="1f138-1264">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="1f138-1265">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="1f138-1265">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1266">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1266">VM</span></span>
* <span data-ttu-id="1f138-1267">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="1f138-1267">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="1f138-1268">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1f138-1268">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="1f138-1269">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="1f138-1269">January 15, 2019</span></span>

<span data-ttu-id="1f138-1270">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="1f138-1270">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1271">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1271">ACR</span></span>
* <span data-ttu-id="1f138-1272">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="1f138-1272">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="1f138-1273">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-1273">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="1f138-1274">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="1f138-1274">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="1f138-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1275">ACS</span></span>
* <span data-ttu-id="1f138-1276">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="1f138-1276">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1277">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1277">Appservice</span></span>
* <span data-ttu-id="1f138-1278">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="1f138-1278">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="1f138-1279">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-1279">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="1f138-1280">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="1f138-1280">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="1f138-1281">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="1f138-1281">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-1282">Botservice</span><span class="sxs-lookup"><span data-stu-id="1f138-1282">Botservice</span></span>
* <span data-ttu-id="1f138-1283">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1283">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="1f138-1284">Configurer</span><span class="sxs-lookup"><span data-stu-id="1f138-1284">Configure</span></span>
* <span data-ttu-id="1f138-1285">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="1f138-1285">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-1286">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-1286">CosmosDB</span></span>
* <span data-ttu-id="1f138-1287">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="1f138-1287">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-1288">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-1288">HDInsight</span></span>
* <span data-ttu-id="1f138-1289">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="1f138-1289">Added commands for managing applications</span></span>
* <span data-ttu-id="1f138-1290">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="1f138-1290">Added commands for managing script actions</span></span>
* <span data-ttu-id="1f138-1291">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="1f138-1291">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="1f138-1292">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="1f138-1292">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="1f138-1293">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1293">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1294">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1294">Network</span></span>
* <span data-ttu-id="1f138-1295">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1295">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="1f138-1296">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="1f138-1296">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="1f138-1297">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1297">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="1f138-1298">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-1298">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1299">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1299">Role</span></span>
* <span data-ttu-id="1f138-1300">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1300">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="1f138-1301">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="1f138-1301">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="1f138-1302">Sécurité</span><span class="sxs-lookup"><span data-stu-id="1f138-1302">Security</span></span>
* <span data-ttu-id="1f138-1303">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-1303">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1304">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1304">Storage</span></span>
* <span data-ttu-id="1f138-1305">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="1f138-1305">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="1f138-1306">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="1f138-1306">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="1f138-1307">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1307">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="1f138-1308">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1308">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="1f138-1309">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1309">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1310">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1310">VM</span></span>
* <span data-ttu-id="1f138-1311">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="1f138-1311">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="1f138-1312">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1312">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1f138-1313">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="1f138-1313">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="1f138-1314">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="1f138-1314">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="1f138-1315">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-1315">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="1f138-1316">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-1316">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="1f138-1317">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1317">December 20, 2018</span></span>

<span data-ttu-id="1f138-1318">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="1f138-1318">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="1f138-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1319">Appservice</span></span>
* <span data-ttu-id="1f138-1320">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1f138-1320">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="1f138-1321">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="1f138-1321">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="1f138-1322">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-1322">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1f138-1323">IotCentral</span><span class="sxs-lookup"><span data-stu-id="1f138-1323">IoTCentral</span></span>
* <span data-ttu-id="1f138-1324">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-1324">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1325">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1325">Role</span></span>
* <span data-ttu-id="1f138-1326">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="1f138-1326">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1327">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1327">SQL</span></span>
* <span data-ttu-id="1f138-1328">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="1f138-1328">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1329">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1329">VM</span></span>
* <span data-ttu-id="1f138-1330">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1330">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="1f138-1331">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1331">December 18, 2018</span></span>

<span data-ttu-id="1f138-1332">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="1f138-1332">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="1f138-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1333">ACR</span></span>
* <span data-ttu-id="1f138-1334">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="1f138-1334">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="1f138-1335">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="1f138-1335">Condensed the table layout for task list</span></span>
* <span data-ttu-id="1f138-1336">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="1f138-1336">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1337">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1337">ACS</span></span>
* <span data-ttu-id="1f138-1338">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="1f138-1338">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1f138-1339">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1339">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="1f138-1340">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1340">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="1f138-1341">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="1f138-1341">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="1f138-1342">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-1342">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="1f138-1343">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="1f138-1343">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1344">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1344">Appservice</span></span>
* <span data-ttu-id="1f138-1345">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="1f138-1345">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="1f138-1346">Botservice</span><span class="sxs-lookup"><span data-stu-id="1f138-1346">Botservice</span></span>
* <span data-ttu-id="1f138-1347">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="1f138-1347">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="1f138-1348">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="1f138-1348">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="1f138-1349">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="1f138-1349">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="1f138-1350">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="1f138-1350">Reduced Kudu network calls</span></span>
* <span data-ttu-id="1f138-1351">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="1f138-1351">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-1352">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-1352">Consumption</span></span>
* <span data-ttu-id="1f138-1353">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="1f138-1353">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-1354">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-1354">CosmosDB</span></span>
* <span data-ttu-id="1f138-1355">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="1f138-1355">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="1f138-1356">Cartes</span><span class="sxs-lookup"><span data-stu-id="1f138-1356">Maps</span></span>
* <span data-ttu-id="1f138-1357">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1357">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1358">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1358">Network</span></span>
* <span data-ttu-id="1f138-1359">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="1f138-1359">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="1f138-1360">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-1360">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1361">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1361">Resource</span></span>
* <span data-ttu-id="1f138-1362">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1362">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="1f138-1363">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1363">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1364">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1364">Storage</span></span>
*  <span data-ttu-id="1f138-1365">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1365">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1366">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1366">VM</span></span>
* <span data-ttu-id="1f138-1367">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="1f138-1367">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="1f138-1368">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1368">December 4, 2018</span></span>

<span data-ttu-id="1f138-1369">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="1f138-1369">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="1f138-1370">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1370">Core</span></span>
* <span data-ttu-id="1f138-1371">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="1f138-1371">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="1f138-1372">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="1f138-1372">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1373">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1373">Appservice</span></span>
* <span data-ttu-id="1f138-1374">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="1f138-1374">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="1f138-1375">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="1f138-1375">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1376">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1376">Network</span></span>
* <span data-ttu-id="1f138-1377">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="1f138-1377">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1378">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1378">Role</span></span>
* <span data-ttu-id="1f138-1379">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="1f138-1379">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="1f138-1380">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1380">VM</span></span>
* <span data-ttu-id="1f138-1381">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="1f138-1381">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="1f138-1382">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="1f138-1382">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="1f138-1383">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="1f138-1383">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="1f138-1384">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="1f138-1384">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="1f138-1385">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1385">November 20, 2018</span></span>

<span data-ttu-id="1f138-1386">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="1f138-1386">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="1f138-1387">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1387">Core</span></span>
* <span data-ttu-id="1f138-1388">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="1f138-1388">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1389">ACR</span></span>
* <span data-ttu-id="1f138-1390">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="1f138-1390">Added context token to task step</span></span>
* <span data-ttu-id="1f138-1391">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="1f138-1391">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="1f138-1392">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="1f138-1392">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1393">Appservice</span></span>
* <span data-ttu-id="1f138-1394">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="1f138-1394">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="1f138-1395">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1395">Updated the default `node_version`.</span></span> <span data-ttu-id="1f138-1396">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="1f138-1396">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="1f138-1397">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-1397">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="1f138-1398">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="1f138-1398">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1f138-1399">IotCentral</span><span class="sxs-lookup"><span data-stu-id="1f138-1399">IotCentral</span></span>
* <span data-ttu-id="1f138-1400">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="1f138-1400">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-1401">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-1401">KeyVault</span></span>
* <span data-ttu-id="1f138-1402">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="1f138-1402">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1403">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1403">Network</span></span>
* <span data-ttu-id="1f138-1404">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="1f138-1404">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="1f138-1405">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="1f138-1405">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="1f138-1406">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1406">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="1f138-1407">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="1f138-1407">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1408">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1f138-1408">Rdbms</span></span>
* <span data-ttu-id="1f138-1409">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="1f138-1409">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="1f138-1410">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="1f138-1410">Rbac</span></span>
* <span data-ttu-id="1f138-1411">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1411">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="1f138-1412">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1412">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="1f138-1413">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1413">Storage</span></span>
* <span data-ttu-id="1f138-1414">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1414">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="1f138-1415">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1415">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="1f138-1416">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="1f138-1416">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="1f138-1417">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="1f138-1417">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1418">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1418">VM</span></span>
* <span data-ttu-id="1f138-1419">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="1f138-1419">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="1f138-1420">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="1f138-1420">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="1f138-1421">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="1f138-1421">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="1f138-1422">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="1f138-1422">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="1f138-1423">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1423">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="1f138-1424">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1424">Added `snapshot wait` command</span></span>
* <span data-ttu-id="1f138-1425">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-1425">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="1f138-1426">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1426">November 6, 2018</span></span>

<span data-ttu-id="1f138-1427">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="1f138-1427">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1428">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1428">Core</span></span>
* <span data-ttu-id="1f138-1429">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="1f138-1429">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1430">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1430">ACR</span></span>
* <span data-ttu-id="1f138-1431">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="1f138-1431">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="1f138-1432">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="1f138-1432">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1433">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1433">ACS</span></span>
* <span data-ttu-id="1f138-1434">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-1434">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="1f138-1435">Advisor</span><span class="sxs-lookup"><span data-stu-id="1f138-1435">Advisor</span></span>
* <span data-ttu-id="1f138-1436">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="1f138-1436">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-1437">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-1437">AMS</span></span>
* <span data-ttu-id="1f138-1438">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="1f138-1438">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="1f138-1439">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="1f138-1439">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="1f138-1440">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1440">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="1f138-1441">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="1f138-1441">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="1f138-1442">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="1f138-1442">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="1f138-1443">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="1f138-1443">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="1f138-1444">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="1f138-1444">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="1f138-1445">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="1f138-1445">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="1f138-1446">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="1f138-1446">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="1f138-1447">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="1f138-1447">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="1f138-1448">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-1448">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="1f138-1449">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1449">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="1f138-1450">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="1f138-1450">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="1f138-1451">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="1f138-1451">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="1f138-1452">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1452">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="1f138-1453">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="1f138-1453">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="1f138-1454">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="1f138-1454">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1455">AppService</span></span>
* <span data-ttu-id="1f138-1456">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="1f138-1456">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="1f138-1457">Configurer</span><span class="sxs-lookup"><span data-stu-id="1f138-1457">Configure</span></span>
* <span data-ttu-id="1f138-1458">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="1f138-1458">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1459">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1459">Container</span></span>
* <span data-ttu-id="1f138-1460">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="1f138-1460">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="1f138-1461">Event Hub</span><span class="sxs-lookup"><span data-stu-id="1f138-1461">EventHub</span></span>
* <span data-ttu-id="1f138-1462">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1462">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1463">Interactive</span></span>
* <span data-ttu-id="1f138-1464">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="1f138-1464">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1465">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1465">Monitor</span></span>
* <span data-ttu-id="1f138-1466">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1466">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1467">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1467">Network</span></span>
* <span data-ttu-id="1f138-1468">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="1f138-1468">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="1f138-1469">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1469">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="1f138-1470">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1470">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="1f138-1471">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-1471">Profile</span></span>
* <span data-ttu-id="1f138-1472">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="1f138-1472">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1473">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-1473">RDBMS</span></span>
* <span data-ttu-id="1f138-1474">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="1f138-1474">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1475">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1475">Resource</span></span>
* <span data-ttu-id="1f138-1476">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="1f138-1476">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1477">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1477">Role</span></span>
* <span data-ttu-id="1f138-1478">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="1f138-1478">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="1f138-1479">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="1f138-1479">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="1f138-1480">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="1f138-1480">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1481">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1481">Storage</span></span>
* <span data-ttu-id="1f138-1482">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="1f138-1482">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1483">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1483">VM</span></span>
* <span data-ttu-id="1f138-1484">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="1f138-1484">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="1f138-1485">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="1f138-1485">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="1f138-1486">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="1f138-1486">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="1f138-1487">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="1f138-1487">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="1f138-1488">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="1f138-1488">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="1f138-1489">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="1f138-1489">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="1f138-1490">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1490">October 23, 2018</span></span>

<span data-ttu-id="1f138-1491">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="1f138-1491">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1492">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1492">Core</span></span>
* <span data-ttu-id="1f138-1493">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="1f138-1493">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="1f138-1494">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="1f138-1494">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1495">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1495">ACR</span></span>
* <span data-ttu-id="1f138-1496">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="1f138-1496">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-1497">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-1497">CDN</span></span>
* <span data-ttu-id="1f138-1498">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="1f138-1498">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1f138-1499">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="1f138-1499">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1500">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1500">Container</span></span>
* <span data-ttu-id="1f138-1501">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="1f138-1501">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="1f138-1502">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-1502">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="1f138-1503">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="1f138-1503">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="1f138-1504">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-1504">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="1f138-1505">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="1f138-1505">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="1f138-1506">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="1f138-1506">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="1f138-1507">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="1f138-1507">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-1508">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-1508">CosmosDB</span></span>
* <span data-ttu-id="1f138-1509">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1509">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-1510">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1510">Interactive</span></span>
* <span data-ttu-id="1f138-1511">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="1f138-1511">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="1f138-1512">IoT Central</span><span class="sxs-lookup"><span data-stu-id="1f138-1512">IoT Central</span></span>
* <span data-ttu-id="1f138-1513">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="1f138-1513">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="1f138-1514">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="1f138-1514">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1515">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1515">Monitor</span></span>
* <span data-ttu-id="1f138-1516">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="1f138-1516">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="1f138-1517">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1517">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="1f138-1518">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="1f138-1518">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1f138-1519">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="1f138-1519">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="1f138-1520">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="1f138-1520">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="1f138-1521">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="1f138-1521">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="1f138-1522">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="1f138-1522">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="1f138-1523">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="1f138-1523">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1f138-1524">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="1f138-1524">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="1f138-1525">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1525">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1526">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1526">Network</span></span>
* <span data-ttu-id="1f138-1527">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1527">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="1f138-1528">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1528">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="1f138-1529">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1f138-1529">ServiceBus</span></span>
* <span data-ttu-id="1f138-1530">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-1530">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1531">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1531">SQL</span></span>
* <span data-ttu-id="1f138-1532">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="1f138-1532">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1533">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1533">Storage</span></span>
* <span data-ttu-id="1f138-1534">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="1f138-1534">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="1f138-1535">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="1f138-1535">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1536">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1536">VM</span></span>
* <span data-ttu-id="1f138-1537">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1537">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="1f138-1538">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1538">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="1f138-1539">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1539">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="1f138-1540">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1540">October 16, 2018</span></span>

<span data-ttu-id="1f138-1541">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="1f138-1541">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1542">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1542">VM</span></span>
* <span data-ttu-id="1f138-1543">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="1f138-1543">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="1f138-1544">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1544">October 9, 2018</span></span>

<span data-ttu-id="1f138-1545">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="1f138-1545">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1546">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1546">Core</span></span>
* <span data-ttu-id="1f138-1547">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="1f138-1547">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1548">ACR</span></span>
* <span data-ttu-id="1f138-1549">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="1f138-1549">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1550">ACS</span></span>
* <span data-ttu-id="1f138-1551">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="1f138-1551">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="1f138-1552">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="1f138-1552">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="1f138-1553">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="1f138-1553">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="1f138-1554">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="1f138-1554">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1555">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1555">Container</span></span>
* <span data-ttu-id="1f138-1556">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="1f138-1556">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="1f138-1557">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-1557">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="1f138-1558">Event Hub</span><span class="sxs-lookup"><span data-stu-id="1f138-1558">Event Hub</span></span>
* <span data-ttu-id="1f138-1559">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1559">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="1f138-1560">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="1f138-1560">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="1f138-1561">Extensions</span><span class="sxs-lookup"><span data-stu-id="1f138-1561">Extensions</span></span>
* <span data-ttu-id="1f138-1562">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="1f138-1562">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1f138-1563">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f138-1563">HDInsight</span></span>
* <span data-ttu-id="1f138-1564">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-1564">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1565">IoT</span></span>
* <span data-ttu-id="1f138-1566">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="1f138-1566">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-1567">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-1567">KeyVault</span></span>
* <span data-ttu-id="1f138-1568">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="1f138-1568">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1569">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1569">Network</span></span>
* <span data-ttu-id="1f138-1570">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="1f138-1570">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="1f138-1571">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="1f138-1571">See #6052</span></span>
* <span data-ttu-id="1f138-1572">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1572">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="1f138-1573">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="1f138-1573">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="1f138-1574">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1f138-1574">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="1f138-1575">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1f138-1575">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="1f138-1576">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="1f138-1576">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="1f138-1577">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1577">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1578">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1578">Role</span></span>
* <span data-ttu-id="1f138-1579">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="1f138-1579">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="1f138-1580">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="1f138-1580">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="1f138-1581">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="1f138-1581">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="1f138-1582">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="1f138-1582">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="1f138-1583">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-1583">Service Bus</span></span>
* <span data-ttu-id="1f138-1584">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="1f138-1584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1585">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1585">VM</span></span>
* <span data-ttu-id="1f138-1586">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="1f138-1586">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="1f138-1587">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1587">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="1f138-1588">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="1f138-1588">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="1f138-1589">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="1f138-1589">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="1f138-1590">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1590">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="1f138-1591">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="1f138-1591">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="1f138-1592">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1592">September 21, 2018</span></span>

<span data-ttu-id="1f138-1593">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="1f138-1593">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1594">ACR</span></span>
* <span data-ttu-id="1f138-1595">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1595">Added ACR Task commands</span></span>
* <span data-ttu-id="1f138-1596">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="1f138-1596">Added quick run command</span></span>
* <span data-ttu-id="1f138-1597">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="1f138-1597">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="1f138-1598">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1598">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="1f138-1599">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="1f138-1599">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="1f138-1600">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="1f138-1600">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1601">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1601">ACS</span></span>
* <span data-ttu-id="1f138-1602">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-1602">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="1f138-1603">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="1f138-1603">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1604">AppService</span></span>

* <span data-ttu-id="1f138-1605">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="1f138-1605">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="1f138-1606">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="1f138-1606">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="1f138-1607">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="1f138-1607">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="1f138-1608">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="1f138-1608">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1609">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1609">Batch</span></span>
* <span data-ttu-id="1f138-1610">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="1f138-1610">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="1f138-1611">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="1f138-1611">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="1f138-1612">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1612">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="1f138-1613">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="1f138-1613">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1f138-1614">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-1614">Batch AI</span></span> 
* <span data-ttu-id="1f138-1615">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1615">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1f138-1616">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-1616">Cognitive Services</span></span>
* <span data-ttu-id="1f138-1617">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="1f138-1617">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="1f138-1618">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="1f138-1618">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="1f138-1619">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="1f138-1619">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="1f138-1620">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1620">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="1f138-1621">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="1f138-1621">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="1f138-1622">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="1f138-1622">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1623">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1623">Container</span></span>
* <span data-ttu-id="1f138-1624">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="1f138-1624">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="1f138-1625">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1625">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="1f138-1626">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="1f138-1626">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="1f138-1627">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-1627">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="1f138-1628">DataLake</span><span class="sxs-lookup"><span data-stu-id="1f138-1628">Datalake</span></span>
* <span data-ttu-id="1f138-1629">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="1f138-1629">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="1f138-1630">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="1f138-1630">Interactive Shell</span></span>
* <span data-ttu-id="1f138-1631">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-1631">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="1f138-1632">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="1f138-1632">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-1633">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1633">IoT</span></span>
* <span data-ttu-id="1f138-1634">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1634">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-1635">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1f138-1635">Key Vault</span></span>
* <span data-ttu-id="1f138-1636">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="1f138-1636">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1637">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1637">Network</span></span>
* <span data-ttu-id="1f138-1638">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1638">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="1f138-1639">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="1f138-1639">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="1f138-1640">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="1f138-1640">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="1f138-1641">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1641">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="1f138-1642">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1642">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="1f138-1643">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1643">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="1f138-1644">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="1f138-1644">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="1f138-1645">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="1f138-1645">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="1f138-1646">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="1f138-1646">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="1f138-1647">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="1f138-1647">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="1f138-1648">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="1f138-1648">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="1f138-1649">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="1f138-1649">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="1f138-1650">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="1f138-1650">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="1f138-1651">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="1f138-1651">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="1f138-1652">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="1f138-1652">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="1f138-1653">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="1f138-1653">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="1f138-1654">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1654">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="1f138-1655">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="1f138-1655">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1656">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-1656">RDBMS</span></span>
* <span data-ttu-id="1f138-1657">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="1f138-1657">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="1f138-1658">Réservation</span><span class="sxs-lookup"><span data-stu-id="1f138-1658">Reservation</span></span>
* <span data-ttu-id="1f138-1659">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="1f138-1659">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="1f138-1660">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="1f138-1660">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="1f138-1661">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="1f138-1661">Manage App</span></span>
* <span data-ttu-id="1f138-1662">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="1f138-1662">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="1f138-1663">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="1f138-1663">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1664">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1664">Role</span></span>
* <span data-ttu-id="1f138-1665">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="1f138-1665">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="1f138-1666">SignalR</span><span class="sxs-lookup"><span data-stu-id="1f138-1666">SignalR</span></span>
* <span data-ttu-id="1f138-1667">Première version</span><span class="sxs-lookup"><span data-stu-id="1f138-1667">First release</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1668">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1668">Storage</span></span>
* <span data-ttu-id="1f138-1669">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="1f138-1669">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="1f138-1670">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="1f138-1670">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1671">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1671">VM</span></span>
* <span data-ttu-id="1f138-1672">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="1f138-1672">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="1f138-1673">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="1f138-1673">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="1f138-1674">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1674">August 28, 2018</span></span>

<span data-ttu-id="1f138-1675">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="1f138-1675">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1676">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1676">Core</span></span>

* <span data-ttu-id="1f138-1677">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="1f138-1677">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="1f138-1678">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1f138-1678">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1679">ACR</span></span>

* <span data-ttu-id="1f138-1680">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-1680">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="1f138-1681">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="1f138-1681">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1682">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1682">ACS</span></span>

* <span data-ttu-id="1f138-1683">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="1f138-1683">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="1f138-1684">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="1f138-1684">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1685">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1685">AppService</span></span>

* <span data-ttu-id="1f138-1686">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="1f138-1686">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="1f138-1687">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="1f138-1687">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="1f138-1688">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1688">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-1689">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-1689">Backup</span></span>

* <span data-ttu-id="1f138-1690">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1690">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="1f138-1691">Service de robot</span><span class="sxs-lookup"><span data-stu-id="1f138-1691">Bot Service</span></span>

* <span data-ttu-id="1f138-1692">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="1f138-1692">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1f138-1693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-1693">Cognitive Services</span></span>

* <span data-ttu-id="1f138-1694">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="1f138-1694">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-1695">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1695">IoT</span></span>

* <span data-ttu-id="1f138-1696">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="1f138-1696">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-1697">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-1697">Monitor</span></span>

* <span data-ttu-id="1f138-1698">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="1f138-1698">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="1f138-1699">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="1f138-1699">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1700">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1700">Network</span></span>

* <span data-ttu-id="1f138-1701">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1701">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1702">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1702">Resource</span></span>

* <span data-ttu-id="1f138-1703">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1703">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1704">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1704">Storage</span></span>

* <span data-ttu-id="1f138-1705">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1705">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1706">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1706">VM</span></span>

* <span data-ttu-id="1f138-1707">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1707">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="1f138-1708">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1708">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="1f138-1709">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1709">Auguest 14, 2018</span></span>

<span data-ttu-id="1f138-1710">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="1f138-1710">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1711">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1711">Core</span></span>

* <span data-ttu-id="1f138-1712">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="1f138-1712">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="1f138-1713">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="1f138-1713">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="1f138-1714">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="1f138-1714">Telemetry</span></span>

* <span data-ttu-id="1f138-1715">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="1f138-1715">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1716">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1716">ACR</span></span>

* <span data-ttu-id="1f138-1717">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-1717">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="1f138-1718">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="1f138-1718">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1719">ACS</span></span>

* <span data-ttu-id="1f138-1720">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-1720">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="1f138-1721">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-1721">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="1f138-1722">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="1f138-1722">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="1f138-1723">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="1f138-1723">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="1f138-1724">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="1f138-1724">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="1f138-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1725">AppService</span></span>

* <span data-ttu-id="1f138-1726">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="1f138-1726">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="1f138-1727">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="1f138-1727">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-1728">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-1728">BatchAI</span></span>

* <span data-ttu-id="1f138-1729">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="1f138-1729">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="1f138-1730">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1730">Container</span></span>

* <span data-ttu-id="1f138-1731">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1731">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="1f138-1732">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-1732">IoT</span></span>

* <span data-ttu-id="1f138-1733">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="1f138-1733">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="1f138-1734">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="1f138-1734">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="1f138-1735">Iot Central</span><span class="sxs-lookup"><span data-stu-id="1f138-1735">Iot Central</span></span>

* <span data-ttu-id="1f138-1736">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="1f138-1736">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-1737">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-1737">KeyVault</span></span>


* <span data-ttu-id="1f138-1738">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="1f138-1738">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="1f138-1739">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1739">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="1f138-1740">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="1f138-1740">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="1f138-1741">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="1f138-1741">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="1f138-1742">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="1f138-1742">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="1f138-1743">Relais</span><span class="sxs-lookup"><span data-stu-id="1f138-1743">Relay</span></span>

* <span data-ttu-id="1f138-1744">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-1744">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1745">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1745">Sql</span></span>

* <span data-ttu-id="1f138-1746">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="1f138-1746">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1747">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1747">Storage</span></span>

* <span data-ttu-id="1f138-1748">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="1f138-1748">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="1f138-1749">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="1f138-1749">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="1f138-1750">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="1f138-1750">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="1f138-1751">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="1f138-1751">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="1f138-1752">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1752">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1753">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1753">VM</span></span>

* <span data-ttu-id="1f138-1754">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="1f138-1754">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="1f138-1755">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1755">July 31, 2018</span></span>

<span data-ttu-id="1f138-1756">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="1f138-1756">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1757">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1757">ACR</span></span>

* <span data-ttu-id="1f138-1758">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="1f138-1758">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="1f138-1759">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="1f138-1759">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1760">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1760">ACS</span></span>

* <span data-ttu-id="1f138-1761">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="1f138-1761">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1762">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1762">Batch</span></span>

* <span data-ttu-id="1f138-1763">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1f138-1763">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1764">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1764">Container</span></span>

* <span data-ttu-id="1f138-1765">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="1f138-1765">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1766">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1766">Network</span></span>

* <span data-ttu-id="1f138-1767">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1f138-1767">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="1f138-1768">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1768">Resource</span></span>

* <span data-ttu-id="1f138-1769">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-1769">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="1f138-1770">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-1770">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1771">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1771">Role</span></span>

* <span data-ttu-id="1f138-1772">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="1f138-1772">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="1f138-1773">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-1773">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="1f138-1774">Recherche</span><span class="sxs-lookup"><span data-stu-id="1f138-1774">Search</span></span>

* <span data-ttu-id="1f138-1775">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="1f138-1775">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="1f138-1776">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-1776">Service Bus</span></span>

* <span data-ttu-id="1f138-1777">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="1f138-1777">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="1f138-1778">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1778">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="1f138-1779">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="1f138-1779">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="1f138-1780">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="1f138-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1781">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1781">Storage</span></span>

* <span data-ttu-id="1f138-1782">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="1f138-1782">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="1f138-1783">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1783">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1784">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1784">VM</span></span>

* <span data-ttu-id="1f138-1785">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1785">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="1f138-1786">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="1f138-1786">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="1f138-1787">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="1f138-1787">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="1f138-1788">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="1f138-1788">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="1f138-1789">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1789">July 18, 2018</span></span>

<span data-ttu-id="1f138-1790">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="1f138-1790">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1791">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1791">Core</span></span>

* <span data-ttu-id="1f138-1792">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-1792">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="1f138-1793">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="1f138-1793">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="1f138-1794">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="1f138-1794">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1795">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1795">ACR</span></span>

* <span data-ttu-id="1f138-1796">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="1f138-1796">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="1f138-1797">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="1f138-1797">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="1f138-1798">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="1f138-1798">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="1f138-1799">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="1f138-1799">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1800">ACS</span></span>

* <span data-ttu-id="1f138-1801">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="1f138-1801">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1802">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1802">AppService</span></span>

* <span data-ttu-id="1f138-1803">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="1f138-1803">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1804">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1804">Batch</span></span>

* <span data-ttu-id="1f138-1805">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1f138-1805">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="1f138-1806">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-1806">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1f138-1807">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-1807">Batch AI</span></span>

* <span data-ttu-id="1f138-1808">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="1f138-1808">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1809">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1809">Container</span></span>

* <span data-ttu-id="1f138-1810">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="1f138-1810">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="1f138-1811">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="1f138-1811">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1812">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1812">Network</span></span>

* <span data-ttu-id="1f138-1813">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1813">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="1f138-1814">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1814">Added `network nic wait`</span></span>
* <span data-ttu-id="1f138-1815">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1815">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="1f138-1816">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1816">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="1f138-1817">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1817">Resource</span></span>

* <span data-ttu-id="1f138-1818">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-1818">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="1f138-1819">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-1819">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="1f138-1820">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1820">Added `deployment wait` command</span></span>
* <span data-ttu-id="1f138-1821">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="1f138-1821">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1822">SQL</span></span>

* <span data-ttu-id="1f138-1823">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1823">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="1f138-1824">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="1f138-1824">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="1f138-1825">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="1f138-1825">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1826">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1826">Storage</span></span>

* <span data-ttu-id="1f138-1827">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="1f138-1827">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1828">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1828">VM</span></span>

* <span data-ttu-id="1f138-1829">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-1829">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="1f138-1830">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="1f138-1830">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="1f138-1831">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="1f138-1831">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="1f138-1832">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1832">July 3, 2018</span></span>

<span data-ttu-id="1f138-1833">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="1f138-1833">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-1834">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-1834">AKS</span></span>

* <span data-ttu-id="1f138-1835">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1835">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="1f138-1836">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1836">July 3, 2018</span></span>

<span data-ttu-id="1f138-1837">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="1f138-1837">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1838">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1838">Core</span></span>

* <span data-ttu-id="1f138-1839">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1839">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1840">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1840">ACR</span></span>

* <span data-ttu-id="1f138-1841">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="1f138-1841">Added polling build status</span></span>
* <span data-ttu-id="1f138-1842">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-1842">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="1f138-1843">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="1f138-1843">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1844">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1844">ACS</span></span>

* <span data-ttu-id="1f138-1845">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-1845">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="1f138-1846">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-1846">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="1f138-1847">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1847">Updated options for `aks browse` command.</span></span> <span data-ttu-id="1f138-1848">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="1f138-1848">Added `--listen-port` support</span></span>
* <span data-ttu-id="1f138-1849">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1849">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="1f138-1850">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="1f138-1850">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="1f138-1851">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="1f138-1851">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1852">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1852">AppService</span></span>

* <span data-ttu-id="1f138-1853">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="1f138-1853">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="1f138-1854">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="1f138-1854">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-1855">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-1855">Backup</span></span>

* <span data-ttu-id="1f138-1856">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="1f138-1856">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-1857">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-1857">BatchAI</span></span>

* <span data-ttu-id="1f138-1858">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="1f138-1858">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="1f138-1859">Cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-1859">Cloud</span></span>

* <span data-ttu-id="1f138-1860">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-1860">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="1f138-1861">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-1861">Container</span></span>

* <span data-ttu-id="1f138-1862">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="1f138-1862">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="1f138-1863">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="1f138-1863">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="1f138-1864">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="1f138-1864">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-1865">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-1865">Extension</span></span>

* <span data-ttu-id="1f138-1866">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="1f138-1866">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1867">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1867">Network</span></span>

* <span data-ttu-id="1f138-1868">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="1f138-1868">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-1869">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1f138-1869">Rdbms</span></span>

* <span data-ttu-id="1f138-1870">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-1870">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-1871">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-1871">Resource</span></span>

* <span data-ttu-id="1f138-1872">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="1f138-1872">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1873">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1873">VM</span></span>

* <span data-ttu-id="1f138-1874">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="1f138-1874">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="1f138-1875">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1875">June 25, 2018</span></span>

<span data-ttu-id="1f138-1876">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="1f138-1876">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="1f138-1877">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-1877">CLI</span></span>

* <span data-ttu-id="1f138-1878">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="1f138-1878">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="1f138-1879">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1879">June 19, 2018</span></span>

<span data-ttu-id="1f138-1880">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="1f138-1880">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1881">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1881">Core</span></span>

* <span data-ttu-id="1f138-1882">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-1882">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1883">ACR</span></span>

* <span data-ttu-id="1f138-1884">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="1f138-1884">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="1f138-1885">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="1f138-1885">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1886">ACS</span></span>

* <span data-ttu-id="1f138-1887">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1887">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="1f138-1888">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1888">Added `--update` support</span></span>
* <span data-ttu-id="1f138-1889">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="1f138-1889">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="1f138-1890">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="1f138-1890">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="1f138-1891">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="1f138-1891">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="1f138-1892">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="1f138-1892">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="1f138-1893">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1f138-1893">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="1f138-1894">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1f138-1894">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1895">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1895">AppService</span></span>

* <span data-ttu-id="1f138-1896">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="1f138-1896">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="1f138-1897">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="1f138-1897">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1898">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1898">Batch</span></span>

* <span data-ttu-id="1f138-1899">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="1f138-1899">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1f138-1900">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-1900">Batch AI</span></span>

* <span data-ttu-id="1f138-1901">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="1f138-1901">Added support for workspaces.</span></span> <span data-ttu-id="1f138-1902">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="1f138-1902">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="1f138-1903">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="1f138-1903">Added support for experiments.</span></span> <span data-ttu-id="1f138-1904">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="1f138-1904">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="1f138-1905">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="1f138-1905">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="1f138-1906">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1906">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="1f138-1907">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="1f138-1907">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="1f138-1908">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="1f138-1908">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="1f138-1909">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="1f138-1909">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="1f138-1910">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="1f138-1910">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="1f138-1911">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1911">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="1f138-1912">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="1f138-1912">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="1f138-1913">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1913">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="1f138-1914">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="1f138-1914">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="1f138-1915">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="1f138-1915">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="1f138-1916">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="1f138-1916">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="1f138-1917">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1917">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="1f138-1918">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="1f138-1918">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="1f138-1919">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="1f138-1919">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="1f138-1920">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="1f138-1920">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1f138-1921">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="1f138-1921">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1f138-1922">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="1f138-1922">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="1f138-1923">Cartes</span><span class="sxs-lookup"><span data-stu-id="1f138-1923">Maps</span></span>

* <span data-ttu-id="1f138-1924">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="1f138-1924">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1925">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1925">Network</span></span>

* <span data-ttu-id="1f138-1926">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="1f138-1926">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="1f138-1927">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="1f138-1927">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="1f138-1928">#6502</span><span class="sxs-lookup"><span data-stu-id="1f138-1928">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="1f138-1929">Réservations</span><span class="sxs-lookup"><span data-stu-id="1f138-1929">Reservations</span></span>

* <span data-ttu-id="1f138-1930">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="1f138-1930">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="1f138-1931">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="1f138-1931">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="1f138-1932">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="1f138-1932">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="1f138-1933">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="1f138-1933">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="1f138-1934">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="1f138-1934">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="1f138-1935">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="1f138-1935">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="1f138-1936">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-1936">Role</span></span>

* <span data-ttu-id="1f138-1937">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="1f138-1937">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1938">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1938">SQL</span></span>

* <span data-ttu-id="1f138-1939">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-1939">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-1940">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1940">Storage</span></span>

* <span data-ttu-id="1f138-1941">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="1f138-1941">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1942">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1942">VM</span></span>

* <span data-ttu-id="1f138-1943">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1943">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="1f138-1944">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="1f138-1944">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="1f138-1945">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="1f138-1945">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1f138-1946">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1946">June 13, 2018</span></span>

<span data-ttu-id="1f138-1947">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="1f138-1947">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1948">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1948">Core</span></span>

* <span data-ttu-id="1f138-1949">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1949">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1f138-1950">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1950">June 13, 2018</span></span>

<span data-ttu-id="1f138-1951">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="1f138-1951">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-1952">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-1952">AKS</span></span>

* <span data-ttu-id="1f138-1953">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1953">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="1f138-1954">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="1f138-1954">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="1f138-1955">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1955">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="1f138-1956">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1956">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="1f138-1957">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1957">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-1958">AppService</span></span>

* <span data-ttu-id="1f138-1959">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="1f138-1959">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1f138-1960">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1960">June 5, 2018</span></span>

<span data-ttu-id="1f138-1961">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="1f138-1961">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-1962">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-1962">Interactive</span></span>

* <span data-ttu-id="1f138-1963">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="1f138-1963">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1f138-1964">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1964">June 5, 2018</span></span>

<span data-ttu-id="1f138-1965">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="1f138-1965">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1966">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1966">Core</span></span>

* <span data-ttu-id="1f138-1967">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="1f138-1967">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="1f138-1968">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="1f138-1968">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-1969">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-1969">ACR</span></span>

* <span data-ttu-id="1f138-1970">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="1f138-1970">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="1f138-1971">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="1f138-1971">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="1f138-1972">AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-1972">AKS</span></span>

* <span data-ttu-id="1f138-1973">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="1f138-1973">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-1974">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-1974">Batch</span></span>

* <span data-ttu-id="1f138-1975">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="1f138-1975">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-1976">IOT</span><span class="sxs-lookup"><span data-stu-id="1f138-1976">IOT</span></span>

* <span data-ttu-id="1f138-1977">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="1f138-1977">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="1f138-1978">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-1978">Network</span></span>

* <span data-ttu-id="1f138-1979">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="1f138-1979">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="1f138-1980">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1f138-1980">Policy Insights</span></span>

* <span data-ttu-id="1f138-1981">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-1981">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="1f138-1982">ARM</span><span class="sxs-lookup"><span data-stu-id="1f138-1982">ARM</span></span>

* <span data-ttu-id="1f138-1983">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="1f138-1983">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-1984">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-1984">SQL</span></span>

* <span data-ttu-id="1f138-1985">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="1f138-1985">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="1f138-1986">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="1f138-1986">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="1f138-1987">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-1987">Storage</span></span>

* <span data-ttu-id="1f138-1988">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="1f138-1988">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-1989">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-1989">VM</span></span>

* <span data-ttu-id="1f138-1990">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="1f138-1990">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="1f138-1991">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1991">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="1f138-1992">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="1f138-1992">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="1f138-1993">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-1993">May 22, 2018</span></span>

<span data-ttu-id="1f138-1994">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="1f138-1994">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="1f138-1995">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-1995">Core</span></span>

* <span data-ttu-id="1f138-1996">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="1f138-1996">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-1997">ACS</span></span>

* <span data-ttu-id="1f138-1998">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="1f138-1998">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="1f138-1999">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-1999">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2000">AppService</span></span>

* <span data-ttu-id="1f138-2001">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="1f138-2001">Improved generic update commands</span></span>
* <span data-ttu-id="1f138-2002">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="1f138-2002">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2003">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2003">Container</span></span>

* <span data-ttu-id="1f138-2004">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="1f138-2004">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="1f138-2005">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2005">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2006">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2006">Extension</span></span>

* <span data-ttu-id="1f138-2007">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="1f138-2007">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2008">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2008">Interactive</span></span>

* <span data-ttu-id="1f138-2009">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="1f138-2009">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="1f138-2010">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="1f138-2010">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-2011">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-2011">KeyVault</span></span>

* <span data-ttu-id="1f138-2012">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="1f138-2012">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2013">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2013">Network</span></span>

* <span data-ttu-id="1f138-2014">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="1f138-2014">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="1f138-2015">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="1f138-2015">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2016">SQL</span></span>

* <span data-ttu-id="1f138-2017">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="1f138-2017">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="1f138-2018">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="1f138-2018">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="1f138-2019">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="1f138-2019">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="1f138-2020">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="1f138-2020">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="1f138-2021">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="1f138-2021">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="1f138-2022">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2022">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="1f138-2023">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="1f138-2023">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="1f138-2024">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2024">`edition`.</span></span> <span data-ttu-id="1f138-2025">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="1f138-2025">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="1f138-2026">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2026">`elasticPoolName`.</span></span> <span data-ttu-id="1f138-2027">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="1f138-2027">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="1f138-2028">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="1f138-2028">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="1f138-2029">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2029">`edition`.</span></span> <span data-ttu-id="1f138-2030">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="1f138-2030">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="1f138-2031">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2031">`dtu`.</span></span> <span data-ttu-id="1f138-2032">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="1f138-2032">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="1f138-2033">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2033">`databaseDtuMin`.</span></span> <span data-ttu-id="1f138-2034">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="1f138-2034">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="1f138-2035">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2035">`databaseDtuMax`.</span></span> <span data-ttu-id="1f138-2036">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="1f138-2036">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="1f138-2037">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="1f138-2037">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="1f138-2038">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="1f138-2038">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2039">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2039">Storage</span></span>

* <span data-ttu-id="1f138-2040">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-2040">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="1f138-2041">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="1f138-2041">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2042">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2042">VM</span></span>

* <span data-ttu-id="1f138-2043">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2043">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="1f138-2044">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="1f138-2044">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="1f138-2045">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="1f138-2045">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="1f138-2046">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="1f138-2046">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="1f138-2047">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2047">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="1f138-2048">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2048">May 7, 2018</span></span>

<span data-ttu-id="1f138-2049">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="1f138-2049">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2050">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2050">Core</span></span>

* <span data-ttu-id="1f138-2051">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="1f138-2051">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="1f138-2052">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="1f138-2052">Added limited support for positional arguments</span></span>
* <span data-ttu-id="1f138-2053">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2053">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="1f138-2054">#5591</span><span class="sxs-lookup"><span data-stu-id="1f138-2054">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="1f138-2055">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2055">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="1f138-2056">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="1f138-2056">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="1f138-2057">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-2057">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="1f138-2058">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="1f138-2058">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="1f138-2059">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2059">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2060">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2060">ACR</span></span>

* <span data-ttu-id="1f138-2061">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2061">Added ACR Build commands</span></span>
* <span data-ttu-id="1f138-2062">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="1f138-2062">Improved resource not found error messages</span></span>
* <span data-ttu-id="1f138-2063">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2063">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="1f138-2064">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="1f138-2064">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="1f138-2065">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="1f138-2065">Improved repository commands error messages</span></span>
* <span data-ttu-id="1f138-2066">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="1f138-2066">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2067">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2067">ACS</span></span>

* <span data-ttu-id="1f138-2068">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2068">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="1f138-2069">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="1f138-2069">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="1f138-2070">AMS</span><span class="sxs-lookup"><span data-stu-id="1f138-2070">AMS</span></span>

* <span data-ttu-id="1f138-2071">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="1f138-2071">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2072">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2072">Appservice</span></span>

* <span data-ttu-id="1f138-2073">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="1f138-2073">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="1f138-2074">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2074">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="1f138-2075">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="1f138-2075">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="1f138-2076">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2076">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1f138-2077">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-2077">Batch AI</span></span>

* <span data-ttu-id="1f138-2078">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="1f138-2078">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1f138-2079">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-2079">Cognitive Services</span></span>

* <span data-ttu-id="1f138-2080">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="1f138-2080">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-2081">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2081">Consumption</span></span>

* <span data-ttu-id="1f138-2082">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="1f138-2082">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2083">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2083">Container</span></span>

* <span data-ttu-id="1f138-2084">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="1f138-2084">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1f138-2085">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-2085">Cosmos DB</span></span>

* <span data-ttu-id="1f138-2086">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1f138-2086">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="1f138-2087">DMS</span><span class="sxs-lookup"><span data-stu-id="1f138-2087">DMS</span></span>

* <span data-ttu-id="1f138-2088">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="1f138-2088">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2089">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2089">Extension</span></span>

* <span data-ttu-id="1f138-2090">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="1f138-2090">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2091">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2091">Interactive</span></span>

* <span data-ttu-id="1f138-2092">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="1f138-2092">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="1f138-2093">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="1f138-2093">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="1f138-2094">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="1f138-2094">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="1f138-2095">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-2095">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="1f138-2096">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-2096">Lab</span></span>

* <span data-ttu-id="1f138-2097">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="1f138-2097">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2098">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2098">Network</span></span>

* <span data-ttu-id="1f138-2099">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="1f138-2099">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="1f138-2100">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2100">Profile</span></span>

* <span data-ttu-id="1f138-2101">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2101">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="1f138-2102">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="1f138-2102">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="1f138-2103">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="1f138-2103">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="1f138-2104">Redis</span><span class="sxs-lookup"><span data-stu-id="1f138-2104">Redis</span></span>

* <span data-ttu-id="1f138-2105">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2105">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="1f138-2106">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="1f138-2106">Deprecated `redis list-all`.</span></span> <span data-ttu-id="1f138-2107">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2107">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="1f138-2108">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="1f138-2108">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="1f138-2109">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-2109">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="1f138-2110">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2110">Role</span></span>

* <span data-ttu-id="1f138-2111">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="1f138-2111">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2112">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2112">Storage</span></span>

* <span data-ttu-id="1f138-2113">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="1f138-2113">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="1f138-2114">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="1f138-2114">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="1f138-2115">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="1f138-2115">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="1f138-2116">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="1f138-2116">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="1f138-2117">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2117">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2118">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2118">VM</span></span>

* <span data-ttu-id="1f138-2119">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="1f138-2119">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="1f138-2120">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1f138-2120">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="1f138-2121">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="1f138-2121">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="1f138-2122">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="1f138-2122">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="1f138-2123">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="1f138-2123">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="1f138-2124">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="1f138-2124">Added write accelerator support</span></span>
* <span data-ttu-id="1f138-2125">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1f138-2125">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="1f138-2126">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2126">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="1f138-2127">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="1f138-2127">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="1f138-2128">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2128">April 10, 2018</span></span>

<span data-ttu-id="1f138-2129">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="1f138-2129">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2130">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2130">ACR</span></span>

* <span data-ttu-id="1f138-2131">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="1f138-2131">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2132">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2132">ACS</span></span>

* <span data-ttu-id="1f138-2133">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="1f138-2133">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2134">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2134">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="1f138-2136">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="1f138-2136">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-2137">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-2137">BatchAI</span></span>

* <span data-ttu-id="1f138-2138">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="1f138-2138">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="1f138-2139">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="1f138-2139">Job level mounting</span></span>
  - <span data-ttu-id="1f138-2140">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="1f138-2140">Environment variables with secret values</span></span>
  - <span data-ttu-id="1f138-2141">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="1f138-2141">Performance counters settings</span></span>
  - <span data-ttu-id="1f138-2142">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="1f138-2142">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="1f138-2143">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="1f138-2143">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="1f138-2144">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="1f138-2144">Usage and limits reporting</span></span>
  - <span data-ttu-id="1f138-2145">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="1f138-2145">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="1f138-2146">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="1f138-2146">Support for custom images</span></span>
  - <span data-ttu-id="1f138-2147">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="1f138-2147">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="1f138-2148">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="1f138-2148">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="1f138-2149">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="1f138-2149">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="1f138-2150">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="1f138-2150">National clouds are supported</span></span>
* <span data-ttu-id="1f138-2151">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="1f138-2151">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="1f138-2152">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="1f138-2152">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="1f138-2153">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-2153">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="1f138-2154">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="1f138-2154">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="1f138-2155">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="1f138-2155">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="1f138-2156">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="1f138-2156">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="1f138-2157">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2157">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="1f138-2158">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="1f138-2158">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="1f138-2159">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="1f138-2159">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="1f138-2160">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2160">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="1f138-2161">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2161">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="1f138-2162">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="1f138-2162">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="1f138-2163">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2163">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="1f138-2164">Facturation</span><span class="sxs-lookup"><span data-stu-id="1f138-2164">Billing</span></span>

* <span data-ttu-id="1f138-2165">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="1f138-2165">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-2166">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2166">Consumption</span></span>

* <span data-ttu-id="1f138-2167">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="1f138-2167">Added `marketplace` commands</span></span>
* <span data-ttu-id="1f138-2168">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="1f138-2168">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="1f138-2169">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="1f138-2169">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="1f138-2170">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="1f138-2170">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="1f138-2171">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="1f138-2171">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="1f138-2172">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="1f138-2172">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2173">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2173">Container</span></span>

* <span data-ttu-id="1f138-2174">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="1f138-2174">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="1f138-2175">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="1f138-2175">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2176">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2176">Extension</span></span>

* <span data-ttu-id="1f138-2177">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="1f138-2177">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2178">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2178">Interactive</span></span>

* <span data-ttu-id="1f138-2179">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="1f138-2179">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="1f138-2180">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2180">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="1f138-2181">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="1f138-2181">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2182">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2182">Network</span></span>

* <span data-ttu-id="1f138-2183">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="1f138-2183">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="1f138-2184">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2184">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="1f138-2185">#4910</span><span class="sxs-lookup"><span data-stu-id="1f138-2185">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="1f138-2186">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="1f138-2186">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="1f138-2187">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="1f138-2187">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="1f138-2188">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2188">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="1f138-2189">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2189">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="1f138-2190">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="1f138-2190">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2191">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2191">Profile</span></span>

* <span data-ttu-id="1f138-2192">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2192">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="1f138-2193">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="1f138-2193">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-2194">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-2194">RDBMS</span></span>

* <span data-ttu-id="1f138-2195">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="1f138-2195">Added `georestore` command</span></span>
* <span data-ttu-id="1f138-2196">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2196">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2197">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2197">Resource</span></span>

* <span data-ttu-id="1f138-2198">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2198">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="1f138-2199">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2199">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2200">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2200">SQL</span></span>

* <span data-ttu-id="1f138-2201">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="1f138-2201">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2202">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2202">Storage</span></span>

* <span data-ttu-id="1f138-2203">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="1f138-2203">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2204">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2204">VM</span></span>

* <span data-ttu-id="1f138-2205">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2205">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="1f138-2206">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="1f138-2206">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="1f138-2208">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2208">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="1f138-2209">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="1f138-2209">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="1f138-2210">#5718</span><span class="sxs-lookup"><span data-stu-id="1f138-2210">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="1f138-2211">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="1f138-2211">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="1f138-2212">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2212">March 27, 2018</span></span>

<span data-ttu-id="1f138-2213">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="1f138-2213">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2214">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2214">Core</span></span>

* <span data-ttu-id="1f138-2215">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="1f138-2215">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2216">ACS</span></span>

* <span data-ttu-id="1f138-2217">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1f138-2217">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2218">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2218">Appservice</span></span>

* <span data-ttu-id="1f138-2219">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2219">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="1f138-2220">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2220">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-2221">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-2221">Backup</span></span>

* <span data-ttu-id="1f138-2222">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="1f138-2222">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="1f138-2223">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-2223">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="1f138-2224">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="1f138-2224">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="1f138-2225">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2225">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2226">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2226">Container</span></span>

* <span data-ttu-id="1f138-2227">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="1f138-2227">Added `container exec` command.</span></span> <span data-ttu-id="1f138-2228">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="1f138-2228">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="1f138-2229">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2229">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2230">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2230">Extension</span></span>

* <span data-ttu-id="1f138-2231">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2231">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="1f138-2232">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="1f138-2232">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="1f138-2233">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2233">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2234">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2234">Interactive</span></span>

* <span data-ttu-id="1f138-2235">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2235">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="1f138-2236">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="1f138-2236">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="1f138-2237">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="1f138-2237">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="1f138-2238">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="1f138-2238">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="1f138-2239">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-2239">Lab</span></span>

* <span data-ttu-id="1f138-2240">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="1f138-2240">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2241">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2241">Monitor</span></span>

* <span data-ttu-id="1f138-2242">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="1f138-2242">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="1f138-2243">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="1f138-2243">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="1f138-2244">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="1f138-2244">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2245">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2245">Network</span></span>

* <span data-ttu-id="1f138-2246">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="1f138-2246">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2247">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2247">Profile</span></span>

* <span data-ttu-id="1f138-2248">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="1f138-2248">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-2249">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-2249">RDBMS</span></span>

* <span data-ttu-id="1f138-2250">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="1f138-2250">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2251">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2251">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="1f138-2253">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2253">Role</span></span>

* <span data-ttu-id="1f138-2254">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2254">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="1f138-2255">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="1f138-2255">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="1f138-2256">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2256">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="1f138-2257">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2257">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="1f138-2258">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="1f138-2258">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2259">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2259">Storage</span></span>

* <span data-ttu-id="1f138-2260">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="1f138-2260">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="1f138-2261">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="1f138-2261">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2262">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2262">VM</span></span>

* <span data-ttu-id="1f138-2263">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="1f138-2263">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="1f138-2264">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2264">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="1f138-2265">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="1f138-2265">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="1f138-2266">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="1f138-2266">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="1f138-2267">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2267">March 13, 2018</span></span>

<span data-ttu-id="1f138-2268">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="1f138-2268">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2269">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2269">ACR</span></span>

* <span data-ttu-id="1f138-2270">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-2270">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="1f138-2271">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="1f138-2271">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="1f138-2272">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="1f138-2272">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2273">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2273">ACS</span></span>

* <span data-ttu-id="1f138-2274">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="1f138-2274">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="1f138-2275">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="1f138-2275">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="1f138-2276">Advisor</span><span class="sxs-lookup"><span data-stu-id="1f138-2276">Advisor</span></span>

* <span data-ttu-id="1f138-2277">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2277">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="1f138-2278">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2278">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="1f138-2279">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="1f138-2279">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="1f138-2280">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2280">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="1f138-2281">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2281">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2282">Appservice</span></span>

* <span data-ttu-id="1f138-2283">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="1f138-2283">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="1f138-2284">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2284">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1f138-2285">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="1f138-2285">Eventhubs</span></span>

* <span data-ttu-id="1f138-2286">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2286">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2287">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2287">Extension</span></span>

* <span data-ttu-id="1f138-2288">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2288">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2289">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2289">Interactive</span></span>

* <span data-ttu-id="1f138-2290">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="1f138-2290">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="1f138-2291">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="1f138-2291">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="1f138-2292">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="1f138-2292">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="1f138-2293">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="1f138-2293">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2294">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2294">Monitor</span></span>

* <span data-ttu-id="1f138-2295">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="1f138-2295">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="1f138-2296">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="1f138-2296">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="1f138-2297">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="1f138-2297">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="1f138-2298">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-2298">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2299">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2299">Network</span></span>

* <span data-ttu-id="1f138-2300">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2300">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="1f138-2301">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="1f138-2301">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="1f138-2302">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="1f138-2302">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="1f138-2303">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="1f138-2303">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2304">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2304">Profile</span></span>

* <span data-ttu-id="1f138-2305">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="1f138-2305">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="1f138-2306">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="1f138-2306">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-2307">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-2307">RDBMS</span></span>

* <span data-ttu-id="1f138-2308">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2308">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="1f138-2309">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1f138-2309">Service Bus</span></span>

* <span data-ttu-id="1f138-2310">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2310">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2311">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2311">Storage</span></span>

* <span data-ttu-id="1f138-2312">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="1f138-2312">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="1f138-2313">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="1f138-2313">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2314">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2314">VM</span></span>

* <span data-ttu-id="1f138-2315">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="1f138-2315">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="1f138-2316">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="1f138-2316">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="1f138-2317">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="1f138-2317">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="1f138-2318">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="1f138-2318">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="1f138-2319">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2319">February 27, 2018</span></span>

<span data-ttu-id="1f138-2320">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="1f138-2320">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2321">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2321">Core</span></span>

* <span data-ttu-id="1f138-2322">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="1f138-2322">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="1f138-2323">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="1f138-2323">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="1f138-2324">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="1f138-2324">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2325">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2325">ACS</span></span>

* <span data-ttu-id="1f138-2326">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2326">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="1f138-2327">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="1f138-2327">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="1f138-2328">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1f138-2328">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="1f138-2329">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="1f138-2329">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2330">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2330">Appservice</span></span>

* <span data-ttu-id="1f138-2331">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="1f138-2331">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="1f138-2332">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="1f138-2332">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1f138-2333">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-2333">Cognitive Services</span></span>

* <span data-ttu-id="1f138-2334">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-2334">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-2335">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2335">Consumption</span></span>

* <span data-ttu-id="1f138-2336">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="1f138-2336">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="1f138-2337">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="1f138-2337">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2338">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2338">Container</span></span>

* <span data-ttu-id="1f138-2339">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="1f138-2339">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2340">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2340">Network</span></span>

* <span data-ttu-id="1f138-2341">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="1f138-2341">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2342">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2342">Resource</span></span>

* <span data-ttu-id="1f138-2343">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="1f138-2343">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="1f138-2344">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2344">Role</span></span>

* <span data-ttu-id="1f138-2345">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="1f138-2345">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2346">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2346">SQL</span></span>

* <span data-ttu-id="1f138-2347">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="1f138-2347">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2348">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2348">Storage</span></span>

* <span data-ttu-id="1f138-2349">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2349">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2350">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2350">VM</span></span>

* <span data-ttu-id="1f138-2351">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="1f138-2351">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="1f138-2352">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2352">February 13, 2018</span></span>

<span data-ttu-id="1f138-2353">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="1f138-2353">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2354">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2354">Core</span></span>

* <span data-ttu-id="1f138-2355">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="1f138-2355">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2356">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2356">ACS</span></span>

* <span data-ttu-id="1f138-2357">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="1f138-2357">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="1f138-2358">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2358">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="1f138-2359">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-2359">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="1f138-2360">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-2360">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="1f138-2361">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="1f138-2361">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="1f138-2362">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="1f138-2362">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="1f138-2363">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-2363">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="1f138-2364">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="1f138-2364">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2365">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2365">Appservice</span></span>

* <span data-ttu-id="1f138-2366">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="1f138-2366">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="1f138-2367">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="1f138-2367">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-2368">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-2368">CDN</span></span>

* <span data-ttu-id="1f138-2369">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2369">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2370">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2370">Container</span></span>

* <span data-ttu-id="1f138-2371">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="1f138-2371">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="1f138-2372">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2372">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-2373">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-2373">CosmosDB</span></span>

* <span data-ttu-id="1f138-2374">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="1f138-2374">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2375">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2375">Extension</span></span>

* <span data-ttu-id="1f138-2376">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2376">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="1f138-2377">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2377">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="1f138-2378">Commentaires</span><span class="sxs-lookup"><span data-stu-id="1f138-2378">Feedback</span></span>

* <span data-ttu-id="1f138-2379">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="1f138-2379">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2380">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2380">Interactive</span></span>

* <span data-ttu-id="1f138-2381">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1f138-2381">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="1f138-2382">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="1f138-2382">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-2383">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2383">IoT</span></span>

* <span data-ttu-id="1f138-2384">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="1f138-2384">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1f138-2385">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="1f138-2385">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1f138-2386">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2386">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="1f138-2387">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="1f138-2387">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2388">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2388">Monitor</span></span>

* <span data-ttu-id="1f138-2389">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2389">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2390">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2390">Network</span></span>

* <span data-ttu-id="1f138-2391">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="1f138-2391">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="1f138-2392">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2392">Profile</span></span>

* <span data-ttu-id="1f138-2393">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="1f138-2393">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2394">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2394">Resource</span></span>

* <span data-ttu-id="1f138-2395">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2395">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="1f138-2396">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2396">Role</span></span>

* <span data-ttu-id="1f138-2397">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2397">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2398">SQL</span></span>

* <span data-ttu-id="1f138-2399">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="1f138-2399">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="1f138-2400">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="1f138-2400">Added `sql db rename`</span></span>
* <span data-ttu-id="1f138-2401">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="1f138-2401">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2402">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2402">Storage</span></span>

* <span data-ttu-id="1f138-2403">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="1f138-2403">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2404">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2404">VM</span></span>

* <span data-ttu-id="1f138-2405">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="1f138-2405">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="1f138-2406">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="1f138-2406">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="1f138-2407">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="1f138-2407">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="1f138-2408">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2408">January 31, 2018</span></span>

<span data-ttu-id="1f138-2409">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="1f138-2409">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2410">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2410">Core</span></span>

* <span data-ttu-id="1f138-2411">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="1f138-2411">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="1f138-2412">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-2412">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="1f138-2413">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="1f138-2413">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="1f138-2414">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="1f138-2414">Use `--verbose` to see</span></span>
* <span data-ttu-id="1f138-2415">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="1f138-2415">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2416">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2416">ACS</span></span>

* <span data-ttu-id="1f138-2417">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="1f138-2417">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="1f138-2418">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="1f138-2418">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2419">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2419">Appservice</span></span>

* <span data-ttu-id="1f138-2420">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="1f138-2420">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="1f138-2421">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="1f138-2421">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-2422">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-2422">CDN</span></span>

* <span data-ttu-id="1f138-2423">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2423">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-2424">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-2424">CosmosDB</span></span>

* <span data-ttu-id="1f138-2425">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="1f138-2425">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2426">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2426">Interactive</span></span>

* <span data-ttu-id="1f138-2427">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="1f138-2427">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2428">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2428">Network</span></span>

* <span data-ttu-id="1f138-2429">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2429">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="1f138-2430">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2430">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="1f138-2431">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2431">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="1f138-2432">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2432">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="1f138-2433">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="1f138-2433">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="1f138-2434">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="1f138-2434">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="1f138-2435">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="1f138-2435">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="1f138-2436">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="1f138-2436">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="1f138-2437">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="1f138-2437">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="1f138-2438">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="1f138-2438">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2439">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2439">Profile</span></span>

* <span data-ttu-id="1f138-2440">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="1f138-2440">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2441">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2441">Resource</span></span>

* <span data-ttu-id="1f138-2442">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="1f138-2442">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2443">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2443">Storage</span></span>

* <span data-ttu-id="1f138-2444">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="1f138-2444">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="1f138-2445">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="1f138-2445">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="1f138-2446">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-2446">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="1f138-2447">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2447">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="1f138-2448">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="1f138-2448">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2449">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2449">VM</span></span>

* <span data-ttu-id="1f138-2450">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="1f138-2450">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="1f138-2451">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="1f138-2451">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="1f138-2452">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="1f138-2452">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="1f138-2453">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2453">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="1f138-2454">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="1f138-2454">January 17, 2018</span></span>

<span data-ttu-id="1f138-2455">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="1f138-2455">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2456">ACR</span></span>

* <span data-ttu-id="1f138-2457">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-2457">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="1f138-2458">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="1f138-2458">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2459">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2459">ACS</span></span>

* <span data-ttu-id="1f138-2460">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1f138-2460">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="1f138-2461">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="1f138-2461">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2462">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2462">Appservice</span></span>

* <span data-ttu-id="1f138-2463">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="1f138-2463">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="1f138-2464">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="1f138-2464">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="1f138-2465">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="1f138-2465">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-2466">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-2466">Backup</span></span>

* <span data-ttu-id="1f138-2467">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="1f138-2467">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="1f138-2468">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="1f138-2468">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="1f138-2469">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-2469">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="1f138-2470">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="1f138-2470">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="1f138-2471">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2471">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2472">Batch</span></span>

* <span data-ttu-id="1f138-2473">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="1f138-2473">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="1f138-2474">Cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-2474">Cloud</span></span>

* <span data-ttu-id="1f138-2475">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-2475">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-2476">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2476">Consumption</span></span>

* <span data-ttu-id="1f138-2477">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="1f138-2477">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="1f138-2478">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1f138-2478">Event Grid</span></span>

* <span data-ttu-id="1f138-2479">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="1f138-2479">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1f138-2480">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="1f138-2480">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1f138-2481">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="1f138-2481">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="1f138-2482">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="1f138-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="1f138-2483">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2483">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="1f138-2484">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2484">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="1f138-2485">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="1f138-2485">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="1f138-2486">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="1f138-2486">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2487">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2487">Interactive</span></span>

* <span data-ttu-id="1f138-2488">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="1f138-2488">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="1f138-2489">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="1f138-2489">Fixed errors on startup</span></span>
* <span data-ttu-id="1f138-2490">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="1f138-2490">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-2491">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2491">IoT</span></span>

* <span data-ttu-id="1f138-2492">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="1f138-2492">Added support for device provisioning service</span></span>
* <span data-ttu-id="1f138-2493">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-2493">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="1f138-2494">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2494">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2495">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2495">Monitor</span></span>

* <span data-ttu-id="1f138-2496">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="1f138-2496">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="1f138-2497">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2497">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="1f138-2498">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="1f138-2498">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2499">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2499">Network</span></span>

* <span data-ttu-id="1f138-2500">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2500">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="1f138-2501">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2501">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2502">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2502">Profile</span></span>

* <span data-ttu-id="1f138-2503">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2503">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="1f138-2504">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2504">Role</span></span>

* <span data-ttu-id="1f138-2505">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="1f138-2505">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1f138-2506">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1f138-2506">Service Fabric</span></span>

* <span data-ttu-id="1f138-2507">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="1f138-2507">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="1f138-2508">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-2508">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2509">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2509">VM</span></span>

* <span data-ttu-id="1f138-2510">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="1f138-2510">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="1f138-2511">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="1f138-2511">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="1f138-2512">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="1f138-2512">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="1f138-2513">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="1f138-2513">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="1f138-2514">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="1f138-2514">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="1f138-2515">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2515">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1f138-2516">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2516">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="1f138-2517">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="1f138-2517">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="1f138-2518">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2518">December 19, 2017</span></span>

<span data-ttu-id="1f138-2519">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="1f138-2519">Version 2.0.23</span></span>

* <span data-ttu-id="1f138-2520">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2520">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2521">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2521">Container</span></span>

* <span data-ttu-id="1f138-2522">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2522">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2523">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2523">Network</span></span>

* <span data-ttu-id="1f138-2524">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2524">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="1f138-2525">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2525">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2526">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2526">Storage</span></span>

* <span data-ttu-id="1f138-2527">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="1f138-2527">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2528">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2528">VM</span></span>

* <span data-ttu-id="1f138-2529">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="1f138-2529">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="1f138-2530">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2530">December 5, 2017</span></span>

<span data-ttu-id="1f138-2531">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="1f138-2531">Version 2.0.22</span></span>

* <span data-ttu-id="1f138-2532">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2532">Removed `az component` commands.</span></span> <span data-ttu-id="1f138-2533">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="1f138-2533">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2534">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2534">Core</span></span>
* <span data-ttu-id="1f138-2535">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="1f138-2535">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="1f138-2536">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="1f138-2536">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2537">ACS</span></span>

* <span data-ttu-id="1f138-2538">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="1f138-2538">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="1f138-2539">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2539">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="1f138-2540">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="1f138-2540">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="1f138-2541">Advisor</span><span class="sxs-lookup"><span data-stu-id="1f138-2541">Advisor</span></span>

* <span data-ttu-id="1f138-2542">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2542">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2543">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2543">Appservice</span></span>

* <span data-ttu-id="1f138-2544">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="1f138-2544">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="1f138-2545">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="1f138-2545">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="1f138-2546">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="1f138-2546">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="1f138-2547">Consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2547">Consumption</span></span>

* <span data-ttu-id="1f138-2548">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="1f138-2548">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2549">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2549">Container</span></span>

* <span data-ttu-id="1f138-2550">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2550">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2551">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2551">Monitor</span></span>

* <span data-ttu-id="1f138-2552">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="1f138-2552">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2553">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2553">Resource</span></span>

* <span data-ttu-id="1f138-2554">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2554">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="1f138-2555">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-2555">Role</span></span>

* <span data-ttu-id="1f138-2556">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2556">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="1f138-2557">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="1f138-2557">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="1f138-2558">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1f138-2558">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2559">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2559">SQL</span></span>

* <span data-ttu-id="1f138-2560">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="1f138-2560">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="1f138-2561">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2561">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2562">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2562">VM</span></span>

* <span data-ttu-id="1f138-2563">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="1f138-2563">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="1f138-2564">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2564">November 14, 2017</span></span>

<span data-ttu-id="1f138-2565">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1f138-2565">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2566">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2566">ACR</span></span>

* <span data-ttu-id="1f138-2567">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="1f138-2567">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1f138-2568">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2568">ACS</span></span>

* <span data-ttu-id="1f138-2569">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="1f138-2569">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1f138-2570">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2570">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="1f138-2571">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="1f138-2571">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="1f138-2572">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-2572">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1f138-2573">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1f138-2573">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2574">Appservice</span></span>

* <span data-ttu-id="1f138-2575">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="1f138-2575">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1f138-2576">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1f138-2576">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="1f138-2577">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1f138-2577">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="1f138-2578">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="1f138-2578">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="1f138-2579">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="1f138-2579">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1f138-2580">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="1f138-2580">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-2581">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2581">Batch</span></span>

* <span data-ttu-id="1f138-2582">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="1f138-2582">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-2583">Batchai</span><span class="sxs-lookup"><span data-stu-id="1f138-2583">Batchai</span></span>

* <span data-ttu-id="1f138-2584">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2584">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1f138-2585">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2585">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1f138-2586">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="1f138-2586">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="1f138-2587">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2587">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1f138-2588">Cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-2588">Cloud</span></span>

* <span data-ttu-id="1f138-2589">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="1f138-2589">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2590">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2590">Container</span></span>

* <span data-ttu-id="1f138-2591">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="1f138-2591">Added support to open multiple ports</span></span>
* <span data-ttu-id="1f138-2592">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1f138-2592">Added container group restart policy</span></span>
* <span data-ttu-id="1f138-2593">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="1f138-2593">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1f138-2594">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="1f138-2594">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1f138-2595">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-2595">Data Lake Analytics</span></span>

* <span data-ttu-id="1f138-2596">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="1f138-2596">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1f138-2597">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-2597">Data Lake Store</span></span>

* <span data-ttu-id="1f138-2598">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="1f138-2598">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2599">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2599">Extension</span></span>

* <span data-ttu-id="1f138-2600">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="1f138-2600">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1f138-2601">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="1f138-2601">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-2602">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2602">IoT</span></span>

* <span data-ttu-id="1f138-2603">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="1f138-2603">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2604">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2604">Monitor</span></span>

* <span data-ttu-id="1f138-2605">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="1f138-2605">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2606">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2606">Network</span></span>

* <span data-ttu-id="1f138-2607">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="1f138-2607">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1f138-2608">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2608">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="1f138-2609">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="1f138-2609">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1f138-2610">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="1f138-2610">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="1f138-2611">Réservations</span><span class="sxs-lookup"><span data-stu-id="1f138-2611">Reservations</span></span>

* <span data-ttu-id="1f138-2612">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2612">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2613">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2613">Resource</span></span>

* <span data-ttu-id="1f138-2614">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-2614">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2615">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2615">SQL</span></span>

* <span data-ttu-id="1f138-2616">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2616">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2617">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2617">Storage</span></span>

* <span data-ttu-id="1f138-2618">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2618">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1f138-2619">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="1f138-2619">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1f138-2620">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="1f138-2620">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="1f138-2621">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="1f138-2621">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="1f138-2622">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2622">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="1f138-2623">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="1f138-2623">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="1f138-2624">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2624">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2625">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2625">VM</span></span>

* <span data-ttu-id="1f138-2626">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="1f138-2626">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1f138-2627">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="1f138-2627">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1f138-2628">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="1f138-2628">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1f138-2629">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="1f138-2629">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="1f138-2630">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1f138-2630">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="1f138-2631">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2631">October 24, 2017</span></span>

<span data-ttu-id="1f138-2632">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1f138-2632">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2633">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2633">Core</span></span>

* <span data-ttu-id="1f138-2634">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="1f138-2634">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2635">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2635">ACR</span></span>

* <span data-ttu-id="1f138-2636">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="1f138-2636">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1f138-2637">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="1f138-2637">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1f138-2638">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="1f138-2638">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2639">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2639">ACS</span></span>

* <span data-ttu-id="1f138-2640">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="1f138-2640">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1f138-2641">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1f138-2641">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2642">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2642">Appservice</span></span>

* <span data-ttu-id="1f138-2643">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="1f138-2643">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1f138-2644">Composant</span><span class="sxs-lookup"><span data-stu-id="1f138-2644">Component</span></span>

* <span data-ttu-id="1f138-2645">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="1f138-2645">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2646">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2646">Monitor</span></span>

* <span data-ttu-id="1f138-2647">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="1f138-2647">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2648">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2648">Resource</span></span>

* <span data-ttu-id="1f138-2649">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="1f138-2649">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="1f138-2650">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="1f138-2650">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2651">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2651">VM</span></span>

* <span data-ttu-id="1f138-2652">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2652">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="1f138-2653">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2653">October 9, 2017</span></span>

<span data-ttu-id="1f138-2654">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1f138-2654">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2655">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2655">Core</span></span>

* <span data-ttu-id="1f138-2656">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1f138-2656">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2657">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2657">Appservice</span></span>

* <span data-ttu-id="1f138-2658">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2658">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-2659">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2659">Batch</span></span>

* <span data-ttu-id="1f138-2660">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="1f138-2660">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1f138-2661">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="1f138-2661">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1f138-2662">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2662">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1f138-2663">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="1f138-2663">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1f138-2664">Batchai</span><span class="sxs-lookup"><span data-stu-id="1f138-2664">Batchai</span></span>

* <span data-ttu-id="1f138-2665">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="1f138-2665">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-2666">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-2666">Keyvault</span></span>

* <span data-ttu-id="1f138-2667">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1f138-2667">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1f138-2668">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1f138-2668">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1f138-2669">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2669">Network</span></span>

* <span data-ttu-id="1f138-2670">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="1f138-2670">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1f138-2671">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="1f138-2671">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2672">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2672">Resource</span></span>

* <span data-ttu-id="1f138-2673">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="1f138-2673">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="1f138-2674">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-2674">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1f138-2675">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="1f138-2675">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1f138-2676">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-2676">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2677">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2677">Sql</span></span>

* <span data-ttu-id="1f138-2678">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="1f138-2678">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1f138-2679">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="1f138-2679">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1f138-2680">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="1f138-2680">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2681">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2681">Storage</span></span>

* <span data-ttu-id="1f138-2682">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="1f138-2682">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2683">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2683">Vm</span></span>

* <span data-ttu-id="1f138-2684">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="1f138-2684">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1f138-2685">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2685">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="1f138-2686">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1f138-2686">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="1f138-2687">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2687">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="1f138-2688">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2688">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="1f138-2689">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2689">September 22, 2017</span></span>

<span data-ttu-id="1f138-2690">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="1f138-2690">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2691">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2691">Resource</span></span>

* <span data-ttu-id="1f138-2692">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="1f138-2692">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1f138-2693">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="1f138-2693">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1f138-2694">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2694">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="1f138-2695">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="1f138-2695">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2696">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2696">Network</span></span>

* <span data-ttu-id="1f138-2697">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="1f138-2697">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1f138-2698">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="1f138-2698">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="1f138-2699">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="1f138-2699">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1f138-2700">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2700">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="1f138-2701">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2701">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1f138-2702">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2702">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="1f138-2703">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2703">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2704">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2704">Storage</span></span>

* <span data-ttu-id="1f138-2705">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1f138-2705">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1f138-2706">Événement</span><span class="sxs-lookup"><span data-stu-id="1f138-2706">Eventgrid</span></span>

* <span data-ttu-id="1f138-2707">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="1f138-2707">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2708">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2708">SQL</span></span>

* <span data-ttu-id="1f138-2709">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="1f138-2709">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1f138-2710">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="1f138-2710">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1f138-2711">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2711">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-2712">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-2712">Keyvault</span></span>

* <span data-ttu-id="1f138-2713">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="1f138-2713">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2714">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2714">VM</span></span>

* <span data-ttu-id="1f138-2715">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2715">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="1f138-2716">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="1f138-2716">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1f138-2717">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2717">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="1f138-2718">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="1f138-2718">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="1f138-2719">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="1f138-2719">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="1f138-2720">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1f138-2720">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2721">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2721">ACS</span></span>

* <span data-ttu-id="1f138-2722">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2722">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2723">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2723">Appservice</span></span>

* <span data-ttu-id="1f138-2724">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2724">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1f138-2725">Backup</span><span class="sxs-lookup"><span data-stu-id="1f138-2725">Backup</span></span>

* <span data-ttu-id="1f138-2726">Préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2726">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1f138-2727">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2727">September 11, 2017</span></span>

<span data-ttu-id="1f138-2728">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1f138-2728">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1f138-2729">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2729">Core</span></span>

* <span data-ttu-id="1f138-2730">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="1f138-2730">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1f138-2731">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="1f138-2731">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2732">Acs</span><span class="sxs-lookup"><span data-stu-id="1f138-2732">Acs</span></span>

* <span data-ttu-id="1f138-2733">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="1f138-2733">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1f138-2734">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="1f138-2734">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2735">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2735">Appservice</span></span>

* <span data-ttu-id="1f138-2736">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="1f138-2736">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-2737">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-2737">CDN</span></span>

* <span data-ttu-id="1f138-2738">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2738">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="1f138-2739">Extension</span><span class="sxs-lookup"><span data-stu-id="1f138-2739">Extension</span></span>

* <span data-ttu-id="1f138-2740">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2740">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-2741">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-2741">Keyvault</span></span>

* <span data-ttu-id="1f138-2742">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-2742">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2743">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2743">Network</span></span>

* <span data-ttu-id="1f138-2744">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1f138-2744">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1f138-2745">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2745">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="1f138-2746">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2746">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="1f138-2747">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2747">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1f138-2748">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2748">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-2749">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-2749">Resource</span></span>

* <span data-ttu-id="1f138-2750">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2750">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="1f138-2751">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2751">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="1f138-2752">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="1f138-2752">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1f138-2753">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="1f138-2753">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-2754">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-2754">SQL</span></span>

* <span data-ttu-id="1f138-2755">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-2755">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2756">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2756">VM</span></span>

* <span data-ttu-id="1f138-2757">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="1f138-2757">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1f138-2758">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="1f138-2758">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1f138-2759">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2759">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1f138-2760">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="1f138-2760">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1f138-2761">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="1f138-2761">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1f138-2762">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2762">August 31, 2017</span></span>

<span data-ttu-id="1f138-2763">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1f138-2763">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-2764">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-2764">Keyvault</span></span>

* <span data-ttu-id="1f138-2765">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="1f138-2765">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="1f138-2766">Sf</span><span class="sxs-lookup"><span data-stu-id="1f138-2766">Sf</span></span>

* <span data-ttu-id="1f138-2767">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="1f138-2767">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2768">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2768">Storage</span></span>

* <span data-ttu-id="1f138-2769">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="1f138-2769">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1f138-2770">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="1f138-2770">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1f138-2771">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2771">August 28, 2017</span></span>

<span data-ttu-id="1f138-2772">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1f138-2772">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1f138-2773">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2773">CLI</span></span>

* <span data-ttu-id="1f138-2774">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="1f138-2774">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2775">ACS</span></span>

* <span data-ttu-id="1f138-2776">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="1f138-2776">Corrected preview regions</span></span>
* <span data-ttu-id="1f138-2777">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-2777">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="1f138-2778">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2778">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2779">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2779">Appservice</span></span>

* <span data-ttu-id="1f138-2780">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2780">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="1f138-2781">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-2781">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="1f138-2782">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2782">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="1f138-2783">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="1f138-2783">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1f138-2784">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-2784">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-2785">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2785">IoT</span></span>

* <span data-ttu-id="1f138-2786">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="1f138-2786">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2787">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2787">Network</span></span>

* <span data-ttu-id="1f138-2788">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1f138-2788">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1f138-2789">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2789">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="1f138-2790">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1f138-2790">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1f138-2791">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2791">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1f138-2792">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2792">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2793">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2793">Profile</span></span>

* <span data-ttu-id="1f138-2794">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2794">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1f138-2795">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1f138-2795">Service Fabric</span></span>

* <span data-ttu-id="1f138-2796">Préversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2796">Preview release</span></span>
* <span data-ttu-id="1f138-2797">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2797">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1f138-2798">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="1f138-2798">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1f138-2799">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="1f138-2799">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2800">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2800">Storage</span></span>

* <span data-ttu-id="1f138-2801">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="1f138-2801">Enabled setting blob tier</span></span>
* <span data-ttu-id="1f138-2802">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="1f138-2802">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1f138-2803">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="1f138-2803">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="1f138-2804">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="1f138-2804">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1f138-2805">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2805">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1f138-2806">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="1f138-2806">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2807">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2807">VM</span></span>

* <span data-ttu-id="1f138-2808">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="1f138-2808">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="1f138-2809">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="1f138-2809">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="1f138-2810">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2810">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="1f138-2811">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="1f138-2811">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1f138-2812">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="1f138-2812">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1f138-2813">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2813">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="1f138-2814">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2814">August 15, 2017</span></span>

<span data-ttu-id="1f138-2815">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1f138-2815">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2816">ACS</span></span>

* <span data-ttu-id="1f138-2817">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="1f138-2817">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2818">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2818">Appservice</span></span>

* <span data-ttu-id="1f138-2819">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="1f138-2819">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1f138-2820">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1f138-2820">Event Grid</span></span>

* <span data-ttu-id="1f138-2821">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1f138-2821">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1f138-2822">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2822">August 11, 2017</span></span>

<span data-ttu-id="1f138-2823">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1f138-2823">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2824">ACS</span></span>

* <span data-ttu-id="1f138-2825">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="1f138-2825">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-2826">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2826">Batch</span></span>

* <span data-ttu-id="1f138-2827">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1f138-2827">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1f138-2828">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="1f138-2828">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1f138-2829">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="1f138-2829">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1f138-2830">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="1f138-2830">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1f138-2831">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="1f138-2831">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1f138-2832">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="1f138-2832">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1f138-2833">Composant</span><span class="sxs-lookup"><span data-stu-id="1f138-2833">Component</span></span>

* <span data-ttu-id="1f138-2834">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="1f138-2834">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1f138-2835">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2835">Container</span></span>

* <span data-ttu-id="1f138-2836">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="1f138-2836">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1f138-2837">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-2837">Data Lake Store</span></span>

* <span data-ttu-id="1f138-2838">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="1f138-2838">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1f138-2839">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1f138-2839">Event Grid</span></span>

* <span data-ttu-id="1f138-2840">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1f138-2840">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2841">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2841">Network</span></span>

* <span data-ttu-id="1f138-2842">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="1f138-2842">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="1f138-2843">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="1f138-2843">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="1f138-2844">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="1f138-2844">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1f138-2845">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="1f138-2845">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2846">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2846">Profile</span></span>

* <span data-ttu-id="1f138-2847">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="1f138-2847">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-2848">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-2848">Storage</span></span>

* <span data-ttu-id="1f138-2849">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="1f138-2849">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-2850">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-2850">VM</span></span>

* <span data-ttu-id="1f138-2851">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="1f138-2851">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1f138-2852">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="1f138-2852">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1f138-2853">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="1f138-2853">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1f138-2854">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="1f138-2854">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1f138-2855">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="1f138-2855">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1f138-2856">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-2856">July 28, 2017</span></span>

<span data-ttu-id="1f138-2857">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1f138-2857">Version 2.0.12</span></span>

* <span data-ttu-id="1f138-2858">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="1f138-2858">Added container commands</span></span>
* <span data-ttu-id="1f138-2859">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="1f138-2859">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1f138-2860">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-2860">Core</span></span>

* <span data-ttu-id="1f138-2861">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="1f138-2861">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1f138-2862">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="1f138-2862">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1f138-2863">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1f138-2863">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1f138-2864">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="1f138-2864">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1f138-2865">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="1f138-2865">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1f138-2866">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="1f138-2866">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1f138-2867">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="1f138-2867">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1f138-2868">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="1f138-2868">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1f138-2869">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="1f138-2869">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1f138-2870">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1f138-2870">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1f138-2871">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="1f138-2871">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1f138-2872">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="1f138-2872">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1f138-2873">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-2873">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1f138-2874">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="1f138-2874">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1f138-2875">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1f138-2875">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1f138-2876">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="1f138-2876">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1f138-2877">ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2877">ACR</span></span>

* <span data-ttu-id="1f138-2878">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="1f138-2878">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1f138-2879">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="1f138-2879">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1f138-2880">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="1f138-2880">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1f138-2881">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="1f138-2881">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1f138-2882">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="1f138-2882">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1f138-2883">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="1f138-2883">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-2884">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-2884">ACS</span></span>

* <span data-ttu-id="1f138-2885">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="1f138-2885">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-2886">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-2886">Appservice</span></span>

* <span data-ttu-id="1f138-2887">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="1f138-2887">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1f138-2888">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="1f138-2888">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1f138-2889">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="1f138-2889">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="1f138-2890">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="1f138-2890">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1f138-2891">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="1f138-2891">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1f138-2892">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="1f138-2892">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1f138-2893">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="1f138-2893">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1f138-2894">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="1f138-2894">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1f138-2895">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="1f138-2895">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1f138-2896">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="1f138-2896">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="1f138-2897">Batch</span><span class="sxs-lookup"><span data-stu-id="1f138-2897">Batch</span></span>

* <span data-ttu-id="1f138-2898">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="1f138-2898">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1f138-2899">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="1f138-2899">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="1f138-2900">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="1f138-2900">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="1f138-2901">CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-2901">CDN</span></span>

* <span data-ttu-id="1f138-2902">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="1f138-2902">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="1f138-2903">Cloud</span><span class="sxs-lookup"><span data-stu-id="1f138-2903">Cloud</span></span>

* <span data-ttu-id="1f138-2904">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="1f138-2904">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1f138-2905">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="1f138-2905">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1f138-2906">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="1f138-2906">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1f138-2907">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="1f138-2907">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1f138-2908">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="1f138-2908">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-2909">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-2909">CosmosDB</span></span>

* <span data-ttu-id="1f138-2910">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="1f138-2910">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1f138-2911">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="1f138-2911">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1f138-2912">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-2912">Data Lake Analytics</span></span>

* <span data-ttu-id="1f138-2913">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="1f138-2913">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1f138-2914">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2914">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="1f138-2915">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="1f138-2915">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1f138-2916">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-2916">Data Lake Store</span></span>

* <span data-ttu-id="1f138-2917">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2917">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="1f138-2918">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="1f138-2918">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1f138-2919">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="1f138-2919">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1f138-2920">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-2920">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1f138-2921">Interactive</span><span class="sxs-lookup"><span data-stu-id="1f138-2921">Interactive</span></span>

* <span data-ttu-id="1f138-2922">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="1f138-2922">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1f138-2923">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="1f138-2923">Increased test coverage</span></span>
* <span data-ttu-id="1f138-2924">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="1f138-2924">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1f138-2925">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="1f138-2925">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1f138-2926">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="1f138-2926">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1f138-2927">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="1f138-2927">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1f138-2928">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="1f138-2928">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1f138-2929">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="1f138-2929">Added `--progress` flag</span></span>
* <span data-ttu-id="1f138-2930">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="1f138-2930">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1f138-2931">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="1f138-2931">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1f138-2932">IoT</span><span class="sxs-lookup"><span data-stu-id="1f138-2932">IoT</span></span>

* <span data-ttu-id="1f138-2933">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="1f138-2933">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1f138-2934">(#3934)</span><span class="sxs-lookup"><span data-stu-id="1f138-2934">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1f138-2935">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="1f138-2935">Key vault</span></span>

* <span data-ttu-id="1f138-2936">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="1f138-2936">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="1f138-2937">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1f138-2937">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="1f138-2938">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1f138-2938">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1f138-2939">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1f138-2939">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1f138-2940">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1f138-2940">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="1f138-2941">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="1f138-2941">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1f138-2942">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="1f138-2942">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1f138-2943">(#3307)</span><span class="sxs-lookup"><span data-stu-id="1f138-2943">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1f138-2944">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-2944">Lab</span></span>

* <span data-ttu-id="1f138-2945">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="1f138-2945">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="1f138-2946">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2946">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-2947">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-2947">Monitor</span></span>

* <span data-ttu-id="1f138-2948">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="1f138-2948">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1f138-2949">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="1f138-2949">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="1f138-2950">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="1f138-2950">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="1f138-2951">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="1f138-2951">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="1f138-2952">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="1f138-2952">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="1f138-2953">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="1f138-2953">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="1f138-2954">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="1f138-2954">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1f138-2955">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="1f138-2955">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="1f138-2956">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="1f138-2956">`location` no longer required</span></span>
  * <span data-ttu-id="1f138-2957">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="1f138-2957">Add name and ID support for target</span></span>
  * <span data-ttu-id="1f138-2958">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-2958">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="1f138-2959">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="1f138-2959">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="1f138-2960">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="1f138-2960">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1f138-2961">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="1f138-2961">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1f138-2962">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="1f138-2962">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1f138-2963">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2963">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="1f138-2964">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-2964">Network</span></span>

* <span data-ttu-id="1f138-2965">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="1f138-2965">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1f138-2966">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2966">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="1f138-2967">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="1f138-2967">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1f138-2968">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="1f138-2968">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1f138-2969">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2969">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="1f138-2970">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1f138-2970">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1f138-2971">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="1f138-2971">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="1f138-2972">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="1f138-2972">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="1f138-2973">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="1f138-2973">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1f138-2974">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1f138-2974">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="1f138-2975">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2975">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="1f138-2976">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="1f138-2976">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="1f138-2977">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="1f138-2977">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="1f138-2978">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2978">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="1f138-2979">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2979">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="1f138-2980">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2980">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="1f138-2981">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="1f138-2981">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1f138-2982">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1f138-2982">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="1f138-2983">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2983">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="1f138-2984">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="1f138-2984">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="1f138-2985">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="1f138-2985">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="1f138-2986">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-2986">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1f138-2987">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="1f138-2987">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="1f138-2988">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1f138-2988">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1f138-2989">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1f138-2989">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1f138-2990">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1f138-2990">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1f138-2991">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1f138-2991">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-2992">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-2992">Profile</span></span>

* <span data-ttu-id="1f138-2993">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="1f138-2993">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1f138-2994">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1f138-2994">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1f138-2995">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="1f138-2995">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1f138-2996">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="1f138-2996">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1f138-2997">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="1f138-2997">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1f138-2998">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1f138-2998">RDBMS</span></span>

* <span data-ttu-id="1f138-2999">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="1f138-2999">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1f138-3000">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="1f138-3000">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1f138-3001">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="1f138-3001">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1f138-3002">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="1f138-3002">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-3003">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-3003">Resource</span></span>

* <span data-ttu-id="1f138-3004">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="1f138-3004">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="1f138-3005">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1f138-3005">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1f138-3006">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1f138-3006">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1f138-3007">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="1f138-3007">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1f138-3008">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="1f138-3008">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1f138-3009">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="1f138-3009">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="1f138-3010">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="1f138-3010">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1f138-3011">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1f138-3011">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1f138-3012">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-3012">Role</span></span>

* <span data-ttu-id="1f138-3013">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1f138-3013">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="1f138-3014">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="1f138-3014">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1f138-3015">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="1f138-3015">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1f138-3016">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="1f138-3016">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="1f138-3017">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="1f138-3017">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1f138-3018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1f138-3018">Service Fabric</span></span>
* <span data-ttu-id="1f138-3019">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="1f138-3019">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1f138-3020">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="1f138-3020">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1f138-3021">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="1f138-3021">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-3022">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-3022">SQL</span></span>

* <span data-ttu-id="1f138-3023">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="1f138-3023">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1f138-3024">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="1f138-3024">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1f138-3025">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="1f138-3025">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-3026">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-3026">Storage</span></span>

* <span data-ttu-id="1f138-3027">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="1f138-3027">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1f138-3028">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="1f138-3028">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1f138-3029">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="1f138-3029">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1f138-3030">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="1f138-3030">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="1f138-3031">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="1f138-3031">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="1f138-3032">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="1f138-3032">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-3033">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-3033">VM</span></span>

* <span data-ttu-id="1f138-3034">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-3034">Support configuring nsg</span></span>
* <span data-ttu-id="1f138-3035">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="1f138-3035">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1f138-3036">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="1f138-3036">Support managed service identities</span></span>
* <span data-ttu-id="1f138-3037">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="1f138-3037">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="1f138-3038">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="1f138-3038">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1f138-3039">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-3039">May 10, 2017</span></span>

<span data-ttu-id="1f138-3040">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1f138-3040">Version 2.0.6</span></span>

* <span data-ttu-id="1f138-3041">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1f138-3041">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1f138-3042">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="1f138-3042">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1f138-3043">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-3043">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="1f138-3044">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1f138-3044">Include Cognitive Services module</span></span>
* <span data-ttu-id="1f138-3045">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1f138-3045">Include Service Fabric module</span></span>
* <span data-ttu-id="1f138-3046">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="1f138-3046">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="1f138-3047">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="1f138-3047">Add support for CDN commands</span></span>
* <span data-ttu-id="1f138-3048">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="1f138-3048">Remove Container module</span></span>
* <span data-ttu-id="1f138-3049">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="1f138-3049">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1f138-3050">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1f138-3050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1f138-3051">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-3051">Core</span></span>

* <span data-ttu-id="1f138-3052">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="1f138-3052">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="1f138-3053">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="1f138-3053">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1f138-3054">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="1f138-3054">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1f138-3055">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="1f138-3055">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1f138-3056">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="1f138-3056">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1f138-3057">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="1f138-3057">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1f138-3058">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="1f138-3058">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1f138-3059">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="1f138-3059">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1f138-3060">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="1f138-3060">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1f138-3061">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="1f138-3061">core: Improved performance</span></span>
* <span data-ttu-id="1f138-3062">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="1f138-3062">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1f138-3063">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="1f138-3063">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-3064">ACS</span></span>

* <span data-ttu-id="1f138-3065">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="1f138-3065">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1f138-3066">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="1f138-3066">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1f138-3067">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="1f138-3067">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1f138-3068">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="1f138-3068">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-3069">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-3069">AppService</span></span>

* <span data-ttu-id="1f138-3070">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="1f138-3070">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1f138-3071">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="1f138-3071">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1f138-3072">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="1f138-3072">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1f138-3073">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="1f138-3073">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1f138-3074">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="1f138-3074">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1f138-3075">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="1f138-3075">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1f138-3076">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="1f138-3076">support slot swap with preview</span></span>
* <span data-ttu-id="1f138-3077">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="1f138-3077">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1f138-3078">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="1f138-3078">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1f138-3079">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1f138-3079">CosmosDB</span></span>

* <span data-ttu-id="1f138-3080">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1f138-3080">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="1f138-3081">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="1f138-3081">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1f138-3082">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="1f138-3082">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1f138-3083">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="1f138-3083">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1f138-3084">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-3084">Data Lake Analytics</span></span>

* <span data-ttu-id="1f138-3085">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="1f138-3085">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="1f138-3086">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="1f138-3086">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1f138-3087">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="1f138-3087">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="1f138-3088">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="1f138-3088">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1f138-3089">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="1f138-3089">Table</span></span>
  * <span data-ttu-id="1f138-3090">Fonction table</span><span class="sxs-lookup"><span data-stu-id="1f138-3090">Table valued function</span></span>
  * <span data-ttu-id="1f138-3091">Affichage</span><span class="sxs-lookup"><span data-stu-id="1f138-3091">View</span></span>
  * <span data-ttu-id="1f138-3092">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="1f138-3092">Table Statistics.</span></span> <span data-ttu-id="1f138-3093">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="1f138-3093">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1f138-3094">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-3094">Data Lake Store</span></span>

* <span data-ttu-id="1f138-3095">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="1f138-3095">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="1f138-3096">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1f138-3096">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1f138-3097">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="1f138-3097">missed help for access show.</span></span> <span data-ttu-id="1f138-3098">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="1f138-3098">adding it.</span></span> <span data-ttu-id="1f138-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1f138-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1f138-3100">Rechercher</span><span class="sxs-lookup"><span data-stu-id="1f138-3100">Find</span></span>

* <span data-ttu-id="1f138-3101">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="1f138-3101">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1f138-3102">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f138-3102">KeyVault</span></span>

* <span data-ttu-id="1f138-3103">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="1f138-3103">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1f138-3104">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="1f138-3104">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="1f138-3105">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="1f138-3105">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1f138-3106">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="1f138-3106">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="1f138-3107">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="1f138-3107">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1f138-3108">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3108">Lab</span></span>

* <span data-ttu-id="1f138-3109">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3109">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="1f138-3110">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3110">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="1f138-3111">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3111">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="1f138-3112">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3112">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="1f138-3113">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="1f138-3113">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="1f138-3114">Moniteur</span><span class="sxs-lookup"><span data-stu-id="1f138-3114">Monitor</span></span>

* <span data-ttu-id="1f138-3115">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="1f138-3115">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1f138-3116">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="1f138-3116">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1f138-3117">Réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-3117">Network</span></span>

* <span data-ttu-id="1f138-3118">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="1f138-3118">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="1f138-3119">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="1f138-3119">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="1f138-3120">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="1f138-3120">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="1f138-3121">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="1f138-3121">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="1f138-3122">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="1f138-3122">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="1f138-3123">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1f138-3123">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="1f138-3124">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="1f138-3124">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="1f138-3125">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="1f138-3125">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="1f138-3126">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="1f138-3126">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="1f138-3127">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="1f138-3127">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1f138-3128">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="1f138-3128">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="1f138-3129">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1f138-3129">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="1f138-3130">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-3130">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="1f138-3131">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="1f138-3131">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="1f138-3132">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="1f138-3132">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="1f138-3133">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="1f138-3133">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="1f138-3134">Profil</span><span class="sxs-lookup"><span data-stu-id="1f138-3134">Profile</span></span>

* <span data-ttu-id="1f138-3135">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="1f138-3135">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1f138-3136">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="1f138-3136">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1f138-3137">Redis</span><span class="sxs-lookup"><span data-stu-id="1f138-3137">Redis</span></span>

* <span data-ttu-id="1f138-3138">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="1f138-3138">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1f138-3139">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="1f138-3139">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="1f138-3140">Ressource</span><span class="sxs-lookup"><span data-stu-id="1f138-3140">Resource</span></span>

* <span data-ttu-id="1f138-3141">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="1f138-3141">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1f138-3142">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="1f138-3142">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1f138-3143">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="1f138-3143">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1f138-3144">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="1f138-3144">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1f138-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1f138-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1f138-3146">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="1f138-3146">Add docs for az lock update.</span></span> <span data-ttu-id="1f138-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1f138-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1f138-3148">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="1f138-3148">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1f138-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1f138-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1f138-3150">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="1f138-3150">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1f138-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1f138-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1f138-3152">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="1f138-3152">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1f138-3153">Role</span><span class="sxs-lookup"><span data-stu-id="1f138-3153">Role</span></span>

* <span data-ttu-id="1f138-3154">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="1f138-3154">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1f138-3155">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="1f138-3155">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1f138-3156">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="1f138-3156">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1f138-3157">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="1f138-3157">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1f138-3158">SQL</span><span class="sxs-lookup"><span data-stu-id="1f138-3158">SQL</span></span>

* <span data-ttu-id="1f138-3159">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="1f138-3159">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="1f138-3160">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="1f138-3160">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1f138-3161">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-3161">Storage</span></span>

* <span data-ttu-id="1f138-3162">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="1f138-3162">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="1f138-3163">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="1f138-3163">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1f138-3164">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="1f138-3164">Add support for large block blob upload</span></span>
* <span data-ttu-id="1f138-3165">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="1f138-3165">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-3166">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-3166">VM</span></span>

* <span data-ttu-id="1f138-3167">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="1f138-3167">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1f138-3168">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="1f138-3168">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1f138-3169">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1f138-3169">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1f138-3170">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1f138-3170">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1f138-3171">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="1f138-3171">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1f138-3172">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="1f138-3172">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1f138-3173">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="1f138-3173">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1f138-3174">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-3174">April 3, 2017</span></span>

<span data-ttu-id="1f138-3175">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1f138-3175">Version 2.0.2</span></span>

<span data-ttu-id="1f138-3176">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="1f138-3176">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="1f138-3177">Core</span><span class="sxs-lookup"><span data-stu-id="1f138-3177">Core</span></span>

* <span data-ttu-id="1f138-3178">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-3178">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="1f138-3179">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="1f138-3179">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1f138-3180">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="1f138-3180">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1f138-3181">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1f138-3181">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1f138-3182">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="1f138-3182">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1f138-3183">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="1f138-3183">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1f138-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="1f138-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1f138-3185">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="1f138-3185">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1f138-3186">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="1f138-3186">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="1f138-3187">ACS</span><span class="sxs-lookup"><span data-stu-id="1f138-3187">ACS</span></span>

* <span data-ttu-id="1f138-3188">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="1f138-3188">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1f138-3189">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="1f138-3189">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1f138-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="1f138-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1f138-3191">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="1f138-3191">Add support for windows clusters.</span></span> <span data-ttu-id="1f138-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="1f138-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1f138-3193">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="1f138-3193">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1f138-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="1f138-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="1f138-3195">AppService</span><span class="sxs-lookup"><span data-stu-id="1f138-3195">AppService</span></span>

* <span data-ttu-id="1f138-3196">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="1f138-3196">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1f138-3197">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="1f138-3197">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1f138-3198">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="1f138-3198">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1f138-3199">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="1f138-3199">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="1f138-3200">DataLake</span><span class="sxs-lookup"><span data-stu-id="1f138-3200">DataLake</span></span>

* <span data-ttu-id="1f138-3201">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1f138-3201">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="1f138-3202">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1f138-3202">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="1f138-3203">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="1f138-3203">DocuemntDB</span></span>

* <span data-ttu-id="1f138-3204">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="1f138-3204">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1f138-3205">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1f138-3205">VM</span></span>

* <span data-ttu-id="1f138-3206">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="1f138-3206">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1f138-3207">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="1f138-3207">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1f138-3208">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="1f138-3208">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1f138-3209">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1f138-3209">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1f138-3210">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="1f138-3210">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1f138-3211">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="1f138-3211">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="1f138-3212">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="1f138-3212">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1f138-3213">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="1f138-3213">February 27, 2017</span></span>

<span data-ttu-id="1f138-3214">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1f138-3214">Version 2.0.0</span></span>

<span data-ttu-id="1f138-3215">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="1f138-3215">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="1f138-3216">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="1f138-3216">Container Service (acs)</span></span>
- <span data-ttu-id="1f138-3217">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="1f138-3217">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1f138-3218">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="1f138-3218">Networking</span></span>
- <span data-ttu-id="1f138-3219">Stockage</span><span class="sxs-lookup"><span data-stu-id="1f138-3219">Storage</span></span>

<span data-ttu-id="1f138-3220">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1f138-3220">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="1f138-3221">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1f138-3221">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="1f138-3222">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="1f138-3222">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="1f138-3223">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="1f138-3223">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="1f138-3224">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="1f138-3224">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="1f138-3225">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="1f138-3225">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1f138-3226">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="1f138-3226">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1f138-3227">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1f138-3227">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="1f138-3228">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1f138-3228">Provide feedback from the command line with the `az feedback` command</span></span>

